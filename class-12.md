# chart in java
 
**getElementsAtEvent(e)**
Looks for the element under the event point, then returns all elements at the same data index. This is used internally for 'label' mode highlighting.

Calling getElementsAtEvent(event) on your Chart instance passing an argument of an event, or jQuery event, will return the point elements that are at that the same position of that event.

canvas.onclick = function(evt) {
    var activePoints = myLineChart.getElementsAtEvent(evt);
    // => activePoints is an array of points on the canvas that are at the same position as the click event.
};
This functionality may be useful for implementing DOM based tooltips, or triggering custom behaviour in your application.

**getDatasetAtEvent(e)**
Looks for the element under the event point, then returns all elements from that dataset. This is used internally for 'dataset' mode highlighting.

myLineChart.getDatasetAtEvent(e);
// => returns an array of elements
.getDatasetMeta(index)
Looks for the dataset that matches the current index and returns that metadata. This returned data has all of the metadata that is used to construct the chart.

**Updating Charts**
It's pretty common to want to update charts after they've been created. When the chart data or options are changed, Chart.js will animate to the new data values and options.

Adding or Removing Data
Adding and removing data is supported by changing the data array. To add data, just add data into the data array as seen in this example.

function addData(chart, label, data) {
    chart.data.labels.push(label);
    chart.data.datasets.forEach((dataset) => {
        dataset.data.push(data);
    });
    chart.update();
}

function removeData(chart) {
    chart.data.labels.pop();
    chart.data.datasets.forEach((dataset) => {
        dataset.data.pop();
    });
    chart.update();
}
Updating Options
To update the options, mutating the options property in place or passing in a new options object are supported.

**New Charts**
Chart.js 2.0 introduces the concept of controllers for each dataset. Like scales, new controllers can be written as needed.

Chart.controllers.MyType = Chart.DatasetController.extend({

});


// Now we can create a new instance of our chart, using the Chart.js API
new Chart(ctx, {
    // this is the string the constructor was registered at, ie Chart.controllers.MyType
    type: 'MyType',
    data: data,
    options: options
});
**New Axes**
Axes in Chart.js can be individually extended. Axes should always derive from Chart.Scale but this is not a mandatory requirement.

let MyScale = Chart.Scale.extend({
    /* extensions ... */
});
Once you have created your scale class, you need to register it with the global chart object so that it can be used. A default config for the scale may be provided when registering the constructor. The first parameter to the register function is a string key that is used later to identify which scale type to use for a chart.

Chart.scaleService.registerScaleType('myScale', MyScale, defaultConfigObject);
To use the new scale, simply pass in the string key to the config when creating a chart.

var lineChart = new Chart(ctx, {
    data: data,
    type: 'line',
    options: {
        scales: {
            yAxes: [{
                type: 'myScale' // this is the same key that was passed to the registerScaleType function }]} }});