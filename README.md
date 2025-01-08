# Compiler-design

Welcome to the Compiler-design repository! This repository contains a collection of LEX and YACC programs, designed to illustrate various concepts in Compiler Design. Each program folder includes source code and corresponding output files to help you understand the results.

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Programs Overview](#programs-overview)
4. [How to Run](#how-to-run)
5. [File Structure](#file-structure)
6. [Contributing](#contributing)
7. [License](#license)

## Introduction

This repository is a comprehensive collection of LEX and YACC programs aimed at demonstrating key concepts in Compiler Design. It is intended for students, educators, and enthusiasts who want to explore lexical analysis, parsing, and automata theory in a practical way. The repository includes examples that run seamlessly on Windows and macOS.

## Prerequisites

To run the programs, ensure you have the following installed:

- A LEX compiler (e.g., `flex`)
- A YACC compiler (e.g., `bison`)
- A terminal or command-line interface
- Basic knowledge of Compiler Design concepts

## Programs Overview

The repository includes the following programs:

1. Program 01: LEX code for counting the number of lines, spaces, tabs, and other characters.
2. Program 02: LEX code to identify and print valid identifiers in C/C++.
3. Program 03: LEX code to identify and print integer and float values.
4. Program 04: LEX code for tokenizing C code.
5. Program 05: LEX code to count characters, words, and white spaces in an input file.
6. Program 06: LEX code to replace multiple whitespaces with a single space.
7. Program 07: LEX code to remove comments from C programs.
8. Program 08: LEX code to extract HTML tags from an input HTML file and store them in a text file.
9. Program 09: Implementation of a DFA accepting even numbers of 'a' and 'b' with a dead state.
10. Program 10: DFA in LEX code that accepts strings where the third last element is 'a'.
11. Program 11: DFA in LEX code to identify and print integer, float constants, and identifiers.
12. Program 14: YACC-LEX code for converting infix expressions to postfix expressions.
13. Program 15: YACC-LEX code for a desk calculator.

Each folder includes:
- Source code (`programXX.l` or `programXX.y`)
- Sample input files (if applicable)
- Output screenshots (`Output.png`)

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Compiler-design.git
   ```

2. Navigate to the program folder:
   ```bash
   cd Compiler-design/ProgramXX
   ```

3. Compile the LEX file:
   ```bash
   flex programXX.l
   gcc lex.yy.c -o programXX
   ./programXX < input.txt  # If applicable
   ```

   For YACC programs:
   ```bash
   yacc -d programXX.y
   lex programXX.l
   gcc y.tab.c lex.yy.c -o programXX
   ./programXX
   ```

4. View the output as specified in the program folder or refer to `Output.png`.

## File Structure

The repository structure is as follows:

```
Compiler-design/
├── Program 01/
│   ├── program01.l
│   ├── input.txt
│   ├── Output.png
├── Program 02/
│   ├── program02.l
│   ├── input.txt
│   ├── Output.png
├── Program 03/
│   ├── program03.l
│   ├── input.txt
│   ├── Output.png
... (and so on for each program)
```

## Contributing

Contributions are welcome! If you have additional examples, bug fixes, or improvements, please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Note: The repository includes output screenshots (`Output.png`) for most programs to help visualize the results. For detailed outputs, refer to the respective program folders.
