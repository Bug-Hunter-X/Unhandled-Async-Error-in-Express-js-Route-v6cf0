# Unhandled Async Error in Express.js Route

This repository demonstrates a common error in Express.js applications: unhandled exceptions within asynchronous route handlers.  When an asynchronous operation throws an error, and that error isn't properly caught, the server can crash unexpectedly.

## Bug Description
The `bug.js` file contains an Express.js server with a route that simulates an asynchronous operation.  Sometimes this operation succeeds, and other times it throws an error.  Because the error isn't handled, the server crashes when the error occurs. 

## Solution
The `bugSolution.js` file shows how to correctly handle such errors using `try...catch` blocks or middleware to gracefully handle exceptions and prevent server crashes. The solution provides more robust error handling.