# Forms

* HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.

* The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

## Form Controls

There are several types of form controls that you can use to collect information from visitors to your site. 

1. Text input
2. Password input
3. Text area
4. Radio buttons
5. Checkboxes
6. Drop-down boxes
7. Submit buttons
8. Image buttons
9. File upload

## How Forms Work

*A user fills in a form and then presses a button to submit the information to the server*

## Form Structure

*Form controls live inside a <form> element. This element should always carry the action attribute and will usually have a method and id attribute too.*

*action Every <form> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted. method Forms can be sent using one of two methods: get or post.*

### Text Input

*The input element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.*

### Password Input

*type="password" When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.*

### Text Area

The textarea element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag.*

### Radio Button

*type="radio" Radio buttons allow users to pick just one of a number of options.*

### Checkbox

*type="checkbox" Checkboxes allow users to select (and unselect) one or more options in answer to a question*

### Drop Down List Box

*A drop down list box (also known as a select box) allows users to select one option from a drop down list.*

### Multiple Select Box

#### File Input Box

*If you want to allow users to upload a file (for example an image, video, mp3, or a PDF), you will need to use a file input box.*

### Submit Button

*type="submit" The submit button is used to send a form to the server.*

#### Grouping Form Elements

*You can group related form controls together inside the element. This is particularly helpful for longer forms.*

### Form Validation

*You have probably seen forms on the web that give users messages if the form control has not been filled in correctly; this is known as form validation.*

### HTML5: Date Input

*Many forms need to gather information such as dates, email addresses, and URLs. This has traditionally been done using text inputs.*

### Email & URL Input

*HTML5 has also introduced inputs that allow visitors to enter email addresses and URLs. Browsers that do not support these input types will just treat them as text boxes.*

1. type="email" If you ask a user for an email address, you can use the email input. Browsers that support HTML5 validation will check that the user has provided information in the correct format of an email address. Some smart phones also optimize their keyboard to display the keys you are most likely to need when entering an email address (such as the @ symbol).

3. type="url" A URL input can be used when you are asking a user for a web page address. Browsers that support HTML5 validation will check that the user has provided information in the format of a URL. Some smart phones also optimize their keyboard to display the keys you are most likely to need when entering a URL.

### HTML5: Search Input

*If you want to create a single line text box for search queries, HTML5 provides a special type of input for that purpose.*

### Images for Bullets

*You can specify an image to act as a bullet point using the list-style-image property. The value starts with the letters url and is followed by a pair of parentheses. Inside the parentheses, the path to the image is given inside double quotes.*

### Positioning the Marker

*Lists are indented into the page by default and the list-style�position property indicates whether the marker should appear on the inside or the outside of the box containing the main points. This property can take one of two values:*

1. outside
2. inside

### List Shorthand

*As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order.*

### Table Properties

*You have already met several properties that are commonly used with tables. Here we will put them together in a single example using the following.*

1. width to set the width of the table.
2. padding to set the space between the border of each table cell and its content.
3. text-transform to convert the content of the table headers to uppercase.
4. etter-spacing, font-size to add additional styling to the content of the table headers.
5. border-top, border-bottom to set borders above and below the table headers.
6. text-align to align the writing to the left of some table cells and to the right of the others.
7. background-color to change the background color of the alternating table rows.
8. hover to highlight a table row when a user's mouse goes over it.

### Cursor Styles

*he cursor property allows you to control the type of mouse cursor that should be displayed to users. For example, on a form you might set the cursor to be a hand when the user hovers over it. Here are the most commonly used values for this property*

### Web Developer Toolbar

*This helpful extension for Firefox and Chrome provides tools to show you the CSS styles that apply to an element when you hover over it, along with the structure of the HTML.*

### Events

*When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events.*

### HOW EVENTS TRIGGER JAVASCRIPT CODE

*When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.*

*Select t he element node(s) you want the script to respond to.*

*Indicate which event on the selected node(s) will trigger the response.*

*State the code you want to run when the event occurs. HTML EVENT HANDLER ATTRIBUTES (DO NOT USE).*

*TRADITIONAL DOM EVENT HANDLERS All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler.*

*Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.*

### THE EVENT OBJECT

*When an event occurs, the event object tells you information about the event, and the element it happened upon.*

*Below you can see how you get the event object in IES-8. It is not passed automatically to event handler/listener functions; but it is available as a child of the window object.*

### EVENT DELEGATION

*Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.*

### USER INTERFACE EVENTS

*User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it, e.g., a page having loaded or the browser window being resized.*

### FOCUS & BLUR EVENTS

*The HTML elements you can interact with, such as links and form elements, can gain focus. These events fire when they gain or lose focus.*

### MUTATION EVENTS & OBSERVERS

*Whenever elements are added to or removed from the DOM, its structure changes. This change triggers a mutation event.*