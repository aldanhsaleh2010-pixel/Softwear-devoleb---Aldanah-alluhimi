
# Class 15 Homework – Quiz Submission Error Handling

**Author:** Aldanah Saleh

## Overview
This notebook explores error handling in a quiz submission system, including student ID validation, failure classification, logging, and recovery strategies.

## Implemented Features
- Checks whether the student ID can be converted to an integer.
- Checks that the student ID contains exactly six characters.
- Removes spaces from the entered ID.
- Displays a success message or a validation error.

## Error Handling Design
The notebook describes how to handle two situations:

- **Deadline passed:** Reject the submission with a clear message and no retry.
- **Server fault:** Log the error, retry once, and offer a manual “Try again” option if the retry fails.

Suggested logs include a timestamp, request ID, and stack trace.

## Requirements
- Python 3
- Jupyter Notebook or Google Colab

## How to Run
1. Open `class_15_HW(1).ipynb`.
2. Run the student ID validation cell.
3. Enter your student ID when prompted.
4. Read the displayed result.

## Limitations
Database saving, deadline checking, logging, and retry handling are discussed but are not implemented in the revised function. Its success message confirms validation only, not an actual saved submission.

## Key Lesson
A system should never report success when an operation has failed.
