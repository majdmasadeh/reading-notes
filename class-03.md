# Lists
 here are three types of HTML lists:
 ordered, unordered, and definition.
- Ordered lists use numbers.
- Unordered lists use bullets.
- Definition lists are used to define terminology.
- Lists can be nested inside one another.
![img](http://ways2web.weebly.com/uploads/5/4/4/8/54485903/8033093_orig.png)

Nested Lists
You can put a second list inside an <li> element to create a sublist or nested list.

![img2](https://s3.amazonaws.com/webucator-how-tos/419.png)


#  Boxes:
![img3](https://i.stack.imgur.com/PSuyr.png)

At the beginning of this section on CSS, you saw how CSS treats each HTML element as if it lives in its own box. You can set several properties that affect the appearance of these boxes. In this chapter you will see how to:

● Control the dimensions of your boxes
 ● Create borders around boxes 
 ● Set margins and padding for boxes 
 ● Show and hide boxes

Once you have learned how to control the appearance of each box, you will see how to position these boxes on your pages in Chapter 15 when we look at page layout.

## Box Dimensions
width, height By default, a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties. The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size. When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box. When you use ems, the size of the box is based on the size of the text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible across devices that have different-sized screens. In the example on the right, you can see that a containing <div> element is used which is 300 pixels wide by 300 pixels high. Inside of this is a paragraph that is 75% of the width and height of the containing element. This means that the size of the paragraph is 225 pixels wide by 225

## Parts of box : 
Content - The content of the box, where text and images appear Padding - Clears an area around the content. The padding is transparent
Border - A border that goes around the padding and content Margin - Clears an area outside the border. The margin is transparent
In order to set the width and height of an element correctly in all browsers, you need to know how the box model works. 
When you set the width and height properties of an element with CSS, you just set the width and height of the content area. To calculate the full size of an element, you must also add padding, borders and margins

## Box Dimensions:
width
height
* Limiting Width:
min-width
max-width
* Limiting Height:
min-height
max-height
* Overflowing Content
1. overflow
2. hidden
3. scroll
![img4](https://miro.medium.com/max/1276/1*PGOsy3OmNgYwHaomZbYePQ.png)

## Border, Margin & Paddin
1- Border
Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

Border Width border-width border-top-width border-right-width border-bottom-width border-left-width

Border Style border-style border-style: solid; border-style: dotted; border-style: dashed; border-style: double; border-style: groove; border-style: ridge; border-style: inset; border-style: outset;

Border Color border-color border-top-color border-right-color border-bottom-color border-left-color

2- Margin
Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

Margin margin margin-top margin-right margin-bottom margin-left

3- Padding
Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

Padding padding padding-top padding-right padding-bottom padding-left

Change Inline/Block
display display: inline display: block display: inline-block display: none

### Hiding Boxes
visibility visibility: hidden; visibility: visible;

CSS treats each HTML element as if it has its own box.
You can use CSS to control the dimensions of a box.
You can also control the borders, margin and padding for each box with CSS.
It is possible to hide elements using the display and visibility properties.
Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
Legibility can be improved by controlling the width of boxes containing text and the leading.
CSS3 has introduced the ability to create image borders and rounded borders

# “Basic JavaScript Instructions”

## ARRAYS
An array is a special type of variable. It doesn’t just store one value; it stores a list of values.

## CREATING AN ARRAY
You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array. This technique for creating an array is known as an array literal. It is usually the preferred method for creating an array. You can also write each value on a separate line. colors= ['white', 'black', 'custom']

## VALU ES IN ARRAYS
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).
![img6](https://www.tutsmake.com/wp-content/uploads/2020/05/JavaScript-Arrays.jpeg)

## SWITCH STATEMENTS
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).
![img7](https://miro.medium.com/max/762/1*0KACYGFFuTfXQcVpL70CeA.png)

#Loops
## For Loops
![img8](https://www.javascripttutorial.net/wp-content/uploads/2020/01/JavaScript-for-Loop.png)

## While Loop
![img9](https://www.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-while-loop.png)
