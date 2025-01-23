# Express.js Error Handling Bug

This repository demonstrates a common error in Express.js applications: insufficient error handling in route handlers.

The `bug.js` file showcases a route that fetches user data from a database.  It lacks proper error handling for database errors and cases where a user is not found.  This results in generic 500 errors, providing little information to the user or developer.

The `bugSolution.js` file provides a corrected version with robust error handling, returning appropriate HTTP status codes (404 and 500) with informative error messages.