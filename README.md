# Unhandled Error in Express.js Route Handler
This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input or unexpected situations.  Specifically, the example shows a route that retrieves a user by ID but lacks error handling if the user is not found. This can lead to unhandled exceptions or unexpected behavior.

## Bug
The `bug.js` file contains the buggy code. The `/users/:id` route attempts to find a user with the given ID. If no user with that ID exists, it doesn't gracefully handle the situation, potentially causing the application to crash or behave unexpectedly. 

## Solution
The `bugSolution.js` file shows the corrected code. It includes explicit error handling to check if a user is found. If not, it returns a 404 Not Found response with an appropriate message.