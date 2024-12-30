# Express.js JSON Body Parsing Error with Empty or Invalid JSON

This repository demonstrates a common issue in Express.js applications where the `express.json()` middleware fails to parse empty or invalid JSON request bodies.  The server does not handle the error appropriately and continues execution, potentially leading to unexpected behavior.

## Bug

The `bug.js` file contains an Express.js server that attempts to parse JSON request bodies using `express.json()`. When an empty or invalid JSON request is sent, the server logs an empty object instead of returning a proper error response.

## Solution

The `bugSolution.js` file shows a corrected version of the server. It uses error handling middleware to catch and respond to JSON parsing errors effectively.  The server now gracefully handles these scenarios, returning appropriate error responses to the client.