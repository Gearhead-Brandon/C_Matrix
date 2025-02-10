# С_matrix Summary

## Overview
The **s21_matrix** project involves implementing a static library (`matrix.h`) in C for working with matrices. The library provides fundamental matrix operations, following structured programming principles and Google style guidelines.

## Key Features
- **Matrix Operations**:
  - Creation (`s21_create_matrix`), deletion (`s21_remove_matrix`), and comparison (`s21_eq_matrix`)
  - Addition (`s21_sum_matrix`), subtraction (`s21_sub_matrix`), and multiplication (`s21_mult_matrix`)
  - Scalar multiplication (`s21_mult_number`)
  - Transposition (`s21_transpose`)
  - Determinant calculation (`s21_determinant`)
  - Minor and algebraic complement calculation (`s21_calc_complements`)
  - Inverse matrix computation (`s21_inverse_matrix`)

- **Implementation Details**:
  - Uses a `matrix_t` struct (`double** matrix`, `int rows`, `int columns`)
  - Written in C (C11 standard) using `gcc`
  - Developed as a static library (`s21_matrix.a`)

- **Testing & Coverage**:
  - Unit tests with **Check** library
  - At least **80%** test coverage (verified with `gcov`)
  - `Makefile` with targets: `all`, `clean`, `test`, `s21_matrix.a`, `gcov_report`
  - `gcov_report` generates an HTML coverage report

## Additional Notes
- The project is inspired by mathematical principles and applications in computer graphics (e.g., Doom 3 shadow calculations).
- Matrices follow standard mathematical definitions (square, diagonal, triangular, identity, etc.).
- Floating-point calculations ensure up to **6 decimal places** of precision.