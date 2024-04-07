Arithmetic Express API Documentation
------------------------------------

The Arithmetic Express API provides endpoints for performing basic arithmetic operations: addition, subtraction, multiplication, and division. These operations can be executed by sending HTTP requests to specific endpoints.

Base URL
--------
http://localhost:3000

Replace localhost with your server's hostname or IP address and 3000 with the port your server is listening on.

Endpoints
---------

Addition
--------
Endpoint: GET /add

Parameters:
- num1: The first number (required).
- num2: The second number (required).

Example:
Request: GET /add?num1=5&num2=3
Response:
{
  "result": 8
}

Subtraction
-----------
Endpoint: GET /sub

Parameters:
- num1: The first number (required).
- num2: The second number (required).

Example:
Request: GET /sub?num1=5&num2=3
Response:
{
  "result": 2
}

Multiplication
--------------
Endpoint: GET /multi

Parameters:
- num1: The first number (required).
- num2: The second number (required).

Example:
Request: GET /multi?num1=5&num2=3
Response:
{
  "result": 15
}

Division
--------
Endpoint: GET /divide

Parameters:
- num1: The first number (required).
- num2: The second number (required).

Example:
Request: GET /divide?num1=10&num2=2
Response:
{
  "result": 5
}

Error Handling
--------------
- If the input parameters are not valid numbers, the API returns a 400 Bad Request error with a JSON response indicating the error.
- If attempting to divide by zero, the API returns a 400 Bad Request error with a JSON response indicating the error.
