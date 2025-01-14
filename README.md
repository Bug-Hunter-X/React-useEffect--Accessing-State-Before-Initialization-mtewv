# React useEffect: Accessing State Before Initialization

This repository demonstrates a common error in React when using the `useEffect` hook: accessing a state variable before it's initialized.  The problem arises because `useEffect` runs before the state is fully updated in the render phase. This example shows how to solve this issue, improving code reliability and preventing unexpected behavior.

## Bug Description
The `bug.js` file contains a component that attempts to log the value of a state variable (`count`) within a `useEffect` hook, *before* the component has rendered and the state has been initialized. This results in an undefined value being logged to the console.

## Solution
The `bugSolution.js` file corrects this by ensuring that `count` is properly accessed after the component has successfully rendered. This fix ensures that the state is properly initialized before it is accessed.

## How to Run
1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install`.
4. Run `npm start`.
