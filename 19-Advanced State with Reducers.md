## useReducer Hook

The useReducer is a hook I use sometimes to manage the state of the application. It is very similar to the useState hook, just more complex.
It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the
reducers in Redux.

## useReducer
```ruby
const [state, dispatch] = useReducer(reducer, initialArg, init);

```

An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.
useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the 
previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

Here’s the counter example from the useState section, rewritten to use a reducer:
```ruby
const initialState = {count: 0};

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return {count: state.count + 1};
    case 'decrement':
      return {count: state.count - 1};
    default:
      throw new Error();
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({type: 'decrement'})}>-</button>
      <button onClick={() => dispatch({type: 'increment'})}>+</button>
    </>
  );
}
```
## Where can I use useReducer Hook?
The useReducer Hook is the better alternative to the useState hook and is generally more preferred over the useState hook when you have complex state-building
logic or when the next state value depends upon its previous value or when the components are needed to be optimized.
