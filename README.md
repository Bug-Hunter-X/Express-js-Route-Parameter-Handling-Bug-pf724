# Express.js Route Parameter Handling Bug

This repository demonstrates a common bug in Express.js route parameter handling and provides a solution.

## Bug Description

The bug occurs when a route parameter is not properly validated before being used. In this case, the route `/users/:id` expects an integer `id`. If the request is made without the `id` parameter or with a non-integer value, unexpected behavior can result. 
The original code lacks input validation for `req.params.id`, making it vulnerable to errors.

## Solution

The solution involves adding input validation and error handling to ensure the parameter `id` is a valid integer.  This prevents crashes and provides more informative error responses to the client.