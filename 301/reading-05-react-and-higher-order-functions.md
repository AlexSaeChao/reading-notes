# React and Higher-Order Functions

This section talks about SOPs behind components, static verision of your react app and what is a higher-order function.

## Thinking in React

What is the single responsibility principle and how does it apply to components?

A component ideally should only do one thing. if it ends up growing into more, it should be broken down even more.

What does it mean to build a ‘static’ version of your application?

Building a static verision of an app means to build or render the UI without the interactivity.

Once you have a static application, what do you need to add?

* ID where you need states to live
* adding callbacks in the parent component down to the child that needs it to update state.
* ID the minimal state needed for interactivity
* Add interactivity with state

What are the three questions you can ask to determine if something is state?

It isn't a state if:

1. Does it not change over time?
2. Is it passed in from a parent?
3. Can you compute it based on state or props 

How can you identify where state needs to live?

* Identify every component that renders something based on state
* Find a common owner component
* Determine if the common owner component should have the state
* If the common owner component doesn't work as the state manager

## Higher-Order Functions

What is a “higher-order function”?

Functions that operate on other functions, by taking them in as arguements or return them.

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

It looks like it is returning an arrow function which compares the arguement of `m` with the value of `n`

``` javascript
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```

Explain how either map or reduce operates, with regards to higher-order functions.

Map:
`map` functions work by iterating over each element of an array and apply a transformation function to that element.

Reduce:
`reduce` takes in an array, iterating over each element and takes in a combining function and a starting point as arguements.

### Things I want to know more about

TBD

### References

[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)
