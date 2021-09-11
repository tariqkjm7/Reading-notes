# Component


## What is a Component?

A **component** is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.


## Characteristics of Components

* **Reusability:** Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
* **Replaceable:** Components may be freely substituted with other similar components.
* **Not context specific:** Components are designed to operate in different environments and contexts.
* **Extensible:** A component can be extended from existing components to provide new behavior.
* **Encapsulated:** A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state. 
* **Independent:** Components are designed to have minimal dependencies on other components.

## **Advantages**
* **Ease of deployment**
* **Reduced cost**
* **Reusable**
* **Modification of technical complexity**
* **Reliability**
* **System maintenance and evolution**
* **Independent**

# props
## What is Props?
**React is a component-based library** which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using **props**.

## How are props used in React?

* Firstly, define an attribute and its value(data)
* Then pass it to child component(s) by using Props
* Finally, render the Props Data



## What is the flow of props?
from the parent until the last child 
so it will be parent ==> 1st-cild ==> 2nd-child ==> 3rd-child==>......==> Nth-child.