# PHP Silent Failure: Accessing Non-Existent Array Indices

This repository demonstrates a subtle bug in PHP related to accessing array elements using numeric indices that were not explicitly assigned.  This bug doesn't throw an error, instead it silently returns nothing, making it hard to debug. The `bug.php` file showcases the issue, and `bugSolution.php` provides a solution.

The issue is described in more detail in the `bug.php` file's comments.  The solution involves checking for the existence of the array key using `isset()` or `array_key_exists()` before accessing it.  Always explicitly define your array keys whenever possible to reduce unexpected behaviors and improve code clarity.