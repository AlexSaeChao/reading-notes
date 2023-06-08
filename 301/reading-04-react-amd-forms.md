# React and Forms

What is a 'Controlled Component'?

When you have a form with input fields and text boxes, HTML can usually manage their own content based on what the user types or selects. In React, instead of letting the form elements handle their state, React likes to keep track of the data in a central space called state. Using things like the method `setState()`, when React manages the form's content and behavior this way, it is called a controlled component.

Should we wait to store the user's responses from the form into state when they submit the form, or should we update the state with their responses as soon as they enter them? Why?

We should update them as soon as they are entered. This allows you to show live updates and provide suggestions based on the user's input. It also provides data persistence if the user leaves the page and comes back to it later.

How do we target what the user is entering if we have an event handler on an input field?

`event.target.value`

# The Conditional (Ternary) Operator Explained

Why would we use a ternary operator?

Also known as the conditional operator, they are written in a concise way using concise syntax. It's a bit more readable and straightforward.

Rewrite the following statement using a ternary operator:

Example:

``` javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Refactored:

``` javascript
console.log(x === y ? true : false);
```

### Things I want to know more about

Can the ternary operator do more in it's form than the original way we learned conditional operators?
