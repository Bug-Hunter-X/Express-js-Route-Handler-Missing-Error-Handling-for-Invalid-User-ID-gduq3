# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.  Specifically, the provided code lacks checks to ensure that a user ID parameter is a valid number before attempting to parse it. This can lead to unexpected behavior or crashes if a non-numeric ID is provided.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides a corrected version with robust error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express`
3. Run `node bug.js`
4. Send a request to `/users/abc` or `/users/123a`. Observe the error (crash or unexpected response).
5. Run `node bugSolution.js`. Send the same requests and compare the improved error handling.