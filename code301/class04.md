# Reading Notes

## How to use Forms in React

What is a ‘Controlled Component’?

A "controlled component" in React refers to a form element, such as an input or textarea, whose value is controlled by React state.

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

You update the state on input but perform comprehensive validation and additional processing on form submission. This way, you can provide real-time feedback to users while still ensuring that the final data meets all requirements.

How do we target what the user is entering if we have an event handler on an input field?

you can target what the user is entering by accessing the event object that is automatically passed to your event handler function. The event object contains information about the event, including the current value of the input field.

Why would we use a ternary operator?

A ternary operator, often referred to as the conditional operator, is a concise way to write a simple if...else statement in a single line.

Rewrite the following statement using a ternary statement:

```javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Ternary statement

```javascript
console.log( x === y ? true : false)
```

### Resourses

[How to use Forms in React](https://www.robinwieruch.de/react-form/)

[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

[ChatGPT](https://chat.openai.com/)
