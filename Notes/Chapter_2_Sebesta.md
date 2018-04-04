# CHAPTER 2: EVOLUTION OF THE MAJOR PROGRAMMING LANGUAGES
****
Summary goes here.
****
## 2.1 - Zuse's Plankalkül

Designed in 1945 for the Z4. Never implemented and only published in 1972.

Featured: arrays, records, twos-complement floating point and hidden bit, "for", many algorithms.

## 2.2 - Pseudocodes

*Not 'pseudocode' in the contemporary sense!*

During the 1940s and 1950s, programs were written in machine language. This was cumbersome.

**Short Code**

The primary means of programming the UNIVAC. Implemented via an interpreter. 50x slower than machine code.

**Speedcoding**

Developed for the IBM 701 to support floating point.

**The UNIVAC "Compiling" System**

Expanded pseudocode into machine code subprograms in the same way as macros are expanded into assembly language.

## 2.3 - The IBM 704 and Fortran

The IBM 704 had both indexing and floating-point instructions in hardware. Programmers needed a language that could take advantage of this.

The first widely accepted compiled high-level language was Fortran.

- **Fortran 0:** Developmental vesion. Variables had 2 characters.
- **Fortran I:** April 1957.
  - Input/output formatting
  - 6 character variable names
  - user-defined subroutines
  - ```if``` selection
  - ```do``` loop statement
  - control statements based on IBM 704 instructions
  - no data typing
    - variables beginning with ```I, J, K, L, M, N``` were implicitly integers, and the remaining variables were floating points.
- **Fortran II:**  Spring 1958.
  - Bug-fixing
  - independant compilation of subroutines
- **Fortrans IV, 77, 90, 95, 2003, 2008:**
  - *IV:* AKA Fortran 66. Added specific type declarations, logical ```if``` construct, and ability to pass subprograms as parameters.
  - *77:* Added character string handling, logical loop control statements, and ```if-else```.
  - *90:* Added dynamic arrays, records, pointers, multiple selection statement, modules, recursion. Removed some deprecated parts.
  - *95:* blah
  - *2003:* OOP support and other stuff.
  - *2008:* blah

  **Evaluation:**
  - Types and storage of all variables are fixed before run-time. Sacrificed flexibility for simplicity and efficiency.

## 2.4 - Functional Programming: Lisp

**The Beginnings of Artificial Intelligence and List Processing:** The contraints of arrays and the need for linked lists was realized.

**Lisp Design Process:** 1958...needed a language to fit arithmetic requirements.

**Lisp Language:**
- 2 data structures: atoms and lists
  - atoms are symbols or numeric literals
  - lists: ```(A B C D)```, nested lists: ```(A (B C) D (E (F G) ) )```
- functional language
- simple syntax

**Scheme:**
- Dialect of Lisp from MIT ca. 1975.
- functions are first-class entities
  - can be assigned to variables, passed as paraeters, returned as values, and be the elements of lists.

**Common Lisp:** developed to unify various dialects and promote portability

## 2.5 - The First Step Toward Sophistication: ALGOL 60

## 2.6 - Computerizing Business Records: COBOL

## 2.7 - The Beginnings of Timesharing: Basic

## 2.8 - Everything for Everybody: PL/I

## 2.9 - Two Early Dynamic Languages: APL and SNOBOL

## 2.10 - The Beginnings of Data Abstraction: SIMULA 67

## 2.11 - Orthogonal Design: ALGOL 68

## 2.12 - Some Early Descendants of the ALGOLs

## 2.13 - Programming Based on Logic: Prolog

## 2.14 - History's Largest Design Effort: Ada

## 2.15 - Object-Oriented Programming: Smalltalk

## 2.16 - Combining Imperative and Object-Oriented Features: C++

## 2.17 - An Imperative-Based Object-Orientet Language: Java

## 2.18 - Scripting Languages

## 2.19 - The Flagship .NET Language: C#

## 2.20 - Markup-Programming Hybrid Languages
