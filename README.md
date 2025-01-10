# React 19 useEffect setInterval memory leak
This example demonstrates a common mistake when using `setInterval` within a React `useEffect` hook.  Forgetting to return a cleanup function leads to memory leaks as the interval continues even after the component unmounts.

The `bug.js` file shows the problematic code.  The solution, in `bugSolution.js`, demonstrates the correct usage with the cleanup function that clears the interval when the component unmounts.