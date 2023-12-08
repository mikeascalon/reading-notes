# Reading Notes

## Understanding the JavaScript Call Stack

What is a ‘call’?

is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom.

How many ‘calls’ can happen at once?

I think this depends on your computer and what ever your doing in the computer.

What does LIFO mean?

Last In, First Out,

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```javascript
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

What causes a Stack Overflow?

* A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

JavaScript error messages

What is a ‘reference error’?

* This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

What is a ‘syntax error’?

* this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

What is a ‘range error’?

type of error that occurs when a numeric variable or parameter is outside the permissible range.

What is a ‘type error’?

* is a type of error that occurs when a value is not of the expected type. This error is thrown when an operation is performed on a value that is not compatible with the operation's expected type.

What is a breakpoint?

* A breakpoint is a designated point in a program's source code where the execution of the program will pause temporarily for debugging purposes. When a breakpoint is set, it allows developers to inspect the program's state, including variable values, at that specific point in the code.

What does the word ‘debugger’ do in your code?

Debugging is the process of finding and resolving errors or unexpected behavior in a program, and a debugger is an essential tool for this purpose.

### Resourse

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

[JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

[ChatGPT](https://chat.openai.com/)
