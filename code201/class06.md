# Reading Notes

## Problem Domain, Objects, and the DOM

## JavaScript Objects Basic

1.How would you describe an object to a non-technical friend you grew up with?

* Imagine a object is like a bus. Inside you the  several couples that are called properties. One of the couple  will be the key and the other is the value .

2.What are some advantages to creating object literals?

* Object literals use a simple and straightforward syntax that is easy to read and write

3.How do objects differ from arrays?

* Objects: Objects are collections of key-value pairs and  Arrays are ordered, integer-indexed collections of values.

4.Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

* You would use bracket notation to access an object's property when the property name contains special characters, spaces, or when it is a dynamically generated string.

5.Evaluate the code below. What does the term this refer to and what is the advantage to using this?

```javascript
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

```

* this refers to the current object, which, in this context, is the dog object. The this keyword is a reference to the object that the method is called on.

## Introduction to the DOM

What is the DOM?

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content

Briefly describe the relationship between the DOM and JavaScript.

JavaScript is used to manipulate and control the DOM, enabling web developers to create interactive and responsive web applications. This combination allows for dynamic, client-side functionality and is a fundamental aspect of modern web development.

## Things I want to know more about

DOM
Resources

[JavaScript oobject basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

[Introduction to the DOM](https://canvas.instructure.com/courses/7890511/discussion_topics/19821041?module_item_id=95034386)
