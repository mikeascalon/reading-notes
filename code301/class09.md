# Reading Notes

## Functional Programming Concepts

What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

What is a pure function and how do we know if something is a pure function?

* It returns the same result if given the same arguments (it is also referred as deterministic)
* It does not cause any observable side effects

What are the benefits of a pure function?

the benefits of pure functions include determinism, no side effects, testability, referential transparency, support for parallelism, memoization, functional composition, and compatibility with immutability. Incorporating these principles can lead to more maintainable, readable, and robust code.

What is immutability?

Immutability is a programming concept that promotes the creation of objects whose state cannot be changed after they are created. This concept contributes to code simplicity, predictability, and thread safety, especially in the context of functional programming.

What is Referential transparency?

Referential transparency is a property of a function in which its output is solely determined by its input, and calling the function with the same input will always produce the same result. In other words, a referentially transparent function can be replaced with its result without affecting the behavior of the program.

What is a module?
What does the word ‘require’ do?
How do we bring another module into the file the we are working in?
What do we have to do to make a module available?

## Node JS Tutorial for Beginners #6

What is a module?

a module is a self-contained unit of code that encapsulates related functionality. Modules are used to organize code into separate and manageable units, promoting code reusability, maintainability, and readability. The term "module" is used in various programming languages, and its implementation might vary across languages.

What does the word ‘require’ do?

The require function is used to include and use external modules in a Node.js application. It is a way to import functionality from other JavaScript files or libraries.

How do we bring another module into the file the we are working in?

* Create a Module (e.g., myModule.js):

```javascript
// myModule.js
const greeting = 'Hello, ';

function greet(name) {
    return greeting + name;
}

module.exports = {
    greet,
};

```

* Use the Module in Another File (e.g., main.js):

```javascript
// main.js
const myModule = require('./myModule');

console.log(myModule.greet('John')); // Outputs: Hello, John
```

* In this example, the myModule.js file exports a function (greet), and in main.js, the require('./myModule') statement is used to import the module. Once imported, you can use the exported functionalities.

What do we have to do to make a module available?

1. Create the Module
1. Export the Module's Components
1. Import the Module Where Needed

## Resources

[Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

[ChatGPT](https://chat.openai.com/)
