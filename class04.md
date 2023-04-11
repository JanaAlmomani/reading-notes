## What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

Class is a user-defined datatype that has its own data members and member functions whereas an object is an instance of class by which we can access the data members and member functions of the class

in class You can declare class only once Example: Car, but You can create more than one object using a class Example: Jaguar, BMW, Tesla, etc

## Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

 A recursive function is a function defined in terms of itself via self-referential expressions** will continue to call itself and repeat its behavior until some condition is met to return a result**
 - All recursive functions share a common structure made up of two parts: base case and recursive case
- Recursive function for calculating n! implemented in Python:
**Here, 1! is our base case, and it equals 1.**

 ```
def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:
        return n * factorial_recursive(n-1)
```
**Here, some best practices to follow when implementing a recursive function**
- Decide what the most basic output needs to be
- Determine what arguments to pass into the function
- A recursive algorithm must have a base case
 
## What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project. 

pytest fixtures are a way of providing data, test doubles, or state setup to your tests. Fixtures are functions that can return a wide range of values. Each test that depends on a fixture must explicitly accept that fixture as an argument.

Most importantly, they can provide data for testing and a wide range of value types when explicitly called by our testing software. You can use the mock data that fixtures create across multiple tests

