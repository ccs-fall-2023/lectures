# Week 4 - Day 2

## Hour 1

### Show'n'Tell'n'Debug

* Review/debug the Github Users and Issues exercises

## Hours 2 - 3

### Clear it out

* Walkthrough clearing `form` elements and `elements`;

### Welcome to `Class`

* Presentation: [JavaScript Prototypes](https://docs.google.com/presentation/d/1o_7-TJMjTDkLj7awAkdyP7hThlV-rgay_d_TJi_oMz0/edit?usp=sharing)

### You down with OOP?

#### Classes

* **Classes:** Classes provide a blueprint for creating objects. You can define properties and methods within a class, and then you can create instances (objects) based on that class. This is a fundamental concept in OOP called "class-based inheritance."
* **Objects:** You can create multiple objects from the same class, each with its own set of properties and behaviors.
* **Encapsulation:** Classes allow you to encapsulate data (properties) and behavior (methods).
* **Inheritance:**CYou can create a subclass that inherits properties and methods from a parent class.

#### JavaScript and Classes...it's complicated

* **Prototypal Inheritance**: JavaScript is often described as a "prototypal" language because objects can inherit properties and methods directly from other objects. Every object in JavaScript has an associated prototype object, and if a property or method is not found on the object itself, JavaScript will look up the prototype chain to find it. This is often referred to as "prototypal inheritance."
* **Classes in ES6:** The introduction of the `Class` keyword in ES6 provides a syntax that resembles traditional class-based inheritance found in languages like Java or Python. However, under the hood, JavaScript classes still use prototypes. When you create a class and instantiate objects from it, JavaScript sets up a prototype chain for you automatically.
*** Objects and Instances:** In JavaScript, objects can be created in various ways, including literal object notation, constructor functions, and ES6 classes. Instances of objects can be created using the new keyword. These instances inherit properties and methods from their prototype, whether it's a prototype object created explicitly or the one associated with a class.

## Recommend Reading

* [Master the JavaScript Interview: What’s the Difference Between Class & Prototypal Inheritance?](https://medium.com/javascript-scene/master-the-javascript-interview-what-s-the-difference-between-class-prototypal-inheritance-e4cd0a7562e9)