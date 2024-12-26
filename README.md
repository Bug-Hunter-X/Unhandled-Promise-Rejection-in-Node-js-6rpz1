# Unhandled Promise Rejection in Node.js

This repository demonstrates a common error in Node.js applications: unhandled promise rejections.  Unhandled promise rejections can lead to application crashes and unexpected behavior. This example shows how to identify and resolve this issue.

## Bug Description

The `bug.js` file contains a simple HTTP server. However, it lacks proper error handling for promises.  If an error occurs within an asynchronous operation (e.g., database interaction, network request), the promise will reject, causing the application to crash with an 'Unhandled promise rejection' error.

## Solution

The `bugSolution.js` file presents a corrected version of the code.  It includes a `.catch()` block to gracefully handle potential promise rejections, preventing the application from crashing.