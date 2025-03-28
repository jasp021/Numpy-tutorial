# NumPy Tutorial Repository

> This repository documents my journey learning NumPy, following the [***Code With Harry***](https://www.codewithharry.com/)&ensp; YouTube tutorial. Explore the code and examples to deepen your understanding of NumPy!

## 📺 Tutorial Video

Watch the tutorial on YouTube: [**NumPy Tutorial by Code With Harry**](https://youtu.be/Rbh1rieb3zc?si=eXCG74aqaVBilxPa)

---

## 🖥️ Environment Setup

- **Operating System:** Ubuntu (via WSL 2)
- **Editor/IDE:** Jupyter Lab
- **Programming Language:** Python

---

## 📚 Topics Covered

### Creating and Manipulating Arrays

- **Array Creation**
  - Using `numpy.array()`
  - Intrinsic creation methods:
    - `np.zeros`
    - `np.arange`
    - `np.linspace`
    - `np.empty`
    - `np.empty_like`
    - `np.identity`

- **Data Types**
  - Changing `dtype` (e.g., `int8`, `int32`, `int64`)

- **Array Properties**
  - `.shape`
  - `.size`
  - `.dtype`

### Array Reshaping and Flattening

- Reshape arrays with `arr.reshape`
- Flatten arrays using `arr.ravel`

### Array Operations and Functions

- **Axis Operations**
  - Utilizing `axis=0` and `axis=1`
  - Transposing arrays using `array.transpose()`

- **Iteration and Indexing**
  - Iterating over elements with `array.flat`
  - Finding indices using:
    - `array.argmin()`
    - `array.argmax()`
    - `array.argsort()`

- **Mathematical Operations**
  - Square root of array elements: `np.sqrt(ar)`
  - Summing elements: `array.sum()`
  - Finding maximum and minimum: `array.max()`, `array.min()`

- **Conditional Operations**
  - Filtering with `np.where(ar > 5)`
  - Counting non-zero elements using:
    - `np.count_nonzero(ar)`
    - `np.nonzero(ar)`

### Memory Size Calculation

- Calculate using Python's built-in function:
  - `sys.getsizeof(1) * len(py_ar)`
- Calculate using NumPy's properties:
  - `np_ar.itemsize * np_ar.size`

---

## 📂 Files

- **Notebook:** `Numpy.ipynb`  
  This Jupyter Notebook contains all the code examples and experiments related to the tutorial.

---

## 💻 Sample Code

Below is an example snippet demonstrating some of the functionalities covered:

```python
import numpy as np
import sys

# Creating a NumPy array from a Python list
py_ar = [1, 2, 3, 4, 5]
np_ar = np.array(py_ar)

# Display array properties
print("Shape:", np_ar.shape)
print("Size:", np_ar.size)
print("Data type:", np_ar.dtype)

# Array creation methods
zeros_arr = np.zeros((3, 3))
range_arr = np.arange(10)
linspace_arr = np.linspace(0, 1, 5)
empty_arr = np.empty((2, 2))
identity_arr = np.identity(3)

# Reshape and flatten the array
reshaped_arr = np_ar.reshape((5, 1))
flattened_arr = np_ar.ravel()

# Array operations
print("Minimum index:", np_ar.argmin())
print("Maximum index:", np_ar.argmax())
print("Sorted indices:", np.argsort(np_ar))

# Mathematical operations
sqrt_arr = np.sqrt(np_ar)
print("Square root of array:", sqrt_arr)
print("Sum of elements:", np_ar.sum())
print("Max element:", np_ar.max())
print("Min element:", np_ar.min())

# Conditional operations
filtered_indices = np.where(np_ar > 3)
print("Indices where elements > 3:", filtered_indices)
nonzero_count = np.count_nonzero(np_ar)
print("Count of non-zero elements:", nonzero_count)

# Memory size calculations
memory_python = sys.getsizeof(1) * len(py_ar)
memory_numpy = np_ar.itemsize * np_ar.size
print("Memory (using sys.getsizeof):", memory_python)
print("Memory (using np.itemsize):", memory_numpy)
```
---

## ⚡ Getting Started:

1. **Clone the Repository:**

```bash
git clone <repository-url>
```

2. **Navigate to the Directory:**

```bash
cd <repository-folder>
```

3. **Launch Jupyter Lab:**

```bash
jupyter lab
```

4. **Open Numpy.ipynb and explore the examples!**

---

## 🔧 Contributing

Feel free to fork this repository and submit pull requests for any improvements or additional examples.  
For any issues, please open an issue on GitHub.

---

## 🙏 Acknowledgements

* [***Code With Harry***](https://www.codewithharry.com/)&ensp; for the comprehensive tutorial that inspired this repository.

* The open-source community for continuous learning and sharing knowledge.
---

## 🪪 License

This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2025 Jaspreet Singh Kalsi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```

----------