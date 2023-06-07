# Passing Functions as Props

This reading talks about lists and keys, how to use spread operators and how to pass functions between components

## React Docs - lists and keys

What does .map() return?

.map() returns a new array with a function applied to each element of the original array.

If I want to loop through an array and display each value in JSX, how do I do that in React?

You would map out your array of numbers arrow it to a list of numbers. Then you use ReactDom to get element by ID and render the list there.

``` javascript
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((numbers) =>
  <li>{numbers}</li>
);

const root = ReactDOM.createRoot(document.getElementById('root')); 
root.render(<ul>{listItems}</ul>);
```

Each list item needs a unique `key`.

What is the purpose of a key?

Keys help React ID which which items have been modified, added, or removed. Keys should be nested withing the element inside the array to give the elements a stable identity.

## The Spread Operator

What is the spread operator?

The spread operator is passed through the parameters of a function to separate arguements from an array. `...` is passed

List 4 things that the spread operator can do.

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

Give an example of using the spread operator to combine two arrays.

``` javascript
let arr1 = [1, 2, 3];
let arr2 = [4, 5, 6];

let combArr = [...arr1, ...arr2];

console.log(combArr); 

// expected output [1, 2, 3, 4, 5, 6]
```

Give an example of using the spread operator to add a new item to an array.

``` javascript
let arr1 = [1, 2, 3];
let newItem = 4;

let addItemArr = [...arr1, newItem];

console.log(addItemArr); 

// expected output [1, 2, 3, 4]
```

Give an example of using the spread operator to combine two objects into one.

``` javascript
let objectOne = { name: Adam, age: 27 };
let objectTwo = { hobby: Drawing, hasBike: true };

let combinedObj = [...objectOne, ...objectTwo];

console.log(combinedObj); 

// expected output { name: Adam, age: 27, hobby: Drawing, hasBike: true }
```

## How to Pass Functions Between Components

In the video, what is the first step that the developer does to pass functions between components?

He makes a function in the parent component to update the state then calling the function in the child component

In your own words, what does the increment function do?

The increment function takes in a person's name and then maps out the whole array, compares it and if it matches, increment the count property. Finally update the state of count.

How can you pass a method from a parent component into a child component?

You can pass a method from a parent component into a child component by including the child component within the parent component's JSX and pass the the method there, where the attribute's value is the method you want to pass.

How does the child component invoke a method that was passed to it from a parent component?

to invoke the method passed, you would attach the method to something like an event handler onclick.

### Things I want to know more about

### References

[List and Key - Reading](https://legacy.reactjs.org/docs/lists-and-keys.html)

[Spread Operator - Reading](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)