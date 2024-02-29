# Reading Notes

## React 3

What is React Context, and how does it help in managing state and data sharing in a React application?

React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

In other words, React context allows us to share data (state) across our components more easily.

Using context, you can effectively manage state and share data across your React application without having to resort to prop drilling (passing props through multiple layers of components), which can make your code cleaner and more maintainable. However, it's important to use context judiciously and avoid overusing it for all state management needs, as it can lead to complex and hard-to-understand code if used excessively.

Explain the useContext Hook and how it can be used to access data from a React Context within a functional component.

Instead of using render props, we can pass the entire context object to React.useContext() to consume context at the top of our component.

Here is the example above using the useContext hook:

```python

import React from 'react';

export const UserContext = React.createContext();

export default function App() {
  return (
    <UserContext.Provider value="Reed">
      <User />
    </UserContext.Provider>
  )
}

function User() {
  const value = React.useContext(UserContext);  
    
  return <h1>{value}</h1>;
}

```

The benefit of the useContext hook is that it makes our components more concise and allows us to create our own custom hooks.

You can either use the consumer component directly or the useContext hook, depending on which pattern you prefer.

Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application.

## Resouces

[React Context for Beginners](https://www.freecodecamp.org/news/react-context-for-beginners/#what-is-the-usecontext-hook)

[Chatgpt](https://chat.openai.com/)

[Why I’m Using Next.js in 2020](https://www.youtube.com/watch?v=rtgbaKBhdkk)

[Learn useContext In 13 Minutes](https://www.youtube.com/watch?v=5LrDIWkK_Bc)