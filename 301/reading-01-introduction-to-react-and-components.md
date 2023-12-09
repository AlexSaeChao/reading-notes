# Introduction to React and Components

Component-based architecture allows for the creation of reusable, replaceable, and extensible software components that are independent, encapsulated, and not context-specific, providing advantages such as ease of deployment, reduced cost, ease of development, reusability, modification of technical complexity, reliability, system maintenance and evolution, and independent development.

## Component-Based Architecture

What is a “component”?

A component is like a plug and play software object, that should talk well to others in the same archtecture.

What are the characteristics of a component?

* Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

* Replaceable − Components may be freely substituted with other similar components.

* Not context specific − Components are designed to operate in different environments and contexts.

* Extensible − A component can be extended from existing components to provide new behavior.

* Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

* Independent − Components are designed to have minimal dependencies on other components.

What are the advantages of using component-based architecture?

* Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

* Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.

* Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

* Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

* Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.

* Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

* System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.

* Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

## What is Props and How to Use it in React

What is “props” short for?

Properties is long for "props"

How are props used in React?

Properties are being used for passing data from one component to another.

* Firstly, define an attribute and its value(data)
* Then pass it to child component(s) by using Props
* Finally, render the Props Data

What is the flow of props?

The flow is that the data with props are beiing passed in a uni-directional flow. Oneway from parent to child.

### Things I want to know more about

React seems to be a subset or short hand tooling of JavaScript for faster write times.

### References

[Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

[What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

[React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
[React Docs - Hello world](https://reactjs.org/docs/hello-world.html)
[React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
[React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)
[React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)