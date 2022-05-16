## Context API - Behaviors

 to implement Context API and the React Hook useContext() in our  React project we need to know the followwing :
 - The Context API is a React structure that allows you to share specific data from all levels of your application and aids in solving prop-drilling.
 - React Hooks are functions that serve as a modular replacement for state and lifecycle methods written in functional components.
 - The useContext() method is an alternative to prop-drilling through the component tree and creates an internal global state to pass data.
 - 
React offers the createContext() method to assist in passing data as a prop.you can apply the .Provider component to your context in another file. The Provider
component enables the data in your context throughout your entire application. 

### Handling the useContext() Method
The useContext() method accepts a context within a functional component, and works with a .Provider and .Consumer component in one call. 
In your index.js file, import the useContext() method and the ColorContext function, and declare a functional component:

```ruby 
import React, { useContext } from "react";
import ColorContext from './ColorContext';

const MyComponent = () => {
  const colors = useContext(ColorContext);

  return <div style={{ backgroundColor: colors.blue }}>Hello World</div>;
};
```

The functional component MyComponent sets the value within your ColorContext as an argument to the useContext() method. 
Your return statement applies the background color in your application. When a change triggers, the useContext() method will subscribe
update with the latest context value. Compared to the Context API, the useContext() method allows you to share and pass data throughout your application
in fewer lines of code.

So ,The Context API in React provides you with built-in functions and components to avoid prop-drilling in your component tree. The React Hook useContext()
applies the same functionality in a streamlined, functional component body in one call.
