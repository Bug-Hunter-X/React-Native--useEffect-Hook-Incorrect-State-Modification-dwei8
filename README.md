# React Native: useEffect Hook Incorrect State Modification

This repository demonstrates a common error encountered when using the `useEffect` hook in React Native: attempting to modify state directly within the effect callback, outside of a state update function.  This can lead to unpredictable behavior and application crashes.

## The Problem

The provided `bug.js` file showcases the incorrect implementation, where the `setState` function is called directly from inside the `useEffect` callback to update the state from fetched data.

## The Solution

The `bugSolution.js` file demonstrates the correct approach.  It uses the `useState` hook and updates the state using the `setState` function provided by the hook. This ensures that React is able to efficiently update the component's UI and handle potential re-renders.