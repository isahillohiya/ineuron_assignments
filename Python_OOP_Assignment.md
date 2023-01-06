## Python OOP Assignment

<b> Q1. What is the purpose of Python's OOP? </b>
```
Object-oriented programming (OOP) is a programming is based on the concept of "objects", which can contain data and code that manipulates that data. The main purpose of OOP in Python is to provide a way to organize and structure your code in a logical and modular way, and to make it easier to reuse, modify, and maintain.
```

<b> Q2. Where does an inheritance search look for an attribute? </b>
```
 the attribute lookup mechanism works as follows:

 1. If the attribute is not found in the current class, Python will search for it in the base class or base classes of the current class. This search is performed recursively, starting with the base class immediately following the current class in the inheritance hierarchy and proceeding up the chain of base classes.

 2. If the attribute is not found in any of the base classes, Python will raise an AttributeError exception.
```

<b> Q3. How do you distinguish between a class object and an instance object? </b>
```
Class objects are defined using the class keyword, whereas instance objects are created by calling the class's constructor
```
```
class MyClass:
    def __init__(self):
        self.x = 1

# MyClass is a class object

obj = MyClass()

# obj is an instance object of the MyClass class

```
<b> Q4. What makes the first argument in a class’s method function special? </b>

```
the first argument of a method in a class is referred to as self. This argument is special because it is used to refer to the instance of the object.
```

<b> Q5. What is the purpose of the init method? </b>
```
The __init__ method (short for "initialize") is a special method in Python classes that is called when an instance of the class is created. It is used to initialize the attributes of the instance and to set them to their default values.
```

<b> Q6. What is the process for creating a class instance? </b>
```
 To create a class instance, You need to call the class variable as if it was a function.
```

<b> Q7. What is the process for creating a class? </b>
```
To create a class, you need to Define the class using the class keyword and a class name of your choice. Inside the class definition, you can define the attributes and methods of the class.

```

<b> Q8. How would you define the superclasses of a class? </b>
```
To define the superclasses of a class in Python, you can use the class keyword and the superclass name in parentheses when defining the class.

```

```
class MyClass(SuperClass1, SuperClass2, SuperClass3):
    def __init__(self):
        self.x = 1
```


<b> Q9. What is the relationship between classes and modules? </b>
```
In Python, a module is a file that contains a collection of related code, such as functions, classes, and variables. A module allows you to organize your code into logical units and to reuse it in other parts of your program.

Classes are a fundamental element in object-oriented programming (OOP), and they are often defined in modules. When you define a class in a module, you can use that class in any other code that imports the module. This allows you to create reusable, modular components that can be easily shared and reused in different parts of your program.
```

<b> Q10. How do you make instances and classes? </b>
```
To create a class, you need to Define the class using the class keyword and a class name of your choice. Inside the class definition, you can define the attributes and methods of the class.

To create a class instance, You need to call the class variable as if it was a function.
```

<b> Q11. Where and how should be class attributes created? </b>
```
In Python, you can create class attributes in the following ways:

- Inside the class definition: You can define class attributes directly inside the class definition by assigning a value to a variable name. These attributes will be shared by all instances of the class.
```

```
class MyClass:
    x = 1
    y = 2

obj1 = MyClass()

print(obj1.x)  # Output: 1
```


```
- Using the classmethod decorator: You can define a class method using the classmethod decorator and use it to set a class attribute. A class method is a method that is bound to the class and not the instance of the class.
```
```
class MyClass:
    x = 1

    @classmethod
    def set_x(cls, value):
        cls.x = value
print(MyClass.x)
MyClass.set_x(2)
print(MyClass.x)

```


<b> Q12. Where and how are instance attributes created? </b>
```
- Inside the __init__ method you need to assign a value to self.variable_name. These attributes will be specific to each instance of the class and can be different for each instance.
```
```
class MyClass:
    def __init__(self, value):
        self.x = value

obj1 = MyClass(1)
print(obj1.x)  # Output: 1
```

<b> Q13. What does the term "self" in a Python class mean? </b>
```
In Python classes, self keyword represents the instance of that class. it stores the reference of that instance.
```

<b> Q14. How does a Python class handle operator overloading? </b>
```
In Python, you can define methods in a class to overload operators for instances of the class. This allows you to define how operators such as +, -, *, and / should behave when applied to instances of your class.

```
```
class MyClass:
    def __init__(self, value):
        self.value = value
    
    def __add__(self, other):
        return MyClass(self.value + other.value)
    
    def __sub__(self, other):
        return MyClass(self.value - other.value)
    
    def __mul__(self, other):
        return MyClass(self.value * other.value)
    
    def __"true"div__(self, other):
        return MyClass(self.value / other.value)


a = MyClass(10)
b = MyClass(20)
c = a + b  # c is a new instance of MyClass with value 30
d = a - b  # d is a new instance of MyClass with value -10
e = a * b  # e is a new instance of MyClass with value 200
f = a / b  # f is a new instance of MyClass with value 0.5

```



<b> Q15. When do you consider allowing operator overloading of your classes? </b>
```
Here are a few guidelines to help you decide when to consider operator overloading:

- Make sure that operator overloading makes sense semantically for your class. For example, if you are creating a class to represent a complex number, it makes sense to overload the + operator to allow complex numbers to be added together.

- Consider whether operator overloading will make your code easier to understand and maintain. If the meaning of an operator is ambiguous or difficult to understand when applied to objects of your class, it may be better to use a different approach.

```

<b> Q16. What is the most popular form of operator overloading? </b>
```
The most popular form of operator overloading is probably the use of magic methods in Python. Magic methods, also known as dunder methods (short for "double underscore methods"), are special methods that you can define in a Python class to overload various operators.

```

<b> Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code? </b>
```
two of the most important concepts are: 

1) Class: A class is a template or blueprint for creating objects. It defines the attributes and methods that the objects will have, as well as the behavior of the objects. 

2)An object is an instance of a class. When you create an object of a particular class, you are creating an instance of that class. Objects have attributes and methods that are defined by the class.
```


<b> Q18. Describe three applications for exception processing. </b>
```
Here are three common applications for exception processing in Python:

Handling errors: Exception processing is often used to handle errors and exceptions that may occur during the execution of your code. For example, you might use exception processing to handle an error that occurs when you try to open a file that does not exist, or when you try to divide by zero.

Validating user input: Exception processing can be used to validate user input and ensure that it meets certain criteria. For example, you might use exception processing to handle an error that occurs when a user enters a non-integer value when a numeric value is expected.

Debugging and testing: Exception processing can be a useful tool for debugging and testing your code, as it allows you to identify and fix errors and exceptions that may occur during the execution of your code.
```

<b> Q19. What happens if you don't do something extra to treat an exception? </b>
```
If we don't do anything extra to handle an exception our execution will be stopped.
```

<b> Q20. What are your options for recovering from an exception in your script? </b>
```
There are two options for recovering from an exception:

1 ) Handling the exception: One option is to handle the exception using a try statement and an except statement. The try statement encloses the code that may raise an exception, and the except statement catches the exception and provides an appropriate response.

2)Logging the exception: Another option is to log the exception using a logging library, such as the built-in logging module. This allows you to record the exception and any relevant information, such as the stack trace, and use it to debug and fix the error.
```
<b> Q21. Describe two methods for triggering exceptions in your script. </b>
```
1) Using the raise statement: You can use the raise statement to raise an exception manually. 

2) using try and and except : you can write some illigal statement in try block which will trigger the exeption.

```

<b> Q22. Identify two methods for specifying actions to be executed at termination time, regardless of  
whether or not an exception exists. </b>
```
Using the finally clause: The finally clause of a try statement can be used to specify actions that should be executed at termination time, regardless of whether or not an exception exists.
```
```
Using the atexit module: The atexit module provides a way to register functions to be called at program termination. You can use the atexit.register function to register a function that should be executed at termination time. For example:

```
<b> Q23. What is the purpose of the try statement? </b>
```
The try statement in Python is used to handle errors that may occur during the execution of your code. It allows you to specify code that should be executed in an attempt to handle an error
```
<b> Q24. What are the two most popular try statement variations? </b>
```
try:
    # Code that might raise an exception
except ExceptionType:
    # Code to handle the exception
else:
    # Code to be executed if no exception is raised
finally
    # compulsory Code to be executed 
```

<b> Q25. What is the purpose of the raise statement? </b>
```
The raise statement in Python is used to raise an exception. It allows you to interrupt the normal flow of control in your program and transfer control to an exception handler.


```

<b> Q26. What does the assert statement do, and what other statement is it like? </b>
```
The assert statement in Python is used to evaluate a condition, and raise an  exception if the condition is False
assert condition, message

```



<b> Q27. What is the purpose of the with/as argument, and what other statement is it like? </b>
```
When we open any file it is crucial to close the file, otherwise it will keep consuming our resources. 

with/as statement make sure that once we have executed the code block, it frees the resources.
```

<b> Q28. What are *args, **kwargs? </b>
```
*args is a tuple that contains all the positional arguments passed to a function that are not already specified as formal parameters. It allows you to define a function that can accept an arbitrary number of arguments.
```
```
def print_numbers(*args):
    for arg in args:
        print(arg)

# Call the function with multiple arguments
print_numbers(1, 2, 3, 4, 5)
# Output: 1, 2, 3, 4, 5

```

```
**kwargs is a dictionary that contains all the keyword arguments passed to a function that are not already specified as formal parameters. It allows you to define a function that can accept an arbitrary number of keyword arguments.

```
```
def print_keywords(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

# Call the function with multiple keyword arguments
print_keywords(name="Alice", age=30, city="New York")
# Output: name: Alice, age: 30, city: New York

```
<b> Q29. How can I pass optional or keyword parameters from one function to another? </b>
```
To pass optional or keyword parameters from one function to another, you can use the * and ** syntax when calling the second function.

```
```
def func1(arg1, arg2, *args):
  # do something with the arguments
  print(arg1, arg2, args)

def func2(arg1, arg2, *args):
  # call func1 and pass on the optional arguments
  func1(arg1, arg2, *args)

# call func2 with three arguments
func2(1, 2, 3, 4, 5)

```
<b> Q30. What are Lambda Functions? </b>
```
In Python, a lambda function is a small anonymous function without a name. It is defined using the lambda keyword, and it has the following syntax:

lambda arguments: expression

```
<b> Q31. Explain Inheritance in Python with an example? </b>
```
In Python, inheritance is a way to create a new class that is a modified version of an existing class. The new class is called the subclass, and the existing class is the superclass.
```

```
class pet:
    def __init__(self, name, species):
        self.name = name
        self.species = species
class dog():
    def __init__(self, name,species):
        super().__init__(name, species="Dog")
        self.legs = 4

dog = dog("bassanti", "Labrador")
print(dog.name) 
```

<b> Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of 
class C, which version gets invoked? </b>
```
In python, methods are inherited from the leftmost superclass first, and then from the rightmost superclass.

So version of A class will be invoked
```
<b> Q33. Which methods/functions do we use to determine the type of instance and inheritance? </b>
```
-> In Python, you can use the type() function to determine the type of an instance. For example:
```
```
In Python, you can use the type() function to determine the type of an instance. For example:
```
```
You can also use the isinstance() function to check if an instance is of a particular type. such way we can identigy the type of inharitance
```
```
You can also use the isinstance() function to check if an instance is of a particular type. For example:
```


<b> Q34.Explain the use of the 'nonlocal' keyword in Python. </b>
```
 the nonlocal keyword is used to modify variables defined in a parent, It is used in nested functions, where the inner function needs to modify a variable defined in the outer function. 

```

```
def outer_function():
    x = 10

    def inner_function():
        nonlocal x
        x += 1
        print(x)

    inner_function()
    print(x)

outer_function()  # Output: 11, 11

```
<b> Q35. What is the global keyword? </b>
```
global keyword is used to access/define global variables.
```
