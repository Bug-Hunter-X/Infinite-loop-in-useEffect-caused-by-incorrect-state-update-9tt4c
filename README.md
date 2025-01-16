# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by incorrect usage of the `useEffect` hook.

## Bug Description
The `bug.js` file contains a component that uses the `useEffect` hook to update its state. However, the state update is done without specifying any dependencies, resulting in an infinite loop.

## Solution
The `bugSolution.js` file demonstrates the corrected code.  The dependency array is updated to include `count`, so the effect only runs when the `count` variable changes, preventing the infinite loop.