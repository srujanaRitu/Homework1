### What does one need to do to use a module?

--> Anytime you use a module, you have to IMPORT it into your program
    import welcome

### Name a Module (not the DateTime Nodule) we looked at and write a line or 2 of code as an example using this module.

import math
result = math.sqrt(25)
print(result)

### What is a benefit of using Exception handling?

Python generates a message called an exception, when an error or exception occurs in a called block of code.


### what are the 4 components used for Python Exception Handling?

* The try block lets you test a block of code for errors.

* The except block lets you handle the error.

* The else block lets you execute code when there is no error.

* The finally block lets you execute code, regardless of the result of the try- and except blocks.


### NumPy arrays are like what Python data type?

NumPy arrays are most similar to Python lists.

### What is one of the main benefits of using NumPy arrays.

1.Less Memory - NumPy arrays occupy less memory 
2.Fast - NumPy arrays are faster 
3.Convenient - it is convenient to work with NumPy

NumPy array elements are homogeneous -- of the same or a similar kind or nature.

### What is one of the main requirements about the 'dtype' of NumPy arrays?
 Changes array's data type.
 While the default data type of a NumPy Array is floating point (np.float64), you can explicitly specify which data type you want using the dtype keyword.

NumPy supports a much greater variety of numerical data types than Python does natively.

Along with these NumPy dtypes there are a bunch of methods to change and manipulate data types. So, even though your data might be of one type, you could possibly change that to better work with your project.

Of the 10 uses of NumPy, name 2.

1. It contains a multidimensional array and matrix data structure (in the form of rows and columns)
2. Supplies an enormous library of high-level mathematical functions that operate on these arrays and matrices

### Name one of the other libraries we'll use with NumPy?

One of the most common libraries used alongside NumPy is Pandas.

### What is the shape of NumPy arrays?

# import numpy as np

# ar1 = np.ar1([[10,15,20], [25,30,35]])

# print(ar1.shape)

Output : (2, 3)

### What is a Tensor?

Tensor == an array with 3+ dimensions

### Name a reason why it's better using NumPy for Data Analysis than using a Python List?

We use Python NumPy array instead of a list because of the below three reasons:

> Less Memory - NumPy arrays occupy less memory as compared to lists
> Fast - NumPy arrays are faster compared to lists
> Convenient - it is convenient to work with NumPy

### When creating an "empty" array, where do the elements come from?


 ~~~ When you create an "empty" array, there are no elements in it initially. It's just a container that has been allocated in memory, ready to hold values, but it doesn't contain any actual data yet.

~~~ Python: An empty list ([] or list()) has no elements. The list is created, but there is nothing in it until you append values.

~~~ Empty will fill in values based on memory