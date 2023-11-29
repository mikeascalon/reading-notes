# Reading Notes

## Passing Functions as Props

What does .map() return?

Returns an array of React elements that can be rendered in the component's JSX.

If I want to loop through an array and display each value in JSX, how do I do that in React?

You can use .map() in the context of React, it is typically used to transform each element of an array into a corresponding React element.

Each list item needs a unique ____.

key prop

What is the purpose of a key?

It serves as a special attribute that helps React identify and keep track of individual elements in a list or a set of sibling elements. I

## The Spread Operator

What is the spread operator?

Use is to pass props or state down to child components

List 4 things that the spread operator can do.

1. Copying Arrays

2. Merging Arrays

3. Copying Objects:

4. Passing Props in React

Give an example of using the spread operator to combine two arrays.

```javascript
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];

const combinedArray = [...array1, ...array2];

```

Give an example of using the spread operator to add a new item to an array.

```javascript
const originalArray = [1, 2, 3];
const newItem = 4;

const newArrayWithNewItem = [...originalArray, newItem];


```

Give an example of using the spread operator to combine two objects into one.

```javascript
const object1 = { key1: 'value1', key2: 'value2' };
const object2 = { key3: 'value3', key4: 'value4' };

const combinedObject = { ...object1, ...object2 };

```

## How to Pass Functions Between Components

In the video, what is the first step that the developer does to pass functions between components?

you need to pass it as a prop

In your own words, what does the handleClick function do?

it is lke a eventlistner for the button

How can you pass a method from a parent component into a child component?

You just need to pass the function as a code.

How does the child component invoke a method that was passed to it from a parent component?

You will nee a callback funtion on the child and invoke the callback from the parent

### Resources

[React Docs - lists and keys](https://canvas.instructure.com/courses/8071521/discussion_topics/20114872?module_item_id=96643319)

[Spread syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

ChatGPT
