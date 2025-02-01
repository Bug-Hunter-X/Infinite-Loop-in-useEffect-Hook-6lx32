# Infinite Loop in useEffect Hook

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by improperly managing dependencies.

The `bug.js` file contains a component that attempts to increment a state variable within the `useEffect` hook, causing an infinite loop because the dependency array `[count]` triggers the effect every time `count` changes (which is immediately after incrementing it). 

The `bugSolution.js` file provides the corrected version, showcasing how to avoid this error and prevent unnecessary re-renders.