# React useEffect Bug: Unexpected Re-renders

This repository demonstrates a common React bug involving the `useEffect` hook.  The `useEffect` hook is intended to perform side effects after a component renders, but in this example, it runs on every render even though an empty dependency array is specified.

The bug arises from a misunderstanding of how `useEffect`'s dependency array works, coupled with potential issues in state updates.  The solution showcases the correct way to use `useEffect` to avoid unnecessary re-renders and improve performance.

## Bug:

The `bug.js` file shows the incorrect implementation.  The `useEffect` hook, despite having an empty dependency array (`[]`), runs on every render.  This is inefficient and could cause performance problems, especially in complex applications.