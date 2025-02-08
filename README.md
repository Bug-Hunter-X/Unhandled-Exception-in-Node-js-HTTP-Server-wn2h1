# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js HTTP servers: failure to handle exceptions properly.  The provided code creates a simple HTTP server but lacks robust error handling.  This can lead to unexpected server crashes and disruptions.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides a corrected version with comprehensive error handling.

## Bug Description

The `bug.js` example lacks a `try...catch` block to handle potential errors within the request listener.  If an exception occurs during request processing, the server will crash without logging any information.  This makes debugging difficult and can result in service interruptions.

## Solution

The `bugSolution.js` file implements proper error handling using a `try...catch` block.  This ensures that exceptions are caught, logged appropriately, and the server remains operational, thereby improving the server's resilience and providing valuable debugging information.