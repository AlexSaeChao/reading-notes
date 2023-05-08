# Readings: Problem Domain, Objects, and the DOM

## JavaScript Object Basics

1. How would you describe an object to a non-technical friend you grew up with?

  * JS objects are like cars. Each cars may have characterics that help identify what the car is like make, model, paint, year.

2. What are some advantages to creating object literals?

  * they are easier to refer to and can be used to create complex data structures like arrays

3. How do objects differ from arrays?

  * Arrays are stored values of data while objects are used to store collections of properties or key-value pairs.

4. Give an example for when you would need to use bracket notation to access an object’s property
instead of dot notation.

  * Bracket notation is used instead of a dot notion is when the property name is stored in a varible.

5. Evaluate the code below. What does the term this refer to and what is the advantage to using 
this?

```
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

  *  `this` is redering to the const of `dog`. `this.name` refering to Spot and `this.age refers to the dog's age.

## Things I want to know more about

Why is makes objects so modular for coding?