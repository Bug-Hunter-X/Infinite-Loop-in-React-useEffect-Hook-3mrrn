# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: creating an infinite loop within the `useEffect` hook.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

## Bug Description

The bug occurs because the `useEffect` hook attempts to update the `count` state within its own dependency array. This causes a continuous cycle of updates, resulting in an infinite loop.

## Solution

The solution removes the direct dependency of the `setCount` function on `count`. The updated state is now generated by an external function or event.