# ICT 111 Student Grading System

A simple, menu-driven Python command-line application for registering students, assigning grades from marks, displaying student records, and reviewing class statistics.

## Features

- Add a student using a student number, name, and mark.
- Reject blank student numbers and names.
- Validate that marks are numeric and between 0 and 100.
- Assign a grade and performance decision automatically.
- Display all students registered during the current run.
- Calculate the class average, highest and lowest marks, and pass/fail counts.

## Grade scale

| Mark range | Grade | Decision |
| --- | --- | --- |
| 75–100 | A | Excellent |
| 65–less than 75 | B | Very good |
| 50–less than 65 | C | Good |
| 45–less than 50 | D | Pass |
| 0–less than 45 | F | Fail |

The class summary counts marks of **50 or higher** as passes and marks below 50 as fails. Consequently, a mark from 45 to less than 50 receives a D / “Pass” grade but is counted as a fail in the summary.

## Requirements

- Python 3
- A terminal or command prompt

The application uses only Python's standard library; no packages need to be installed.

## Getting started

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Run:

   ```bash
   python3 "grading system.py"
   ```

   On Windows, you can use:

   ```powershell
   py "grading system.py"
   ```

## Using the application

Choose an option from the menu:

1. **Add student** — enter a non-blank student number and name, then a mark from 0 to 100.
2. **Display all** — print every student registered in this run.
3. **Class summary** — show class statistics. This option displays a message if no students have been added.
4. **Exit** — close the application.

Invalid menu choices and invalid marks prompt for valid input.

## Data and limitations

Student records are stored in memory and are cleared when the program exits. The application does not currently save records to a file or database, prevent duplicate student numbers, or provide student record editing and deletion.

## Project structure

```text
.
├── grading system.py
└── README.md
```
