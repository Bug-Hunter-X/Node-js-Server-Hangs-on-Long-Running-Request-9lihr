# Node.js Server Hang - Blocking the Event Loop

This repository demonstrates a common issue in Node.js where a long-running operation blocks the event loop, causing the server to become unresponsive to new requests.

The `server.js` file contains a simple HTTP server that simulates a long-running task using a busy-wait loop.  This blocks the event loop, preventing the server from handling other requests while the loop is executing.

The `serverSolution.js` file shows a solution using asynchronous operations and the `setTimeout` function to avoid blocking the event loop.