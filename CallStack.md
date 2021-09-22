# CallStack  

**What It Is and Why It's Necessary**


The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.


The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.


In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

**LIFO**: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

## Manage function invocation (call): 

The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.



### This is what happens when the code is run:

*  **When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.**

* **. secondFunction() then calls firstFunction()which is pushed into the stack.**
* **firstFunction() returns and prints “Hello from firstFunction” to the console.**
* **firstFunction() is pop off the stack.**
* **The execution order then move to secondFunction().**
* **secondFunction() returns and print “The end from secondFunction” to the console.**
* **secondFunction() is pop off the stack, clearing the memory.**
👍

## In summary

The key **`takeaways`** from the call stack are:

* **It is single-threaded. Meaning it can only do one thing at a time.**
* **Code execution is synchronous.**
* **A function invocation creates a stack frame that occupies a temporary memory.**
* **It works as a LIFO — Last In, First Out data structure**

We have used the call stack article to lay the foundation for a series we will be looking at on Asynchronous JavaScript (which we will be looking at in another article).



All code samples can be found in this GitHub [repo](https://github.com/charlesfreeborn/JS-CallStack-CodeSamples/blob/master/codesamples.md).