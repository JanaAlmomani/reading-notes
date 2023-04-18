## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

There are two types of variables: global variables and local variables. The scope of global variables is the entire program whereas the scope of local variable is limited to the function where it is defined.

Example: 

def func():
   x = "Python"
   s = "test"
   print(x)
   print(s)
   s = "Tutorialspoint"
   print(s)
func()
print(x) 

In above program- x is a local variable whereas **s is a global variable**, we can access the local variable only within the function it is defined (func() above) and trying to call local variable outside its scope(func()) will through an Error as shown below 

However, we can call global variable anywhere in the program including functions (func()) defined in the program.

## How do the global and nonlocal keywords work in Python, and in what situations might you use them?
The main difference is that Global is used to access and modify global variables from within a function, while nonlocal is used to access and modify variables from the nearest enclosing scope that is not global.

## What is nonlocal keyword in Python?
After global and local variables, we have Non-local variables where non-local means “neither local nor global”. The nonlocal is a keyword in python that is used to declare any variable as not local but instead comes from the nearest enclosing scope that is not global.
