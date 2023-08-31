# Week 1 - Day 4

## The story so far...

### JavaScript Control Flow

* Conditional Statements
  * `if` some value is `true` or `false` _then_ do some thing...`else` do another thing.
  * NOTE: `else` is optional, and JavaScript technically [does not have an `else if` syntax!](https://dev.to/genta/theres-no-else-if-in-js--24f9)
* Loops
  * `for` every item in a group of items, do a thing over and over until a predetermined "stop" event happens, i.e. a certain number of loops is reached.
  * `forEach` "needle" in a "haystack" do some thing.
  * `while` some condition is met, do a thing. Stop the loop when the condition is no longer met.

### The DOM

* Document
* Object
* Model

This is the in-memory representation of the page you're veiwing in the browser. JavaScript can interact with a page via methods and APIs that expose DOM elements to JavaScript. You can add, remove, edit, read, HTML elements, i.e. `<p>` tags, by querying the `document` object, aka the "root" of the DOM. This is one of many items provided by the **browser** (not unique to JS!) as part of the Browser API.

### Scope

* "global" scope variables are available to an entire application.
* "local" scope limits variables to where they were created.
* Functions can access variables in their local scope _and_ anything in the global scope.
* Functions cannot access variables in the scope of other functions.
* Locally scoped variables are not available globally.

### JavaScript is asynchronous

* When given a series of commands, i.e. functions/method, JavaScript doesn't wait for one command to finish before moving on to the next.
* JavaScript uses an Event Loop, a call stack and event queue kept in memory, to keep track of that status of each function.
* It adds each task to the queue, and returns the result of each task as they are **completed** not as they are **submitted**.
* We are also asynchronous, we can start any number of tasks and complete them regardless of the order in which they were started (i.e. Doing a morning routine that consists of making coffee, doing laundry, emptying the dishwasher.)

### Call me maybe??

* JavaScript uses "Callbacks", a functions that is passed as an argument to another function, to handle asynchronous events.
* A function starts, it's added to the call stack and event queue, when it's done the resulting data is given to the "callback" function.
* This is useful when a particular function _needs_ to wait on the data from a previous function.

## Recommended Reading

* [Frontend Weekly: Ajax — Async, Callback & Promise](https://medium.com/front-end-weekly/ajax-async-callback-promise-e98f8074ebd7)

## Helpful Links

* [Vanilla JS Toolkit](https://vanillajstoolkit.com/plugins/)

## Keywords

* objects
* event listeners
* event loop
* DOM
* selectors
* elements
* callbacks
* scope
