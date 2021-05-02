# chapter 6 in html
##  table 

The <table> element is used to add tables to a web page. table is drawn out row by row. Each row is created with the <tr> element.Inside each row there are a number of cells represented by the <td> element (or <th> if it is a header).You can make cells of a table span more than one row or column using the rowspan and colspan attributes. For long tables you can split the table into a <thead>, 
<tbody>, and <tfoot>

![table](https://vertex-academy.com/tutorials/wp-content/uploads/2016/08/table.png)
The HTML table model allows authors to arrange data -- text, preformatted text, images, links, forms, form fields, other tables, etc. -- into rows and columns of cells.

Each table may have an associated caption (see the CAPTION element) that provides a short description of the table's purpose. A longer description may also be provided (via the summary attribute) for the benefit of people using speech or Braille-based user agents.

Table rows may be grouped into a head, foot, and body sections, (via the THEAD, TFOOT and TBODY elements, respectively). Row groups convey additional structural information and may be rendered by user agents in ways that emphasize this structure. User agents may exploit the head/body/foot division to support scrolling of body sections independently of the head and foot sections. When long tables are printed, the head and foot information may be repeated on each page that contains table data.

Authors may also group columns to provide additional structural information that may be exploited by user agents. Furthermore, authors may declare column properties at the start of a table definition (via the COLGROUP and COL elements) in a way that enables user agents to render the table incrementally rather than having to wait for all the table data to arrive before rendering.
![tab](https://flaviocopes.com/html-tables/no-styling.png)

You may want to consider using HTML tables in your website. In addition to creating HTML tables to present data in rows and columns, you can also create HTML tables to organize information on your web page.

The process of creating an HTML table is similar to the process that you used to create your web page and any elements that you may have already included in your page, such as links or frames. Coding HTML tables into your web page is fairly easy since you need only understand a few basic table codes.

** Creating a basic table **

The basic structure of an HTML table consists of the following tags:

1. Table tags:  <TABLE> </TABLE>
2. Row tags:   <TR> </TR>
3. Cell tags:    <TD> </TD>

# chapter 3
## function, method  and object

object is a combination of data and procedures working on the available data. An object has a state and behavior.

The state of an object is stored in fields (variables), while methods (functions) display the object's behavior. Objects are created from templates known as classes.

In Java, an object is created using the keyword "new".

ava objects are very similar to the objects we can observe in the real world. A cat, a lighter, a pen, or a car are all objects.

They are characterized by three features:

- Identity

- State

- Behavior

** What is Object in Java? **
Object is an instance of a class. An object in OOPS is nothing but a self-contained component which consists of methods and properties to make a particular type of data useful. For example color name, table, bag, barking. When you send a message to an object, you are asking the object to invoke or execute one of its methods as defined in the class.

From a programming point of view, an object in OOPS can include a data structure, a variable, or a function. It has a memory location allocated. Java Objects are designed as class hierarchies.

Syntax

ClassName ReferenceVariable = new ClassName();

Java is an object-oriented programming language.

Everything in Java is associated with classes and objects, along with its attributes and methods. For example: in real life, a car is an object. The car has attributes, such as weight and color, and methods, such as drive and brake.

A Class is like an object constructor, or a "blueprint" for creating objects.

![object](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQshAYTTJXZJAkT8QGgGelzOpGjTx4v490Vlg&usqp=CAU)

JavaScript is designed on a simple object-based paradigm. An object is a collection of properties, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as a method. In addition to objects that are predefined in the browser, you can define your own objects. This chapter describes how to use objects, properties, functions, and methods, and how to create your own objects.

Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. The concept of objects in JavaScript can be understood with real life, tangible objects.

In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

# Domain modeling 

**Domain modeling** is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

### Define a constructor and initialize properties

*To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.*

|Property   | Data         | Type   |
|-----------|--------------|--------|
| epicRating|1 to 10       | Number |
| hasAnimals| true or false| Boolean|
