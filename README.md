# React Router Dom v6 Unexpected Route Matching

This repository demonstrates an unexpected behavior in React Router Dom v6 related to route matching with nested routes and wildcard parameters.  The issue arises when a route with a wildcard parameter (`*`) is defined, causing it to unexpectedly match even when a more specific route should take precedence.

## Steps to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to `/contact/details`.  You'll notice that the Contact component renders, rather than a 404 error, even though no route explicitly defines that path. 

## Solution
The solution involves modifying the route definitions to prevent the unintended matching, ensuring correct route resolution.  See the `bugSolution.js` file for the corrected code. 