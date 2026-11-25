# Day 5 – Introduction to NumPy

## 🎯 Learning Objectives

By the end of this lesson, I learned how to:

- Understand what NumPy is and why it is useful.
- Import NumPy using `import numpy as np`.
- Create NumPy arrays.
- Perform mathematical operations on arrays.
- Use built-in NumPy functions.
- Access array elements using indexing and slicing.
- Create and work with 2D arrays (matrices).
- Understand array properties such as shape, ndim, size, and dtype.
- Apply NumPy to simple Machine Learning tasks.

## 1. What is NumPy?

NumPy stands for **Numerical Python**.

It is a Python library used for:
- Working with large collections of numbers.
- Performing mathematical calculations.
- Creating arrays and matrices.
- Preparing numerical data for Machine Learning.

### Installation

If NumPy is not already installed, run:

```bash
pip install numpy
```

Google Colab usually comes with NumPy pre-installed.

## 2. Import NumPy

```python
import numpy as np
```

The alias `np` is the standard shortcut for NumPy.

## 3. Creating NumPy Arrays

```python
import numpy as np

numbers = np.array([10, 20, 30, 40, 50])

print(numbers)
print(type(numbers))
```

**Output:**
```text
[10 20 30 40 50]
<class 'numpy.ndarray'>
```

## 4. Array Calculations

NumPy allows us to perform calculations on every element without writing loops.

```python
numbers = np.array([10, 20, 30, 40])

print(numbers + 5)
print(numbers * 2)
print(numbers - 3)
print(numbers / 10)
```

**Output:**
```text
[15 25 35 45]
[20 40 60 80]
[ 7 17 27 37]
[1. 2. 3. 4.]
```

## 5. Important NumPy Functions

```python
numbers = np.array([10, 20, 30, 40, 50])

print(np.mean(numbers))
print(np.median(numbers))
print(np.max(numbers))
print(np.min(numbers))
print(np.sum(numbers))
print(np.std(numbers))
```

| Function | Purpose |
|---|---|
| `np.mean()` | Calculates the average |
| `np.median()` | Finds the middle value |
| `np.max()` | Finds the largest value |
| `np.min()` | Finds the smallest value |
| `np.sum()` | Calculates the total |
| `np.std()` | Calculates standard deviation |

## 6. Array Indexing and Slicing

```python
numbers = np.array([10, 20, 30, 40, 50])

print(numbers[0])
print(numbers[2])
print(numbers[-1])
print(numbers[1:4])
```

**Output:**
```text
10
30
50
[20 30 40]
```

Remember: Python indexing starts at 0.

## 7. Two-Dimensional Arrays (Matrices)

A 2D array contains rows and columns.

```python
matrix = np.array([
    [10, 20, 30],
    [40, 50, 60],
    [70, 80, 90]
])

print(matrix)

print(matrix[0, 0])
print(matrix[1, 2])
print(matrix[2, 1])
```

**Output:**
```text
[[10 20 30]
 [40 50 60]
 [70 80 90]]

10
60
80
```

## 8. Useful Array Properties

```python
matrix = np.array([
    [10, 20, 30],
    [40, 50, 60]
])

print(matrix.shape)
print(matrix.ndim)
print(matrix.size)
print(matrix.dtype)
```

**Output:**
```text
(2, 3)
2
6
int64
```

| Property | Meaning |
|---|---|
| `.shape` | Number of rows and columns |
| `.ndim` | Number of dimensions |
| `.size` | Total number of elements |
| `.dtype` | Data type of elements |

*Note: The exact dtype may depend on your system and values.*

## 9. NumPy and Machine Learning

NumPy is useful for analyzing numerical datasets.

Example: Analyzing students' exam scores.

```python
scores = np.array([75, 80, 90, 65, 85])

average = np.mean(scores)
highest = np.max(scores)
lowest = np.min(scores)

print("Average:", average)
print("Highest:", highest)
print("Lowest:", lowest)
```

**Output:**
```text
Average: 79.0
Highest: 90
Lowest: 65
```

Machine Learning uses similar numerical operations to process data, identify patterns, and make predictions.

## 10. Practical Exercises

- [ ] **Exercise 1:** Create a NumPy array containing 5, 10, 15, 20, 25.
- [ ] **Exercise 2:** Multiply every element of the array by 3.
- [ ] **Exercise 3:** Calculate the average of [12, 15, 18, 20, 25].
- [ ] **Exercise 4:** Find the maximum and minimum values in [45, 12, 89, 34, 67].
- [ ] **Exercise 5:** Create a 2D array with 2 rows and 3 columns.
- [ ] **Exercise 6:** Print the shape and number of dimensions of your 2D array.

## 11. Day 5 Quiz

**1. What does NumPy stand for?**

- Numerical Python
- New Python
- Number Program

**2. Which function calculates the average?**

- `np.sum()`
- `np.mean()`
- `np.max()`

**3. What does `.shape` return?**

- Data type
- Number of dimensions only
- Array dimensions

**4. How do you multiply every array element by 2?**

- `array * 2`
- `array.append(2)`
- `array.multiply(2)`

**5. What is a 2D array?**

- A single number
- An array with rows and columns
- A text string


## ✅ Day 5 Completion Checklist

- [x] Understand what NumPy is.
- [x] Learn how to create NumPy arrays.
- [x] Perform array calculations.
- [x] Use important NumPy functions.
- [x] Understand indexing and slicing.
- [x] Create 2D arrays and matrices.
- [x] Learn array properties.
- [ ] Complete all six exercises.
- [ ] Complete the quiz.
- [ ] Push the project to GitHub.


