# Class 05 Reading Notes *(11/10/22)*

[*back*](../README.md)

## React Docs - Thinking in React

1. a component should only do one thing
2. renders UI but has no interactivity
3. add interactivity through state
4.  
    1. Is it passed in from a parent via props? If so, it  probably isn’t state.
    2. Does it remain unchanged over time? If so, it probably isn’t state.
    3. Can you compute it based on any other state or props in your component? If so, it isn’t state.
5. For each piece of state in your application:
    1. Identify every component that renders something based on that state.
    2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
    3. Either the common owner or another component higher up in the hierarchy should own the state.
    4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

1. Functions that operate on other functions, either by taking them as arguments or by returning them
2. returns a number greater then 10
3. map iterates through each item on an array and changes it.
