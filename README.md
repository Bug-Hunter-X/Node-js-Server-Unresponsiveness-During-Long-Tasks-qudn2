# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js where long-running operations in request handlers can cause the server to become unresponsive.  The `server.js` file shows the problematic code, while `serverSolution.js` provides a solution using asynchronous operations.

## Problem

Node.js is single-threaded. When a request handler performs a long-running task, it blocks the event loop, preventing the server from processing other requests.  This leads to unresponsiveness and potentially crashes.