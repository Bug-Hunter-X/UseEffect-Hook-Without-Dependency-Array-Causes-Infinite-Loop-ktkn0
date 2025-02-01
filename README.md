# React useEffect Hook Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The `useEffect` hook, without a dependency array, runs after every render, leading to an infinite render loop. This example shows the problem and its solution.

## Problem

The `MyComponent` in `bug.js` uses `useEffect` without a dependency array.  This causes the effect to run after every render, creating an infinite loop.  The console will continuously log 'Count changed:'.

## Solution

The solution, in `bugSolution.js`, adds a dependency array `[count]` to the `useEffect` hook. Now, the effect only runs when the `count` state variable changes.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npm start`.
5. Observe the behavior in the browser console and how it is fixed.