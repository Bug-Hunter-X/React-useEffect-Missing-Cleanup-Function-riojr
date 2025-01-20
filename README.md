# React useEffect Missing Cleanup Function

This repository demonstrates a common error in React applications: forgetting to include a cleanup function in the `useEffect` hook.  This can lead to memory leaks and unexpected behavior.

## Problem
The `bug.js` file contains a `MyComponent` that updates the document title whenever the count changes. However, it's missing a cleanup function which would reset the title when the component unmounts or when the `count` dependency changes.

## Solution
The `bugSolution.js` file provides a corrected version, including the cleanup function.  The cleanup function ensures that the title is always reset appropriately.

## How to run
1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install`.
4. Run `npm start`.

You can then compare the behavior of the buggy and corrected components.