# Reading Notes

## React lifecycle

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

* Render will happen first

What is the very first thing to happen in the lifecycle of React?

* initialization of the constructor

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

1. constructor

1. Render

1. componentDidMount

1. React Updates

1. componentWillUnmount




What does componentDidMount do?

* This method is called just before the component is removed from the DOM. It is used for cleanup tasks such as cancelling network requests or cleaning up subscriptions to prevent memory leaks.


## React State Vs Props

What types of things can you pass in the props?

1. Primitive Data Types

1. JavaScript Expressions

1. Functions

1. Objects

1. Arrays

1. Components

1. Callback Functions

1. Children (JSX Markup)

What is the big difference between props and state?

* Props (Properties): Data that is passed into a component from its parent. Props are immutable and are set by the parent component.

* State: Data that is managed within a component and can be changed by that component. State is internal and specific to the component that owns it.



When do we re-render our application?

It occurs when the component's state or props change.

What are some examples of things that we could store in state?

* State Changes

* Props Changes

* Force Re-render


### Resources

[Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)


[ChatGPT]()
