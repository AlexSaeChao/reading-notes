# Page Summary

Functional programming focuses on functions and immutability, Node.js modules allow us to use code from separate files in our program.

## Functional Programming Concepts

What is functional programming?

Functional Programming is about writing code with the focus on functions, avoiding data changes, promoting predictablility and reusability.

What is a pure function and how do we know if something is a pure function?

pure functions are functions that, given the same inputs, always produces the  same output. it also doesn't modify any variables.

What are the benefits of a pure function?

Some benefits are they are predictable, they are easier to test, and because they don't rely on context outside of their inputs.

What is immutability?

this refers to a concept of not changing the data after it is created. it cannot be modified but if you want to modify it youu'd have to create a new copy with the desired changes.

What is Referential transparency?

A function is referentially transparent if the input can be replaced by its return value without affecting the overall program.

## Node JS Tutorial for Beginners #6 - Modules and require()

What is a module?

a module a seperate file that has a certain functionality that can called when needed to run its function.

What does the word ‘require’ do?

The word require links the module to an app that is trying to use it.

How do we bring another module into the file the we are working in?

``` javascript

const moduleName = require('modulePath');

```

What do we have to do to make a module available?

``` javascript
const myFunction = () => {
  // ...
};

module.exports = myFunction;
```

## Things I want to know more about
It seems the exporting  and require from ESM is really similar to the tradtional Node.js. What scenarios to use one over the other?

## References

[Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)
