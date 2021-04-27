# HTML Texts

- Headings and paragraphs
- Bold, italic, emphasis
- Structural and semantic markup

## Headings
![img1](https://i.ytimg.com/vi/LuHUU9ladBQ/maxresdefault.jpg)

### Paragraphs
<p> To create a paragraph, surround the words that make up the paragraph with an opening <p> tag and closing </p> tag.

#### Bold & Italic

**** By enclosing words in the tags and </b> we can make characters appear bold.

**** By enclosing words in the tags and </i> we can make characters appear italic.

#### semantic markup.

< strong> The use of the < strong>element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.

< em> The < em> element indicates emphasis that subtly changes the meaning of a sentence

< blockquote> The < blockquote> element is used for longer quotes that take up an entire paragraph. Note how the < p> element is still used inside the < blockquote> element. 
![img2](https://miro.medium.com/max/1000/1*zHJFnu7QF-PgUb8108aLcA.png)

# Introducing CSS

## BLOCK & INLINE ELEMENTS
Block level elements look like they start on a new line.

* why css :

CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented

* CSS associates style rules with HTML elements :


CSS properties affected of how the elements are displayed

 



CSS file: body {

font-family: Arial, Verdana, sans-serif; } h1, h2 {

color: #ee3e80; } p {

color: #665544; }

## Ways to link CSS with HTML:
![img3](https://www.bitdegree.org/learn/storage/media/images/8c4493d3-110c-4a95-8b70-7626ce2d2f4e.jpg)

## An Overall
- CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
- Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
- Different types of selectors allow you to target your rules at different elements.
Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document, although they may appear within an HTML page.


# JAVASCRIPT

## Chapter 2: “Basic JavaScript Instructions”

### What is JavaScript?
JavaScript is a scripting or programming language that allows you to implement complex features on web pages every time a web page does more than just sit there and display static information for you to look at displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies

### why JavaScript?
JavaScript is one of the 3 languages all web developers must learn:

HTML to define the content of web pages

CSS to specify the layout of web pages

JavaScript to program the behavior of web pages

### JavaScript Data Types:
![img4](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-data-types.jpg)

# Dicision and loops
- Conditional statements allow your code to make decisions about what to do next.
- Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands.
Logical operators allow you to combine more than one set of comparison operators.
- if … else statements allow you to run one set of code if a condition is true, and another if it is false. switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).
- Data types can be coerced from one type to another.
- All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and do … while. Each repeats a set of statements.

Comparison and logical operators
1- Comparsion Operators :
You can evaluate a situation by comparing on value in the script to what you expect it might be. The result will be a boolean True or False .

**== IS EQUAL TO ** We use this operators to compare two values (numbers, strings and booleans) to see if they are the same .

!= IS NOT EQUAL TO We use this operators to compare two values (numbers, strings and booleans) to see if they are Not the same .

=== STRICT EQUAL TO ** We use this operators to compare two values to see if they are the same in **Vlaue and Data type

!== NOT STRICT EQUAL TO ** We use this operators to compare two values to see if they are **NOT ** the same in **Vlaue and Data type

> GREATER THAN ** We use this operators to check if the number in the left side is **great than the number in the right side.

< LESS THAN ** We use this operators to check if the number in the left side is **less than the number in the right side.

>= GREATER THAN OR EQUAL TO ** We use this operators to check if the number in the left side is **great than or equal the number in the right side.

<= LESS THAN OR EQUAL TO We use this operators to check if the number in the left side is less than or equal the number in the right side.

2- Logical Operators
Comparsion operators usually return single values of True or False . Logical operators allow you to compare the result of more thane one compartion operator.

&& LOGICAL AND This operatos is test more than one contion.
Lgical AND Truth Table	 	 	 	 
Left Side	 	Right Side	 	Result of &&
T	 	T	 	T
T	 	F	 	F
F	 	T	 	F
F	 	F	 	F
**|| LOGICAL OR ** This operatos is test at least one contion.
Lgical OR Truth Table	 	 	 	 
Left Side	 	Right Side	 	Result of &&
T	 	T	 	T
T	 	F	 	T
F	 	T	 	T
F	 	F	 	F
**! LOGICAL NOT ** This operator take a single boolean value and inverts it .
Lgical OR Truth Table	 	 
Value	 	Result
T	 	F
F	 	T
LOOPS
Loops check a condition, if its retrn true, a code block it will run. Then the condition will be checked again and if it still returns true,the code block will run again .It repeats until the condition returns false.

- There are Three Common types of Loops
** 1- FOR LOOP ** : If you need to run a code a specific number of times, use a for loop (its the most common loop ). In a for loop, a condition is usually a counter which is used to tell how many times the loop should run.

![img5](https://www.javascripttutorial.net/wp-content/uploads/2020/01/JavaScript-for-Loop.png) . 

** 2- WHILE LOOP **: If you do not know how many time the code should run, you can use a **while **loop. Here the condition can be something other than a counter, and the code will continue to loop as long as the condition is true.

![img6](https://cdn.programiz.com/sites/tutorial2program/files/javascript-while-loop.png)

** 3- Switch Statment : **
![img7](https://media.geeksforgeeks.org/wp-content/uploads/switch-statement-flowchart.png)

