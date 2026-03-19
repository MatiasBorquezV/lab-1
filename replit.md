# Data Structures Lab - Lists and Stacks (C)

## Project Overview
An educational C programming laboratory where students implement data structure functions for Lists and Stacks (TDAs).

## Tech Stack
- **Language:** C
- **Compiler:** gcc (with `-g -Wall -Werror` flags)
- **Build:** Custom shell script (`test.sh`)
- **Debugger:** gdb (for crash analysis)

## Project Structure
- `exercises.c` — Student implementation file (exercises to be completed)
- `arraylist.c` / `arraylist.h` — Generic ArrayList/List TDA implementation
- `stack.h` — Stack TDA built on top of List
- `test.c` — Test suite for validating exercises
- `test.sh` — Build and test runner script; also handles git commits

## Workflow
- **Start application**: `bash test.sh` (console output)
  - Compiles `test.c` with gcc
  - Runs test suite and shows pass/fail results
  - Optionally pushes progress to GitHub

## Exercises
1. **crea_lista** — Create a list with integers 1-10
2. **sumaLista** — Sum all integers in a list
3. **eliminaElementos** — Remove all occurrences of a value from a list
4. **copia_pila** — Copy a stack to another maintaining order
5. **parentesisBalanceados** — Check if bracket string is balanced using a stack

## Notes
- Tests start at `total_score: 0/70` because exercise functions are intentionally empty stubs for students to implement.
- The `test.sh` script tracks changes via `git diff` and only recompiles when `exercises.c` changes.
