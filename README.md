# Unhandled Exception in Asynchronous Node.js Callback

This repository demonstrates a common error in Node.js: unhandled exceptions within asynchronous callbacks.  The `bug.js` file shows a server that may throw an error in its asynchronous response handling. The `bugSolution.js` file provides a solution that includes proper error handling.

## Problem

Asynchronous operations are common in Node.js, often utilizing callbacks or promises. If an error occurs within these asynchronous operations and isn't properly handled, it can lead to the application crashing unexpectedly.

## Solution

The solution involves using `try...catch` blocks to handle potential errors or using async/await with a `try...catch` block for more structured error handling.