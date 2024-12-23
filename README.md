# React useEffect Hook Bug

This repository demonstrates a common bug in React's `useEffect` hook where the dependency array is incorrectly specified, preventing the effect from running when expected.

## Bug Description

The `useEffect` hook in `bug.js` is intended to log a message when the `count` state variable is greater than 0. However, due to an incorrect dependency array, the effect only runs once on component mount, even though the `count` state changes.

## Solution

The solution in `bugSolution.js` correctly specifies the `count` variable in the dependency array. This ensures that the effect runs whenever the `count` state variable changes.