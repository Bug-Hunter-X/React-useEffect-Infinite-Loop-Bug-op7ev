# React useEffect Infinite Loop Bug

This repository demonstrates a subtle bug involving the `useEffect` hook in React that can lead to an infinite rendering loop. The bug arises from a missing dependency in the `useEffect` hook's dependency array.  The solution shows how to correctly manage dependencies to prevent this issue.  The bug is subtle and can be easily overlooked, especially in larger components.

## Bug Description
The `useEffect` hook is designed to perform side effects after component renders. If the component re-renders repeatedly due to changing states, then the effects run in a loop unless properly managed with its dependency array.