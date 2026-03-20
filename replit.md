# C ADT Lab Project

## Overview
This is a C programming laboratory for practicing Abstract Data Types (ADTs) — specifically **Lists** and **Stacks**. Students implement functions in `exercises.c` and run the test suite to check their work.

## Project Structure
- `exercises.c` — Student implementation file (where exercises are solved)
- `arraylist.c` / `arraylist.h` — List ADT implementation
- `stack.h` — Stack ADT (header-only, wraps the List ADT)
- `test.c` — Test suite with automated grading
- `test.sh` — Build + test runner script (also handles Git integration)
- `log` — Auto-generated log file tracking compilation and test results

## Build & Run
The project uses `gcc` to compile and a bash script to orchestrate testing:

```bash
bash test.sh
```

This will:
1. Detect changes to `exercises.c`
2. Recompile: `gcc -g test.c -Wall -Werror -o a.out`
3. Run tests and display results
4. Optionally push progress to GitHub (requires a PAT)

## Workflow
- **Name:** Start application
- **Command:** `bash test.sh`
- **Output type:** console (CLI tool, no web UI)

## Language & Tools
- **Language:** C (GCC 14)
- **Build:** gcc with `-Wall -Werror`
- **Testing:** Custom test runner in `test.c`
- **No frontend** — purely a command-line project
