## Redux
redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and 
native environments and are easy to test. While it's mostly used as a state management tool with React, you can use it with any other
JavaScript framework or library.

## How does Redux manage state
Redux operates according to a few concepts. First, the store is a single object with fields for each selection of data. You update
the data by dispatching an action that says how the data should change. You then interpret actions and update the data using reducers.

Here's a basic example of a Redux store. It's for a simple counter application that can increment and decrement the count on button clicks,
and the state of the counter is managed and handled by Redux:
```ruby
import { createStore } from 'redux'

const initialState = {
  counter: 0,
}

const reducer = (state = initialState, action) => { // Reducer function
  switch (action.type) {
    case 'INCREMENT':
      return { ...state, counter: state.counter + 1 }
    case 'DECREMENT':
      return { ...state, counter: state.counter - 1 }
    default:
      return state
  }
}

const store = createStore(reducer) // redux-store

export default store
```
## How Redux works
The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored
state without having to send down props from one component to another.
There are three building parts: actions, store, and reducers. Let’s briefly discuss what each of them does. This is important because they 
help you understand the benefits of Redux and how it’s to be used. We’ll be implementing a similar example to the login component above but this time in Redux.

There are three building parts: actions, store, and reducers. Let’s briefly discuss what each of them does. This is important because they help you understand the benefits of Redux and how it’s to be used. We’ll be implementing a similar example to the login component above but this time in Redux.
