# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by modifying the state variable within the `useEffect`'s dependency array.

## Description
The `bug.js` file contains a component that attempts to increment a state variable (`count`) within its `useEffect` hook. Since `count` is included in the dependency array, the effect runs infinitely, leading to performance issues and potential crashes.  The solution avoids the infinite loop by properly managing state updates.