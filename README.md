# ECE-2112-PA3
**Made by: Elijah Theodore P. Rojo | 2ECE-D**

This repository contains the Programming Assignment 3 for our course "Advanced Computer Programming" for S.Y. 2026-2027[cite: 3]. This project covers Pandas DataFrames slicing, indexing, and filtering operations using the `cars.csv` dataset.

---

## A. POSITIONAL AND LABEL-BASED SLICING

Load the `cars.csv` dataset into a Pandas DataFrame named `cars`. Extract the specified subset of rows and display selected columns using positional indexing (`.iloc`) and label-based indexing (`.loc`).

The functions and methods used in this problem:
* **`pd.read_csv()`**: Reads a comma-separated values (CSV) file into a Pandas DataFrame (`cars`).
* **`.shape`**: Attribute that returns the dimensional shape (rows, columns) of the DataFrame (`(32, 12)`).
* **`.columns`**: Attribute that returns the column labels of the DataFrame.
* **`.iloc[]`**: Integer-location based indexing used to extract specific rows by index position (`[0, 6, 7, 8, 9, 10]`).
* **`.loc[]`**: Label-location based indexing used to select specific rows along with specified column labels (`['Model', 'mpg', 'hp', 'gear']`).

---

## B. MODEL LOOKUP

Perform conditional filtering on the `cars` DataFrame to look up specific car models and retrieve specified attributes.

The functions and methods used in this problem:
* **Boolean Comparison Operator (`==`)**: Evaluates a boolean mask matching specified strings in the `Model` column.
* **`.loc[]` filtering**: Extracts complete row entries matching the condition (e.g., retrieving all details for `'Toyota Corolla'`).
* **Combined `.loc[]` conditional & column selection**: Filters the row for `'Pontiac Firebird'` while simultaneously selecting specific output columns (`['Model', 'mpg', 'hp', 'wt']`).

---

## C. MULTI-MODEL SUBSETTING

Extract a specific subset of multiple car models using logical conditions and filter down to key performance metrics.

The functions and methods used in this problem:
* **Bitwise OR Operator (`|`)**: Combines multiple boolean conditions to filter rows matching `'Datsun 710'`, `'Lotus Europa'`, or `'Ferrari Dino'`.
* **`.loc[]` subsetting**: Selects specific attributes (`['Model', 'mpg', 'cyl', 'hp', 'gear']`) for the filtered models.
* **`.shape`**: Confirms the output dimensions of the resulting subset DataFrame (`(3, 5)`).

---

Thank you for reading!  
To see the main Python notebook for Programming Assignment 3, click this link: https://github.com/elija-png/ECE2112_PA3/blob/main/ECE2112_PA3.ipynb

---
