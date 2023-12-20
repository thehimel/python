# A Comprehensive Guide on Numpy

> Authored by Himel Das

## What is NumPy?

NumPy is a robust package in Python used for numerical computing. It stands for `Numerical Python` and provides support
for arrays, matrices, and high-level mathematical functions to operate on these arrays efficiently. 

## What Are the Key Features of NumPy? | Why NumPy is Used over Python Lists?

* **N-dimensional arrays**: A multidimensional array object named `ndarray` is provided in NumPy. These arrays are the 
foundation for most numerical computations in Python.
* **Efficient memory management**: NumPy arrays are memory-efficient and provide superior memory management than Python
lists, especially when working with huge datasets.
* **Speed**: Array object in NumPy is much faster than Python lists.
* **Mathematical functions**: Numerous mathematical functions are available in NumPy such as trigonometric, statistical,
linear algebra, Fourier analysis, and more.
* **Vectorized operations**: NumPy supports element-wise operations on arrays without the need for explicit looping,
resulting in faster execution of operations on big datasets.
* **Broadcasting**: It's a strong method that allows NumPy to execute arithmetic operations on arrays of various shapes,
which can substantially simplify coding.

## Why is NumPy Quicker than Lists?

* **Contiguous Memory Allocation**: NumPy arrays are stored in contiguous memory blocks, which allows for efficient
caching and faster element access. Python lists, which are arrays of pointers to objects, may result in scattered memory
allocation, leading to longer access times.
* **Homogeneous Data Type**: NumPy arrays feature a fixed data type for all elements, allowing for better memory
utilization and faster processing. Python lists, on the other hand, might contain components of various types,
resulting in added complexity for type checking and handling.
* **Vectorized Operations**: NumPy supports vectorized operations, which allow mathematical operations on full arrays to
be performed without the use of explicit loops. This vectorization makes use of pre-compiled, optimized C and Fortran
algorithms, resulting in speedier execution as compared to Python's interpreted loops over lists.
* **Optimized Algorithms**: NumPy performs sophisticated mathematical operations such as linear algebra, Fourier
transforms, statistical functions, and so on with optimized algorithms developed in C and Fortran, resulting in speedier
performance when compared to identical operations performed with Python's built-in functions or loops.
* **Efficient C Implementation**: Fundamental operations of NumPy are written in C, which allows for low-level access to
memory and hardware, resulting in faster performance than Python's interpreted nature.

## Where is NumPy used?

NumPy is widely used in scientific computing, data analysis, machine learning, and a variety of other disciplines where
numerical computations and massive dataset processing are required. Its array-oriented computing capabilities make it a
fundamental library for numerical operations in the Python ecosystem.

## Write a Python Code with NumPy to Demonstrate Mean, Maximum, and Sine Values of Each Element in an Array

### Code

```python
import numpy as np

# Create a NumPy array
arr = np.array([1, 2, 3, 4, 5])

print(np.mean(arr))  # Calculate mean
print(np.max(arr))   # Find maximum value
print(np.sin(arr))   # Compute sine of each element
```

### Output

```shell
3.0
5
[ 0.84147098  0.90929743  0.14112001 -0.7568025  -0.95892427]
```

## Where is NumPy Codebase Situated?

* https://github.com/numpy/numpy

## What Programming Languages are Used to Build NumPy?

* Mainly C, C++, Fortran, and Python.

## How to Install NumPy?

Install NumPy with `pip install numpy` considering Python is already installed in the system.

### How to Check the Version in NumPy?

```python
import numpy

print(numpy.__version__)
```

## Create 0D, 1D, 2D, and 3D Arrays with NumPy

> 

```python
import numpy as np

arr_0d = np.array(42)  # 0D array (scalar)
print("0D Array (Scalar):\n", arr_0d)

arr_1d = np.array([1, 2, 3, 4, 5])  # 1D array
print("\n1D Array:\n", arr_1d)

arr_2d = np.array([[1, 2, 3], [4, 5, 6]])  # 2D array
print("\n2D Array:\n", arr_2d)

arr_3d = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])  # 3D array
print("\n3D Array:\n", arr_3d)
```

### How Many Dimensions an Array Can Have in NumPy?

NumPy allows you to generate arrays of any number of dimension, and the number of dimensions is only limited by
available memory and system constraints.
