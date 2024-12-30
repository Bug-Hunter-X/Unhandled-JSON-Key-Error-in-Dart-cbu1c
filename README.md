# Unhandled JSON Key Error in Dart

This repository demonstrates a common error in Dart when handling JSON responses:  accessing a key that doesn't exist in the JSON object.  The example showcases how this can lead to runtime exceptions and how to mitigate the issue using error handling and input validation.

## The Bug

The `bug.dart` file contains a function `fetchData` that fetches JSON data from an API.  The code then attempts to access a key (`'nonExistentKey'`) that may not be present in the JSON response. This causes a runtime error if the key is missing.

## The Solution

The `bugSolution.dart` file provides a corrected version of `fetchData`. It includes checks to ensure the key exists before accessing it, preventing the runtime error.  The solution uses a combination of null checks and conditional expressions to handle the possibility of a missing key gracefully.