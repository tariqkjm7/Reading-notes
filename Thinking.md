# Thinking 
One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.


**we have many steps so let's get started**

* **Break The UI Into A Component Hierarchy**

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!


*  **Build A Static Version in React.**


Now that you have your component hierarchy, it’s time to implement your app. The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and ** ❌not** a lot of typing.


* **Identify The Minimal (but complete) Representation Of UI State.**


To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with **state.**

To build your app correctly, you first need to think of the minimal set of mutable state that your app needs. The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand. For example, if you’re building a TODO list, keep an array of the TODO items around; don’t keep a separate state variable for the count. Instead, when you want to render the TODO count, take the length of the TODO items array.

**Think of all the pieces of data in our example application. We have:**


* **The original list of products**
* **The search text the user has entered**
* **The value of the checkbox**
* **The filtered list of products**



**Let’s go through each one and figure out which one is state. Ask three questions about each piece of data:**


* Is it passed in from a parent via props? If so, it probably isn’t state.

* **Does it remain unchanged over time? If so, it probably isn’t state.**
* **Can you compute it based on any other state or props in your component? If so, it isn’t state.**


to know more [click here](https://reactjs.org/docs/thinking-in-react.html)