# Keys 

**Keys** help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.


## Keys Must Only Be Unique Among Siblings
Keys used within arrays should be unique among their siblings. However, they don’t need to be globally unique. We can use the same keys when we produce two different arrays.

### recommendtion

**We don’t recommend using indexes for keys if the order of items may change. This can negatively impact performance and may cause issues with component state. Check out Robin Pokorny’s article for an in-depth explanation on the negative impacts of using an index as a key. If you choose not to assign an explicit key to list items then React will default to using indexes as keys.**

InJavaScript, [spread syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax) refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.



## routine tasks
The **(…)** spread operator is useful for many different routine tasks in JavaScript, including the following:

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

**One of the best ways to understand the use of spread operator in JavaScript is to look at the the built-in functions Math.min() and [Math.max()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/max), which both expect a list of arguments, not an array.**


## Using an array as arguments

**Since the spread operator “spreads” an array into different arguments, any functions that accepts multiple any number of arguments can benefit from use of the spread operator.**