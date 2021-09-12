#  Component Lifecycle Events

## What are component lifecycle events? 

**React** lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

**let us talk in details and list them**

* Mounting 
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static **getDerivedStateFromProps, render, componentDidMount,** and UNSAFE_componentWillMount all occur in this order during mounting.
* Updting 
**Anytime** a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
* Unmounting 
The final phase of the lifecycle if called when a component is being removed from the DOM. [componentWillUnmount](https://reactjs.org/docs/react-component.html#static-getderivedstatefromprops) is the only lifecycle event during this phase.


### componentDidMount()

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in **componentWillUnmount().**



### UNSAFE Lifecycle Events

* [UNSAFE_componentWillMount()](https://reactjs.org/docs/react-component.html#unsafe_componentwillmount)
* [UNSAFE_componentWillUpdate()](https://reactjs.org/docs/react-component.html#unsafe_componentwillupdate)
* [UNSAFE_componentWillReceiveProps()](https://reactjs.org/docs/react-component.html#unsafe_componentwillreceiveprops)