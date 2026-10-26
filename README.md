# 🧮 Arbitrary Precision Calculator (APC)

A command-line **Arbitrary Precision Calculator** developed in C to perform arithmetic operations on large integers beyond the limits of standard C data types.

## 📌 Project Description

Standard C data types such as `int`, `long`, and `long long` can store only numbers within a fixed range. This project addresses that limitation by implementing custom arithmetic operations for large integers.

The calculator uses linked-list-based data structures to represent and process large numbers. It supports arithmetic operations such as addition, subtraction, multiplication, and division.

## 📂 Project Structure

```text
Arbitrary-Precision-Calculator/
│
├── APC_header.h       # Header file and declarations
├── calculator.c       # Main calculator logic
├── add_fun.c          # Addition operations
├── sub_fun.c          # Subtraction operations
├── mul_fun.c          # Multiplication operations
├── division_fun.c     # Division operations
├── inserting_fun.c    # Insertion and related list operations
├── makefile           # Build configuration
└── README.md          # Project documentation
```

## 🚀 Installation and Execution

### 1. Clone the Repository

```bash
git clone https://github.com/Saipawar4031/Arbitrary-Precision-Calculator.git
```

### 2. Navigate to the Project Directory

```bash
cd Arbitrary-Precision-Calculator
```

### 3. Compile the Project

Use the provided Makefile:

```bash
make
```

### 4. Run the Program

On Linux or WSL, execute the generated program. If the executable is named `result`, run:

```bash
./result
```

On Windows, if the executable is named `result.exe`, run:

```powershell
.\result.exe
```

**Note:** The executable name depends on the target defined in the Makefile.

## 🧠 How It Works

The calculator represents large integers using linked-list-based data structures and processes them through separate arithmetic functions.

1. **Input:** Accepts the numbers and the requested arithmetic operation.
2. **Representation:** Stores the numbers using the linked-list structure.
3. **Calculation:** Performs the selected arithmetic operation.
4. **Output:** Displays the calculated result.

### Arithmetic Operations

- **Addition:** Adds two large integers.
- **Subtraction:** Subtracts one large integer from another.
- **Multiplication:** Multiplies large integers.
- **Division:** Divides large integers.

## 👨‍💻 Author

**Sai Pawar**

B.E. Mechatronics Engineering | Embedded Systems & Robotics Enthusiast

- **GitHub:** [@Saipawar4031](https://github.com/Saipawar4031)
- **Project Repository:** [Arbitrary Precision Calculator](https://github.com/Saipawar4031/Arbitrary-Precision-Calculator)

---

⭐ If you find this project useful, consider giving the repository a star!
