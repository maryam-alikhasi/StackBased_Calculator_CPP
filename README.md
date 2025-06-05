# StackBased_Calculator_CPP

A command-line stack-based calculator implemented in C++ using object-oriented design. This calculator supports mathematical expressions involving operators, constants (π and e), parentheses, and includes factorial and power computations.

---

## Features

- Stack-based expression evaluation
- Supports the following operators:
  - Addition (`+`)
  - Subtraction (`-`)
  - Multiplication (`*`)
  - Division (`/`)
  - Power (`^`)
  - Factorial (`!`)
- Recognizes constants:
  - Pi (`PI` or `-PI`) → 3.14 / -3.14
  - e (`e` or `-e`) → 2.71 / -2.71
- Handles parentheses correctly
- Basic error handling:
  - Invalid expression format
  - Mismatched parentheses
  - Division by zero

---

## Sample Usage

```

Input:
3+4\*2/(1-5)^2^3

Output:
1 - 5 = -4
2 ^ 3 = 8
-4 ^ 8 = 65536
4 \* 2 = 8
8 / 65536 = 0.00012207
3 + 0.00012207 = 3.00012207
Result: 3.00012207

````


## How It Works

1. **Stacks Used**:
   - Stack for operators
   - Stack for operands
2. **Expression Conversion**:
   - The infix expression is converted into postfix using operator precedence.
3. **Evaluation**:
   - The postfix expression is then evaluated using a stack.

---

## File Structure

- `main.cpp` — Main source file including all logic for stack, expression parsing, and evaluation.

---


### Prerequisites

- A C++ compiler (`g++`, `clang++`, or MSVC)

### Compile

```bash
g++ main.cpp -o Calculator
````

### Run

```bash
./Calculator
```