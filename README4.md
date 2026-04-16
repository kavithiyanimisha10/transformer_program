# 📊 Data Analyzer and Transformer Program

## 🔍 Project Description

This is a **menu-driven Python application** designed to perform data
analysis and transformation on user-input datasets.\
The program supports both **1D (single list)** and **2D (matrix-like
list)** data structures, making it flexible for basic analytical
operations.

It is a great beginner-to-intermediate level project to understand how
real-world data processing systems work.

------------------------------------------------------------------------

## 🎯 Objectives of the Project

-   To understand how to handle dynamic user input
-   To perform statistical operations on datasets
-   To implement clean modular programming using functions
-   To work with both **flat (1D)** and **nested (2D)** data
-   To apply concepts like **lambda functions, list comprehension, and
    condition checking**

------------------------------------------------------------------------

## ⚙️ Program Workflow

1.  The program starts with a **main menu**
2.  The user selects an operation
3.  Based on the choice, a specific function is executed
4.  The dataset (`lst`) is globally shared across functions
5.  The program runs continuously until the user selects **Exit**

------------------------------------------------------------------------

## 🧩 Detailed Feature Explanation

### 1. Enter Data (`enter_data`)

This function allows the user to input data in two formats:

#### ➤ 1D List

-   User enters number of elements
-   Values are stored directly in a list

#### ➤ 2D List

-   User defines rows and columns
-   Data is stored as a list of lists (matrix format)

📌 Example:

    1D → [1, 2, 3, 4]
    2D → [[1, 2], [3, 4]]

------------------------------------------------------------------------

### 2. Data Summary (`data_summary`)

This function performs statistical analysis using **nested functions**:

#### Internal Functions:

-   `total_element()` → Counts elements (length of outer list)
-   `sum_num()` → Calculates total sum
-   `min_num()` → Finds smallest value
-   `max_num()` → Finds largest value
-   `avg_num()` → Calculates average

📌 Special Logic: - Uses `isinstance(i, list)` to detect 2D lists -
Flattens data logically when needed

⚠️ Note: For 2D lists, average is calculated using number of rows (can
be improved)

------------------------------------------------------------------------

### 3. Factorial (`factorial`)

-   Calculates factorial using **iteration**
-   Formula:

```{=html}
<!-- -->
```
    n! = n × (n-1) × (n-2) × ... × 1

📌 Example:

    5! = 120

------------------------------------------------------------------------

### 4. Filter Data (`filter_data`)

Filters elements greater than a given threshold.

#### Concepts Used:

-   **Lambda Function**
-   **List Flattening (for 2D lists)**

📌 Logic: - Converts 2D list into 1D - Applies:

    filter(lambda x: x > threshold, data)

------------------------------------------------------------------------

### 5. Sort Data (`sort_data`)

Sorting behavior differs based on data type:

#### ➤ 1D List

-   Ascending or Descending order

#### ➤ 2D List

-   Each row is sorted individually

📌 Example:

    [[3,1],[4,2]] → [[1,3],[2,4]]

------------------------------------------------------------------------

### 6. Return Dataset Statistics (`return_dataset`)

Returns multiple values: - Minimum value - Maximum value - Average

📌 Uses: - Tuple return - Data flattening for 2D lists

------------------------------------------------------------------------

## 🧠 Key Concepts Used

### ✔ Functions

Each task is modularized into separate functions for clarity and reuse.

### ✔ Nested Functions

Used inside `data_summary` to logically group related calculations.

### ✔ Global Variables

The dataset (`lst`) is shared across functions.

### ✔ List Comprehension

Used to flatten 2D lists:

    [j for i in lst for j in i]

### ✔ Lambda Functions

Used for filtering data dynamically.

### ✔ Conditional Type Checking

    isinstance(i, list)

Helps differentiate between 1D and 2D lists.

------------------------------------------------------------------------

## ▶️ How to Run the Program

1.  Install Python (if not installed)
2.  Save the code in a file (e.g., `data_analyzer.py`)
3.  Open terminal and run:

```{=html}
<!-- -->
```
    python data_analyzer.py

4.  Follow the menu instructions

------------------------------------------------------------------------

## 📋 Menu Structure

1.  Enter Data\
2.  Display Data Summary\
3.  Calculate Factorial\
4.  Filter Data\
5.  Sort Data\
6.  Return Dataset Statistics\
7.  Exit

------------------------------------------------------------------------

## ⚠️ Limitations

-   Only supports integer input
-   No validation for empty dataset
-   Average calculation for 2D lists is not fully accurate
-   Global variable usage can reduce scalability

------------------------------------------------------------------------

## 🚀 Future Enhancements

-   Add **input validation**
-   Support **float values**
-   Improve **average calculation for 2D lists**
-   Add **file handling (CSV, Excel)**
-   Build a **GUI using Tkinter or Streamlit**
-   Integrate **data visualization (Matplotlib, Seaborn)**

------------------------------------------------------------------------

## 👩‍💻 Learning Outcome

By building this project, you will understand: - How real data
processing works - Writing structured and maintainable Python code -
Handling complex data structures - Building logic for real-world
problems

------------------------------------------------------------------------

## 📌 Conclusion

This project is a strong foundation for moving into: - Data Analysis -
Data Science - Backend Development

It demonstrates how basic Python concepts can be combined to build a
functional analytical tool.

## explaination viedo

https://drive.google.com/file/d/1aSRSveJJjzB9GYK0IU3kvhqT1RsrcR8Q/view?usp=drive_link