# Scala Exception Handling in Class Setter

This example showcases a potential issue and its solution related to exception handling within a Scala class setter method. The initial implementation throws an `IllegalArgumentException` if a negative age is provided.  While functional, in a more robust system this might require more sophisticated error handling, such as logging, alternative return values or using a custom exception type. The solution shows improvements using Try and Either for advanced error management.

## Bug
The original code throws an `IllegalArgumentException` if a negative age is attempted which, while correct, could be improved upon by incorporating more robust error handling.

## Solution
The improved code handles the potential exception and offers a method that uses Either to return a result and an error, giving more control to the caller on how to deal with the invalid age.