# Unnecessary Re-renders in React's useEffect Hook

This repository demonstrates a common issue in React applications where the `useEffect` hook runs on every render, leading to unnecessary computations and potential performance problems.  The solution shows how to optimize the `useEffect` hook using dependencies to control its execution.

## Bug Description:

The `useEffect` hook in the provided `bug.js` file lacks the correct dependency array, causing it to execute on every render.  This leads to the `console.log` statement being called unnecessarily, which can be especially detrimental with expensive operations.

## Solution:

The `bugSolution.js` file presents the corrected `useEffect` hook.  By including `[count]` as the dependency array, the effect only executes when the value of `count` changes. This prevents unnecessary re-renders and optimizes performance.
