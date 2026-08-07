# PrepTrack — Placement Preparation Performance Analyzer

## Project Overview

PrepTrack is a Python console application that analyzes a student's placement preparation performance. The program collects student details, attendance, project completion status, profile verification status, and seven daily coding practice scores. It validates the input, analyzes the student's performance, evaluates placement readiness, and displays the first major blocker along with the recommended next action.

---

## Features Implemented

- Student profile input
- Student name validation
- Attendance validation (0–100)
- Project completion validation (yes/no)
- Profile verification validation (yes/no)
- Seven-day coding practice processing
- Practice score validation
- Absent day handling using `continue`
- Strong, Satisfactory, Needs Improvement, and Critical score classification
- Attempted, absent, passed, and failed day counting
- Total score calculation
- Average score calculation
- Highest score detection
- Lowest score detection
- First critical score detection
- Placement readiness evaluation
- Final status generation
- Primary blocker identification
- Next action recommendation

---

## Python Concepts Used

- Variables
- Strings, Integers, Floats, Booleans
- `input()`
- `int()`
- `float()`
- Arithmetic Operators
- Assignment Operators
- Relational Operators
- Logical Operators
- Boolean Expressions
- `if`, `elif`, `else`
- Nested Conditions
- `while` Loops
- `for` Loop with `range()`
- `break`
- `continue`
- Counters and Accumulators
- f-Strings

---

## How to Run the Program

Clone the repository:

```bash
git clone https://github.com/chan-g-dev/preptrack-chanakya.git
```

Move into the project folder:

```bash
cd preptrack-chanakya
```

Run the program:

```bash
python main.py
```

or

```bash
python3 main.py
```

---

## Test Result Summary

| Test ID | Scenario | Expected Result | Actual Result | Status |
|---------|----------|-----------------|---------------|--------|
| TC-01 | All requirements satisfied | Ready for Mock Interview | Ready for Mock Interview | Pass |
| TC-02 | Critical score present | Critical Support Required | Critical Support Required | Pass |
| TC-03 | Fewer than six attempts | Practice Incomplete | Practice Incomplete | Pass |
| TC-04 | Fewer than four passed days | Insufficient Passed Practices | Insufficient Passed Practices | Pass |
| TC-05 | Average below 70 | Practice Improvement Required | Practice Improvement Required | Pass |
| TC-06 | Attendance below 75 | Attendance Improvement Required | Attendance Improvement Required | Pass |
| TC-07 | Graduation year not eligible | Graduation Criteria Not Met | Graduation Criteria Not Met | Pass |
| TC-08 | Project incomplete | Application On Hold | Application On Hold | Pass |
| TC-09 | Profile not verified | Application On Hold | Application On Hold | Pass |
| TC-10 | All practice days absent | Practice Not Evaluated | Practice Not Evaluated | Pass |
| TC-11 | Invalid score below -1 | Input rejected | Input rejected | Pass |
| TC-12 | Invalid score above 100 | Input rejected | Input rejected | Pass |
| TC-13 | Boundary value testing | Correct classifications | Correct classifications | Pass |
| TC-14 | Multiple blockers | First blocker displayed | First blocker displayed | Pass |

---

## Individual Contribution

**Name:** Chanakya

**Repository URL:**  
https://github.com/chan-g-dev/preptrack-chanakya

### My Main Contribution

Developed the complete PrepTrack console application according to the project requirements.

### Features I Implemented

- Student information collection
- Input validation
- Seven-day practice score processing
- Score classification
- Attendance and eligibility evaluation
- Highest and lowest score tracking
- First critical score detection
- Average score calculation
- Placement readiness evaluation
- Final report generation

### Python Concepts I Used

- Variables
- Boolean expressions
- Loops
- Conditional statements
- Counters and accumulators
- Input validation
- Arithmetic calculations

### Most Difficult Logic

Implementing the highest and lowest score tracking while ignoring absent practice days and displaying the first major blocker according to the required priority.

### Problem I Faced

Handling absent practice days without affecting calculations and preventing division by zero.

### How I Solved It

Used `continue` to skip absent days, initialized the highest and lowest scores using the first attempted score, and calculated the average only when at least one practice day was attempted.