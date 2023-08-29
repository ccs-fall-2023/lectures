# Exercises

## JS MadLibs: Part 1

Start by creating a fork of this starter repo: [https://github.com/seanrreid/DOM-Starter-Code](https://github.com/seanrreid/DOM-Starter-Code).

### Update the starter code with the following

* A `form` to accept user input.
* `input` elements to collect user's responses.
* A `button` element to __submit__ the form.
* Placeholder elements that will be updated with user's responses.

## JS MadLibs: Part 2

### Here's what we need to do this

* We need to select a placeholder element (or _all_ the placeholder elements).
* We need words to replace the placeholders.
* We need a button to trigger the replacement when clicked.

### Here's how we're going to break it down

#### Update one at a time

1. Grab each input and each placeholder using IDs
1. Have a button for each input that will change the text in the corresponding placeholder.

#### Update _all_ with a single button click

1. Select all inputs _and_ our placeholders using the method `querySelectorAll()`
   <https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelectorAll>
   * __HINT:__ Using classes and/or element selectors will help here
1. Use a `forEach` loop to create an array of values for our replacement words
1. Use a `forEach` loop to update the `innerHTML` of each placeholder
   * __HINT:__ You'll want to use the same `index` to update each entry in the _placeholder_ array with the corresponding _input value_ (aka `input.value`). The `forEach()` method takes `index` as an agrgument, which will return the index of a given item in the loop.

--

#### BONUS

* The `querySelectorAll()` method returns a `NodeList`, which is _like_ an array, but technically is __not__ an array. It has its own `forEach()` method, that behaves like the `Array.prototype.forEach()` method. <br/>(Don't worry too much about prototypes yet...we'll get to them)
* __YOUR CHALLENGE__: Convert the `NodeList` to a proper array. You can use `Array.isArray(value)` method to test if the result is an array (it returns a boolean).
  * __HINT:__ <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from>

#### DOUBLE BONUS

* Once you have an array, use the `map()` method in place of the `forEach()`. <br/><https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map>
