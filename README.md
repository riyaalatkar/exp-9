
### 1. Aim

To explore and implement the fundamental capabilities of the **NumPy** library in Python, specifically focusing on array creation, attribute inspection, specialized matrix generation, and basic statistical operations.

---

### 2. Theory

#### Array Initialization and Attributes**

NumPy’s core object is the **ndarray** (n-dimensional array). Unlike standard Python lists, these arrays are memory-efficient and allow for vectorized operations.

* **`.ndim`**: Returns the number of dimensions (axes) of the array.
* **`.shape`**: Returns a tuple representing the size of the array in each dimension.
* **`.dtype`**: Identifies the data type of the elements. Notice in your code how the presence of `500.5` automatically upcasted the entire array `a` to `float64`.

#### Specialized Array Creation**

Generating placeholder arrays is essential for initializing weights in machine learning or setting up coordinate grids.

* **`np.zeros` / `np.ones**`: Creates arrays filled entirely with 0 or 1.
* **`np.eye`**: Creates an **Identity Matrix**, where the main diagonal is 1 and all other elements are 0.

#### Numerical Sequences**

* **`np.arange(start, stop, step)`**: Generates values within a half-open interval `[start, stop)` with a specific increment.
* **`np.linspace(start, stop, num)`**: Generates `num` evenly spaced samples over a specified interval. This is particularly useful for plotting functions.

#### Vectorized Arithmetic**

This block demonstrates **Broadcasting**. Instead of writing a `for` loop to multiply every element by 2 or add 5, NumPy applies the operation across the entire array simultaneously. This is significantly faster than standard Python loops for large datasets.

#### Statistical Aggregation**

NumPy provides built-in functions to perform mathematical analysis on data:

* **`mean` / `median**`: Measures of central tendency.
* **`sum` / `max**`: Basic descriptive statistics to understand the range and volume of the dataset.

---

### 3. Conclusion

Through this study, I have successfully implemented the primary functions of the NumPy library. I observed that NumPy arrays are more rigid than Python lists regarding data types (homogeneity) but offer superior performance through vectorization. The ability to generate identity matrices and linearly spaced vectors provides a foundation for more advanced computational tasks in data science and linear algebra.

---
