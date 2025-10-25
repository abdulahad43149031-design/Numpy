# 🔢 Exploring NumPy Fundamentals

This repository contains a Jupyter Notebook (`numpyFundamentals.ipynb`) that serves as a comprehensive introduction to the fundamental concepts and operations of the NumPy library. It's a hands-on guide perfect for anyone starting with NumPy for data science, machine learning, or scientific computing.

The notebook explores the core NumPy object, the `ndarray`, and demonstrates why it's the foundation of the Python data science ecosystem.

## 🚀 Key Topics Covered

This notebook is structured as a tutorial, covering the following key areas:

### 1. ⚡ Performance: NumPy vs. Python Lists

* **Speed Comparison:** A practical, timed demonstration (`time.time()`) comparing a vectorized NumPy array operation (`my_arr * 2`) against a standard Python list comprehension (`[x * 2 for x in my_arr]`).
* **Conclusion:** Highlights the significant performance advantage of NumPy for large datasets due to its C-based backend and contiguous memory storage.

### 2. 🛠️ Creating ndArrays

Covers the essential methods for creating NumPy arrays:
* `np.array()`: From existing Python lists (1D and 2D).
* `np.zeros()`: Creating arrays filled with zeros.
* `np.ones()`: Creating arrays filled with ones.
* `np.arange()`: Creating arrays with a range of values.
* `np.random`: A deep dive into the random module.

### 3. 🎲 The `np.random` Module

Demonstrates how to generate various types of random data:
* `np.random.rand()`: Random floats from a uniform distribution [0, 1).
* `np.random.randint()`: Random integers within a specified range.
* `np.random.randn()`: Samples from a standard normal distribution (mean=0, std=1).
* `np.random.normal()`: Samples from a normal distribution with a specified mean and standard deviation.
* `np.random.shuffle()`: In-place shuffling of array elements.

### 4. 📊 Visualizations

Uses `matplotlib` and `seaborn` to create histograms (`sns.histplot`) that visually confirm the properties of `np.random.randn` and `np.random.normal`, showing their distributions.

### 5. 🧮 Array Attributes and Arithmetic

* **Attributes:** Accessing core properties like `.shape` and `.dtype`.
* **Type Casting:** Explicitly changing an array's data type using `.astype()`.
* **Vectorized Operations:** Performing fast, element-wise arithmetic (e.g., `arr * arr`, `1 / arr`, `arr ** 0.5`).
* **Comparisons:** Creating boolean arrays from element-wise comparisons (e.g., `arr2 > arr`).

### 6. 🪓 Indexing and Slicing

A detailed look at how to access and modify array data:
* **1D Slicing:** Basic `arr[5]`, range slicing `arr[5:8]`, and value assignment.
* **Views vs. Copies:** A critical concept. It explains how array slices are *views* of the original data, and any modification to the slice changes the original array. Demonstrates how to use `.copy()` to create a true, independent copy.
* **2D Slicing:** Accessing rows, columns, and sub-matrices (e.g., `arr2d[1, :2]`, `arr2d[:2, 1:]`).

### 7. 💭 Boolean Indexing

Using boolean masks to select, filter, and modify data. This is one of NumPy's most powerful features.
* Selecting elements based on a condition: `integer[condition]`.
* A practical example using a `names` array to filter rows in a corresponding `data` matrix.
* Combining conditions with logical operators (`|` for OR) and negating conditions (`~` for NOT).
* Setting values based on a condition: `data[data < 0] = 0`.

### 8. 🔄 Transposing and Ufuncs

* **Transposing:** Using the `.T` attribute to transpose matrices.
* **Matrix Multiplication:** A brief example using `np.dot()`.
* **Universal Functions (Ufuncs):**
    * **Unary Ufuncs:** `np.sqrt()`, `np.exp()`.
    * **Binary Ufuncs:** `np.maximum()`.
    * **Aggregation:** `.mean()`, `.any()`, `.all()`.
    * **Axis Control:** Using the `axis` parameter to perform aggregations along rows (`axis=1`) or columns (`axis=0`).

### 9. ↔️ Broadcasting

Explains how NumPy handles arithmetic between arrays of different (but compatible) shapes.
* **Scalar Broadcasting:** Operations between an array and a single number.
* **Array Broadcasting:** A practical example of **demeaning data** by subtracting the column-wise mean (`mat.mean(axis=0)`) from the entire matrix.

## 📦 Dependencies

To run this notebook, you will need the following libraries:
* `numpy`
* `matplotlib`
* `seaborn`
* `jupyter` (to run the notebook)

## 💡 How to Use

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/abdulahad43149031-design/Numpy
    ```

2.  **Install dependencies:**
    ```bash
    pip install numpy matplotlib seaborn jupyter
    ```

3.  **Run Jupyter Notebook:**
    ```bash
    jupyter notebook numpyFundamentals.ipynb
    ```

    ## 👨‍💻 Author  

**Abdul Ahad**  
AI/ML Undergraduate, IIIT Nagpur  
Focused on Numerical Computing, Python, and Data Science.  

---

⭐ If this helped you understand NumPy fundamentals better, give it a star on GitHub!
