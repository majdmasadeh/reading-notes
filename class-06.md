# chapter 3
## object literals
Object literals are used to create an object in javascript. Enhancement in Object literals in ES2015 (ES6) release has made it a more powerful feature.

1. The object in javascript can be initialized by directly using the   variable name. See Example 1 below.
2. Object’s method in ES5 requires function statement. This is no longer required in ES6, you can directly return statement. 
3. Object literals key in ES6 can be dynamic. Any Express can be used to create a key.

** The this Keyword **
In a function definition, this refers to the "owner" of the function In the example above, this is the person object that "owns" the fullName function.
In other words, this.firstName means the firstName property of this object.

** Example **
var person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
![img](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTdiGyi-Z1hl6XJ9M6BfsMVX1yLk1WDaZsz4A&usqp=CAU0)

* There are three ways of creating an object in javascript. *
- Using Object literals
- Using new keyword.
- By defining object constructor and then create an object constructor type.

![object](https://image.slidesharecdn.com/jsoreillywebinar-140805111842-phpapp02/95/intro-to-javascript-15-638.jpg?cb=1407237609)

# chapter 5 
## Document Object Model (DOM)

![disc](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTSXNaeOUAiRVk0C10wfZUX3ytECSzkvWZiGg&usqp=CAU)

The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web. In this guide, we'll briefly introduce the DOM. We'll look at how the DOM represents an HTML or XML document in memory and how you use APIs to create web content and applications.

What is the DOM?
The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

A Web page is a document. This document can be either displayed in the browser window or as the HTML source. But it is the same document in both cases. The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.

The W3C DOM and WHATWG DOM standards are implemented in most modern browsers. Many browsers extend the standard, so care must be exercised when using them on the web where documents may be accessed by various browsers with different DOMs.

For example, the standard DOM specifies that the querySelectorAll method in the code below must return a list of all the <p> elements in the document:
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);

** Properties of document object **
Let's see the properties of document object that can be accessed and modified by the document object. 
![dom](https://miro.medium.com/max/1200/1*5zKczvG219FSLibHQH4jSA.png)
