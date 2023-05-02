- **_What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method._**

dunder methods are methods that allow instances of a class to interact with the built-in functions and operators of the language. The word “dunder” comes from “double underscore”, because the names of dunder methods start and end with two underscores, for example __str__ or __add__ 

```
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def __str__(self):
        return f"{self.name} is {self.age} years old"
```

- **_Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation._**

The Python statistics module includes functions for computing fundamental statistical aspects of numeric data such as mean, median, mode, standard deviation, and variance. These routines can be used to do statistical calculations on a collection of data.

```
import statistics

data = [2, 3, 4, 5, 6, 7, 8, 9, 10]

mean = statistics.mean(data)

print(mean)  # Output: 6.0

```