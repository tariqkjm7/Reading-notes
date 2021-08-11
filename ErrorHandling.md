# Error Handling & Debugging

JavaScript can be hard to learn and everyone makes mistakes when writing it.  This chapter will help you learn how to find the errors in your code. It will also teach you how to write scripts that deal with potential errors gracefully. 

When you are writing JavaScript, do not expect to write it perfectly t he fi rst time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too. When writing a long script, nobody gets everything right in their first attempt. The error m essages that a browser gives look cryptic at first, but they can help you determine what went wrong in your JavaScript and how to fix it. 



## **EXECUTION CONTEXTS**

The JavaScript interpreter uses the concept of **execution contexts.** There is  one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 

EXECUTION CONTEXT Every statement in a script lives in one of three execution contexts: 

* GLOBAL CONTEXT:

Code that is in the script, but not in a fu nction. There is only one global context in any page. 


* FUNCTION CONTEXT

 Code that is being run within a function. Each function has its own function context. 

 * EVAL CONTEXT (NOT SHOWN)
 
  Text is executed like code in an internal function called eva l {) (which is not covered in this book). 


  ## **VARIABLE SCOPE** 
  
  The first two execution contexts correspond with the notion of scop


  * GLOBAL SCOPE
  
   If a variable is declared outside a fu nction, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope


* FUNCTION-LEVEL 

SCOPE When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope. 


## **UNDERSTANDING SCOPE** 

In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.


 Functions in JavaScript are said to have lexical scope. They are linked to the object they were defined within. So, for each execution context, t he scope is the current execution context's variables object, plus the variables object for each parent execution context.



## **UNDERSTANDING ERRORS**

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. 


If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error (you meet them on p480). This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.



![img](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQfvH0uQktWRkCsoF1QF2QZeza-2ceXM0heyw&usqp=CAU)
