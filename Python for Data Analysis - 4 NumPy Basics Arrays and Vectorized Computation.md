%%tags: #python #datascience #mckinney%%
parent: [Python for Data Analysis 3rd ed. - Wes McKinney](Python%20for%20Data%20Analysis%203rd%20ed.%20-%20Wes%20McKinney.md)

# Concepts
- Numpy is designed for efficiency of large arrays of data
- Numpy has C-based algorithms that can be 10-100x faster than the pure Python counterpart and use a lot less memory.
## 4.1 The NumyPy ndarray: A Multidimensional Array Object
- import numpy as np is the standard using `from numpy import *` can result in namespace conflicts with built-in functions like `min` and `max`. 
- <u>Vectorization</u>: replacement of explicit loops with optimized pre-compiled operations on entire arrays. NumPy is an example of vectorization.
- `1/arr` is to take the element-wise reciprocal. It is <u>NOT</u> the inverse of a matrix
- Array slices of Python built-in lists are views of the original array, but not so with NumPy arrays. Modifications to the "view" for NumPy arrays will be reflected in the source array. Note this is similar to the variable binding with variable assignments being references to the same object not copies of the object, but it so happens that slices of iterables <u>ARE a copy and create a new object in memory</u>
	- to make sure you don't edit the original NumPy array, you need to create a copy `arr.copy()`
- NumPy arrays have tuple indexing <u>unlike python lists</u>. Where as in python you may have to do `arr[0][2]` with NumPy you can access it as `arr[0,2]` (Note if index is just a number element, the returned value is not an integer but a NumPy object)
- NumPy supports Boolean indexing. 
	- NumPy does not use Python built-in logic operators `and` and `or`. Must use `&` and `|` instead.
- Transpose method with `arr.T`
## 4.3 Universal Functions: Fast Element-Wise Array Functions
- Universal functions, ufunc for short, are numpy functions that performs element-wise operations on nd.arrays such as `numpy.sqrt(arr)` or `numpy.exp(arr)`. 
	- ufuncs acting on only one variable are unary ufuncs
	- binary ufuncs take two arrays and return a single array such as `np.maximum(arr1,arr2)`
