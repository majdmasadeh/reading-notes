# welcome to read 10 

## Error Handling And Debugging

![img](https://images.slideplayer.com/31/9700382/slides/slide_2.jpg)


### What is **Debugging**

> Debugging is a process for testing, finding the errors and reducing them from happening in future. Debugging JavaScript either requires having support for JavaScript debugger keyword, breakpoint support with web browser tools, or third-party tools. These tools range from browser plugins like Augury which is an Angular development and debugging extension for Chrome, third-party tools & more. It is also possible to use 'debugger' keyword support (depending on the browser type and version) and to freeze the code at a given point and investigate the issue. Let us look at few popular debugging and error handling tools.

### Why errors happened ?
 - some times the excution order can be the reason to have an error, because some asks cannot complete until another statement or function has been run in a certain order.

 ## Javascript Execution Context and Hoisting

 ![hoisting](https://miro.medium.com/max/875/1*wXTMuOB_HSMTZlfM2V4xIQ.png)

 > Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.


### If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling  code.

## Error Objects 
> Error objects can help you find where your mistakes areand browsers have tools to help you read them. 

## There are seven types of built-in error objects in JavaScript. 

1. SyntaxError 
   - SYNTAX IS NOT CORRECT : This is caused by incorrect use of the rules of the language. It is often the result of a simple typo. 

2. ReferenceError
   -  VARIABLE DOES NOT EXIST : This is caused by a variable that is not declared or is out of scope.

3.  EvalError 
   - INCORRECT USE OF eval() FUNCTION The eval () function evaluates text through the interpreter and runs it as code. It is rare that you would see this type of error, as browsers often throw other errors when they are supposed to throw an Eva 1 Error.

4. URIError 
   - INCORRECT USE OF URI FUNCTIONS : If these characters are not escaped in URls, they will cause an error: / ? & I : ; 

5.    TypeError
   - VALUE IS UNEXPECTED DATA TYPE : This is often caused by trying to use an object or method that does not exist.

6.  RangeError 
   - NUMBER OUTSIDE OF RANGE : If you call a function using numbers outside of its accepted range. 

7. Error
   -  GENERIC ERROR OBJECT : The generic Error object is the template (or prototype) from which all other error objects are created.  



 ###   HOW TO LOOK AT ERRORS IN CHROME ??

 > The console will show you when there is an error in your JavaScript. It also displays the line where it became a problem for the interpreter. 

 ### How to we handle exceptions 
  - using one of these ;

  1. TRY 
  2. CATCH
  3. FINALLY

  

