# Task #1: List Manipulation Program

## Overview

This Java project demonstrates advanced list manipulation techniques, including:

- **Initializing** predefined lists of integers and strings.
- **Mapping** integer values to string indices with a custom formula.
- **Dynamically populating** a third list based on computed indices.
- **Controlled removal** of elements from the third list until a target size is reached.
- **Printing** the final contents to standard output.

The core logic resides in the `Task1` class within the package `oop.mid2.t1`.

---

## Project Structure


- **`Task1.java`**: Contains the `Task1` class and `main` method implementing the program logic.  
- **`README.md`**: This file, providing an overview and usage instructions.

---

## Detailed Description

1. **List Initialization**  
   - `list1`: A hard-coded list of 12 integers: `[6, 5, 3, 5, 5, 3, 3, 5, 7, 6, 4, 5]`.  
   - `list2`: A hard-coded list of 18 unique strings: e.g., `"PqH", "F5W", "nQ6", ...`.

2. **Populating `list3`**  
   - For each integer `n` in `list1`, compute an index into `list2` using the formula:  
     ```
     index = (n * 2) - 1
     ```  
   - If the index is within bounds, add the corresponding string from `list2` to `list3`. Otherwise, log a warning.  
   - After processing all 12 integers, `list3` contains 12 strings.

3. **Reducing `list3`**  
   - Define a **target size** of 6 elements.  
   - Remove elements from `list3` one at a time at increasing indices:  
     - First remove at index 0, then at index 1 of the updated list, then index 2, and so on, until only 6 strings remain.

4. **Output**  
   - Print the header:  
     ```
     Final 6 strings in list3:
     ```  
   - Print each of the remaining strings on a new line.

---

## Usage

### From the Command Line

```bash
# Navigate to the project root (where README.md and src/ reside)
javac src/oop/mid2/t1/Task1.java
java -cp src oop.mid2.t1.Task1
## 📸 Screenshot

![Program Screenshot](screenshots/midtermsreenshot.png)