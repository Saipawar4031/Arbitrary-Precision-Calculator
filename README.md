🧮 Arbitrary Precision Calculator (APC)

A command-line Arbitrary Precision Calculator developed in C to perform arithmetic operations on very large integers beyond the limits of standard C data types. The project uses a doubly linked list to represent numbers and supports addition, subtraction, multiplication, and division.

📑 Table of Contents

- "Project Description" (#-project-description)
- "How to Run" (#-how-to-run)
- "How It Works" (#-how-it-works)
- "Flowchart" (#-flowchart)
- "Project Structure" (#-project-structure)
- "Input / Output" (#-input--output)
- "Module Details" (#-module-details)
- "Limitations" (#-limitations)
- "Concepts Used" (#-concepts-used)
- "Author" (#-author)

---

📌 Project Description

Standard C data types such as "int", "long", and "long long" have fixed storage limits. This project overcomes those limits by implementing custom arithmetic algorithms for large integers.

The digits of each number are stored in a linked-list-based data structure, allowing calculations to be performed digit by digit without storing the entire number in a standard integer variable.

The project is divided into multiple C source files to keep the arithmetic operations and supporting functions organized.

🚀 How to Run

1. Clone the Repository

git clone https://github.com/Saipawar4031/Arbitrary-Precision-Calculator.git

2. Navigate to the Project Directory

cd Arbitrary-Precision-Calculator

3. Compile the Program

Use the provided Makefile:

make

4. Execute the Program

If the Makefile generates an executable named "result.exe", run:

./result.exe 123456789 x 987654321

Example:

Input:
./result.exe 123456789 x 987654321

Output:
121932631112635269

Note: The executable name and command-line syntax must match your actual implementation. The example above illustrates the expected style of execution.

⚙️ How It Works

The calculator represents large integers using a doubly linked list. Each node stores a digit, and the links allow traversal through the number.

The general execution process is:

1. Input Processing: Accepts two operands and an arithmetic operator.
2. Number Representation: Converts the operands into the linked-list representation.
3. Operation Selection: Identifies the requested arithmetic operation.
4. Arithmetic Calculation: Calls the corresponding arithmetic function.
5. Result Generation: Processes the digits and calculates the result.
6. Output: Displays the final answer.

Supported Arithmetic Operations

Operator| Operation| Description
"+"| Addition| Adds two large integers.
"-"| Subtraction| Subtracts one integer from another.
"x"| Multiplication| Multiplies two large integers.
"/"| Division| Divides one integer by another.

🔄 Flowchart

flowchart TD
    A([Start]) --> B[Read operands and operator]
    B --> C[Convert operands into linked lists]
    C --> D{Select operation}
    D -->|+| E[Addition]
    D -->|-| F[Subtraction]
    D -->|x| G[Multiplication]
    D -->|/| H[Division]
    E --> I[Generate result]
    F --> I
    G --> I
    H --> I
    I --> J[Display result]
    J --> K([End])

📂 Project Structure

Arbitrary-Precision-Calculator/
│
├── APC_header.h       # Header file and function declarations
├── calculator.c       # Main program and operation handling
├── inserting_fun.c    # Linked-list insertion and utility functions
├── add_fun.c          # Addition implementation
├── sub_fun.c          # Subtraction implementation
├── mul_fun.c          # Multiplication implementation
├── division_fun.c     # Division implementation
├── makefile           # Build configuration
└── README.md          # Project documentation

🖥️ Input / Output

Example 1: Addition

Command:

./result.exe 123456789 + 987654321

Output:

1111111110

Example 2: Subtraction

Command:

./result.exe 1000000000 - 1

Output:

999999999

Example 3: Multiplication

Command:

./result.exe 123456789 x 987654321

Output:

121932631112635269

Example 4: Division

Command:

./result.exe 100 / 5

Output:

20

These examples illustrate the intended command-line interface. Verify the exact syntax, output formatting, and supported cases against your source code.

🧩 Module Details

1. "calculator.c"

- Contains the main program.
- Processes the operands and arithmetic operator.
- Selects the appropriate arithmetic function.
- Displays the calculated result.

2. "APC_header.h"

- Contains shared declarations and definitions.
- Declares the data structures used by the calculator.
- Provides function declarations for the different modules.

3. "inserting_fun.c"

- Implements linked-list insertion and supporting operations.
- Helps construct the linked-list representation of numbers.

4. "add_fun.c"

- Implements addition of large integers.
- Handles digit-wise addition and carry propagation.

5. "sub_fun.c"

- Implements subtraction of large integers.
- Handles borrowing and the order of operands as required.

6. "mul_fun.c"

- Implements multiplication of large integers.
- Uses the multiplication algorithm defined in the source code.

7. "division_fun.c"

- Implements division of large integers.
- Calculates the quotient according to the implemented algorithm.

8. "makefile"

- Defines the compilation process.
- Builds the program from its source files.
- Simplifies recompilation after source changes.

⚠️ Limitations

The following cases should be verified against the current implementation:

- Division by zero must be handled safely.
- Invalid operators and malformed inputs may require additional validation.
- Negative-number handling depends on the implemented arithmetic logic.
- Division may return an integer quotient without a fractional part.
- Memory allocation failures should be checked to prevent unexpected behavior.

🧠 Concepts Used

- C programming
- Doubly linked lists
- Structures and pointers
- Dynamic memory allocation
- Digit-wise arithmetic algorithms
- Carry and borrow handling
- Modular programming
- Header files and function declarations
- GCC compilation and Makefiles

👨‍💻 Author

Sai Pawar

B.E. Mechatronics Engineering

- GitHub: "@Saipawar4031" (https://github.com/Saipawar4031)
- Project Repository: "Arbitrary Precision Calculator" (https://github.com/Saipawar4031/Arbitrary-Precision-Calculator)

---

⭐ If you find this project useful, consider giving the repository a star!