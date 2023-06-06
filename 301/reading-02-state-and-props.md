# State and Props

The React lifecycle starts with the mounting phase, where the constructor is called first. The render method is then invoked to generate the initial UI. After that, React Updates may occur, triggering a re-render if there are changes in the state. Finally, the componentDidMount method is called, allowing you to perform any necessary setup, such as fetching data or initializing the DOM.

Props are like arguments passed into a component from outside, allowing you to customize its behavior. On the other hand, state is managed internally within a component and represents its mutable data. When changes occur in the state, the application should be re-rendered to reflect the updated UI. Examples of things that can be stored in state include counters, user input data, or any dynamic values that require the application to react and update accordingly.

## React lifecycle

Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?

Based on the diagram the render happens first before the 'componentDidMount'

What is the very first thing to happen in the lifecycle of React?

Mounting through a constructor is the first thing that happens in the lifecycle of React.

Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`.

1. `constructor`
2. `render`
3. `React Updates`
4. `componentDidMount`
5. `componentWillUnmount`

What does `componentDidMount` do?

This is a method is called or invoked right after a component is mounted. Here is where you can load anthing using a network request or initailize the DOM

## React State Vs Props

What types of things can you pass in the props?

Props is like arguements to a function, what you want the function to work with. You can pass things like a title and subtitle for some DOM manipulation.

What is the big difference between props and state?

* Props you pass into a component and is handled outside that component

* State is handle inside that component and is handled inside that component.

When do we re-render our application?

When we add changes to a state we should re-render our application

What are some examples of things that we could store in state?

A counter or any data from user input. Really any thing that may have its values changed to update and re-render your app based on what the user has done.

## Things I want to know more about

Are there any other life cycle methods that are commonly used in React?

References:

[ChatGPT](https://chat.openai.com/?model=text-davinci-002-render-sha) used for summary.

[React Lifecycle Reading](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

[React State Vs Props Video](https://www.youtube.com/watch?v=IYvD9oBCuJI)
