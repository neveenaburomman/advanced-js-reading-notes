## hook 

A Hook is a special function that lets you “hook into” React features.
For example, useState is a Hook that lets you add React state to function components. 

## What is the use of useState () in Hook?

useState is a Hook (function) that allows you to have state variables in functional components. You pass the initial state to this function and it returns a 
variable with the current state value (not necessarily the initial state) and another function to update this value.

## What does useState Hook returns?

The useState hook is a special function that takes the initial state as an argument and returns an array of two entries. Syntax: The first element is the initial 
state and the second one is a function that is used for updating the state.

## What is useState() in React ?

The useState() is a Hook that allows you to have state variables in functional components. React has two types of components, one is class components 
which are ES6 classes that extend from React and the other is functional components. Class components a Component and can have state and lifecycle methods:
class Message extends React.
The useState hook is a special function that takes the initial state as an argument and returns an array of two entries. 

Syntax: The first element is the initial state and the second one is a function that is used for updating the state.

==>> const [state, setState] = useState(initialstate

We can also pass a function as an argument if the initial state has to be computed. And the value returned by the function will be used as the initial state.

 ==>> const [sum, setsum] = useState(function generateRandomInteger(){5+7);})
The above function is oneline function which computes the sum of two numbers and will be set as the initial state.

Importing: To use useState you need to import useState from react as shown below:

==>> import React, { useState } from "react"
