# React setInterval Memory Leak

This repository demonstrates a common bug in React applications involving the improper use of `setInterval` within the `useEffect` hook, leading to a memory leak.  The `bug.js` file contains the faulty code, while `bugSolution.js` provides the corrected version.

The problem arises from the absence of a cleanup function in the `useEffect` hook.  Without a cleanup function, the interval continues to run even after the component unmounts, resulting in memory leaks and performance issues. This example showcases how to properly use `setInterval` with a cleanup function to avoid this common pitfall.