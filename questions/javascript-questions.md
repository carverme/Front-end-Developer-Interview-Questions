# JS Questions:

* Explain event delegation
* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works
* What do you think of AMD vs CommonJS?
* Explain why the following doesn't work as an IIFE: `function foo(){ }();`.
  * What needs to be changed to properly make it an IIFE?

* What's the difference between a variable that is: `null`, `undefined` or undeclared?
- Null - the value null represents the intentional absence of any object value, a JS primitive value, not an identifier for the property of a global object, expresses a lack of identification, indicates that a variable points to no object.
- Undefined - represents the primitive value of undefined, a primitive JS type, a property of the global object, a variable in global scope.
A variable that has not been assigned a value is of type undefined.  A method or statement also returns undefined if the variable that is being evaluated does not have an assigned value.  A function returns undefined if a value was not returned.  Avoid using this as an identifier, or var name, outside of global scope.
- Undeclared - a variable that has been declared without "var" keyword.  Undeclared variables are created as global variable and they are configurable (ex. can be deleted).

[MDN Null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)
[MDN Undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)
[Medium.com on all three](https://medium.com/@rlynjb/js-interview-question-what-s-the-difference-between-a-variable-that-is-null-undefined-or-bf7233cef1c2)
[MDN Primitive](https://developer.mozilla.org/en-US/docs/Glossary/Primitive)
  * How would you go about checking for any of these states?
- For undeclared, we could turn on 'use strict' or use a 'try' and a 'catch.'
- Undefined is actually a value you can assign.
For ex:
`
"use strict";
var foo = undefined;

if (foo) {
  console.log("foo exists")
} else {
  console.log("foo doesn't exist")
}
`

* What is a closure, and how/why would you use one?
* Can you describe the main difference between a `forEach` loop and a `.map()` loop and why you would pick one versus the other?
* What's a typical use case for anonymous functions?
* How do you organize your code? (module pattern, classical inheritance?)
* What's the difference between host objects and native objects?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* What's the difference between feature detection, feature inference, and using the UA string?
* Explain Ajax in as much detail as possible.
* What are the advantages and disadvantages of using Ajax?
* Explain how JSONP works (and how it's not really Ajax).
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* Difference between window load event and document DOMContentLoaded event?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
* Why is it called a Ternary operator, what does the word "Ternary" indicate?
* What is `"use strict";`? what are the advantages and disadvantages to using it?
--Separates the hobbyists from the mid-level coders... research the 5 differences, etc.
* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`
* Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
* Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
* Explain what a single page app is and how to make one SEO-friendly.



* What is the extent of your experience with Promises and/or their polyfills?
* What are the pros and cons of using Promises instead of callbacks?
* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
* What tools and techniques do you use debugging JavaScript code?
* What language constructions do you use for iterating over object properties and array items?
* Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?
* Explain the difference between synchronous and asynchronous functions.
* What is event loop?
  * What is the difference between call stack and task queue?
* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`
* What are the differences between variables created using `let`, `var` or `const`?
* What are the differences between ES6 class and ES5 function constructors?
* Can you offer a use case for the new arrow `=>` function syntax? How does this new syntax differ from other functions?
* What advantage is there for using the arrow syntax for a method in a constructor?
* What is the definition of a higher-order function?
* Can you give an example for destructuring an object or an array?
* ES6 Template Literals offer a lot of flexibility in generating strings, can you give an example?
* Can you give an example of a curry function and why this syntax offers an advantage?
* What are the benefits of using `spread syntax` and how is it different from `rest syntax`?

* How can you share code between files?
--how we require in node, and export from one file to the next... similarly in react how we import, and export...
    (we can install modules, but once we install we must require them into the project... this is how we connect the js modules...)

* Why you might want to create static class members?
