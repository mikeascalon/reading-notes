# Reading Notes

## Thinking in React

What is the single responsibility principle and how does it apply to components?

* That is one of the SOLID principles of object-oriented design. It states that a class should have only one reason to change, meaning that a class should have only one responsibility or job. A component should ideally only do one thing

What does it mean to build a ‘static’ version of your application?

* This is like building the wireframe first before you add any interactive function.

Once you have a static application, what do you need to add?

* Find the minimal but complete representation of UI state

What are the three questions you can ask to determine if something is state?

* Identify every component that renders something based on that state.
* Find their closest common parent component—a component above them all in the hierarchy.
* Decide where the state should live

How can you identify where state needs to live?

* Often, you can put the state directly into their common parent.
* You can also put the state into some component above their common parent.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component.

## Higher-Order Functions

What is a “higher-order function”?

* Functions that operate on other functions, either by taking them as arguments or by returning them

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

```javascript
return m => m > n;
```

the function takes a parameter of m . then the function looks at if m is greater than n function runs true else it's false.

Explain how either map or reduce operates, with regards to higher-order functions.

it similar on that take a function as an argument.

### Resources

[Thinking in React](https://react.dev/learn/thinking-in-react)

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

[ChatGPT](https://chat.openai.com/)
