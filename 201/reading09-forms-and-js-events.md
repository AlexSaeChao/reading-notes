# Forms and JS Events

## HTML Forms

Why are forms so important in web development?
They provide a way for the user to interact with the page. Forms can collect data and allow the user to control the UI.

When designing a form, what are some key things to keep in mind when it comes to user experience?

When designing a form, ask for the data you absolutely need.

Scannability and readability are important. Using single columns as well helps the scannability as well.

List 5 form elements and explain their importance.

* input - used to take input from user
* text area - multi-line input from user
* select - used in drop-down list, usually the first value in the select element is automatically selected until user input is taken
* button - a clickable button, like a sumbit button for user input
* label - useful for screen readers and can tick the check box when the user clicks the text to toggle

## JS Events

How would you describe events to a non-technical friend?

When programming you can think of events like reactionary actions taken when the user does something like click a button, hover over items/content. and thing the user can do and the browser does something else due to the action. Events doesn't actually have to be the from the user, it could be because something errored out when a page is loaded or a form is trying to be submitted.

When using the addEventListener() method, what 2 arguments will you need to provide?
The action the addEventListener is looking for and the function you are wanting it to take when the listener has heard the event occured

Describe the event object. Why is the target within the event object useful?

event objects are created when an event has occured and gives information about the event. the target within the event object is useful because it refers what just happened, the button being clicked or a submittion of a specific form. It helps identify  the which the element was interacted with.

What is the difference between event bubbling and event capturing?

Bubbling up is when an event occurs in a nested element but is shown in it's parents elements, this is so that you don't have to attached event listeners to each of the child elements. While event capturing is when the event is triggered and passed down into the nested target element.

## This I want to know more about

When using a text area element are there limits to the characters used or is that defined by the person writing it?
Are there different langauge inputs and how is it displayed for the server/person looking at the submission form?

## Other Notes

Types:
* click
* submit
* keypress
* hover
* mouseover
* page load

### Javascript Code: Event Listener

- Target an HTML element to "listen" to
- type of event listed as a string
- event handlet // callback function -> a functinog that is passed in another function as an arguement (not invoked)
- we dont invoke the call back, the event listener method will do something for us when it hears the event.


```javascript

let button = document.querySelector('button');

button.addEventListener('click', handleClick) // method to listen to an HTML element

```

### Javascript - code part 2: Event Handler - callback function

``` javascript
function handleClick(){
  console.log('this button was clicked..')
}
```

