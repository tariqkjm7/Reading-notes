# Functional Programming 

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data


## Pure functions

![anything](https://miro.medium.com/max/875/0*FMur6URY7yAVjeuP)



The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?



So how do we know if a function is pure or not? Here is a very strict definition of purity:



* It returns the same result if given the same arguments (it is also referred as deterministic)
* It does not cause any observable side effects



### **It returns the same result if given the same arguments**.


Imagine we want to implement a function that calculates the area of a circle. An impure function would receive radius as the parameter, and then calculate radius *radius* PI:


**It does not cause any observable side effects**

Examples of observable side effects include modifying a global object or a parameter passed by reference.
Now we want to implement a function to receive an integer value and return the value increased by 1.

We have the *counter* value. Our impure function receives that value and re-assigns the counter with the value increased by 1.



## **Observation:**
mutability is discouraged in functional programming.
We are modifying the global object. But how would we make it pure? Just return the value increased by 1. Simple as that.


See that our pure function increaseCounter returns 2, but the counter value is still the same. The function returns the incremented value without altering the value of the variable.
If we follow these two simple rules, it gets easier to understand our programs. Now every function is isolated and unable to impact other parts of our system.


**Pure functions benefits**

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

* Given a parameter *A* → expect the function to return value *B*

* Given a parameter *C* → expect the function to return value *D*