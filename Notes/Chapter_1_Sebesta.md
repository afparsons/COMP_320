# CHAPTER 1: PRELIMINARIES
****
https://www.youtube.com/watch?v=nV1HAbGvQMA
****
## 1.1 - Reasonsfor Studying Concepts of Programming Languages

Studying programming language concepts improves or increases:

- capacity to express ideas
  - you can borrow concepts from language A and simulate them in language B
- background for choosing appropriate languages
  - > Many programmers, when given a choice of languages for a new project, use the language with which they are most familiar, even if it is poorly suited for the project at hand. If these programmers were familiar with a wider range of languages and language constructs, they would be better able to choose the language with the features that best address the problem.
  - better to use an integrated/native feature than try and simulate
- ability to learn new languages
- understanding the significance of implementation
- use of programming languages already known
- overall advancement of computing

## 1.2 - Programming Domains

**Scientific Applications:** efficiency is the primary concern. Fortran is still largely used.

**Business Applications:** COBOL. Precise arithmetic, decimal operations, ability to produce elaborate reports.

**Artificial Intelligence:** LISP, Scheme, C, Prolog. Flexibility is important.

**Web Software:** dynamic content. JavaScript, PHP, HTML/CSS, etc.

## 1.3 - Language Evaluation Criteria

**Readability:** especially important for code maintenance

1. Overall Simplicity
  - languages with many basic constructs are harder to learn than those with fewer. Some programmers will only learn a 'relevant subset' of the basics.
    - This is problematic when a programmer with partial knowledge must work with code written by a programmer who had a different set of partial knowledge.
  - *feature multiplicity:* more than one way to accomplish a particular operation
  - *operator overloading:*  a single operator symbol has more than one meaning
    - ```+``` does integer AND floating point addition
    - pros and cons
2. Orthogonality
  - small set of primitive constructs can be combined in a small number of ways to build the control and data structures of the language
  - *from class:* related to operator overloading.


3. Data Types
  - give clarity
  - Ex: ```timeOut = 1``` vs. ```timeOut = true``` <-- the latter is clearer
4. Syntax Design
  - *Special Words:* words like ```while```, ```class```, and ```for```
    - statement groups can be confusing
    - special words ought not be legal variable names
  - *Form and meaning:* the semantics of words is important
    - Ex: UNIX ```grep``` means very little without an understanding of its background

**Writability:** a measure of how easily a language can be used to create programs for a chosen problem domain. Related to *Readability*.

1. Simplicity and Orthogonality
  - if a language has a large number of different constructs, some programmers might not be familiar with all of them.
    - leads to misuse of some features and disuse of other (more elegant) features
      - even unknowningly using features is possible! Leads to 'weird errors'
2. Expressivity

**Reliability:** a program is said to be *reliable* if it performs to its specifications under all conditions.

1. Type Checking
  - simply testing for type errors (compile-time checking is preferred)
2. Exception Handling
  - ability of a program to intercept run-time errors, take corrective measures, and then continue
3. Aliasing
  - having two or more distinct names in a program that can be used to access the same memory cell (DANGEROUS)
4. Readability and Writability
  - influence reliability

**Cost:**
  - cost of training. More complexity --> harder to learn --> higher cost
  - cost of writing. Easy writability --> lower costs
  - cost of compiling.
  - cost of executing programs. Many run-time checks required prohibits fast code execution.
    - *optimization:* techniques that compilers may use to decrease the size and/or increase the execution speed of code.
  - cost of implementation.
  - cost of poor reliability.
  - cost of maintenance. Dependant on reliability. 2x-4x cost of development.

Other criteria include: portability, generality, well-definedness.

## 1.4 - Influences on Language Design

**Computer Architecture:** imperative languages are designed around von Neumann architecture.

- Central features:
  - *variables* model memory cells.
  - *assignment statements*
  - *iteration*
- functional languages are different but could potentially be superior if executed on non-von Neumann architecture

**Programming Design Methodologies:**

- lol wut. lots of words I don't yet understand.

## 1.5 - Language Categories

**imperative**

**functional**

**logic**

**object-oriented**

## 1.6 - Language Design Trade-Offs

**Reliability vs. Cost of Execution**

**Writability vs. Readability**

## 1.7 - Implementation Methods

Primary components of a computer:

- *Internal memory:* stores programs and data
- *Processor:* collection of circuits that provices a realization of a set of primitive operations (arithmetic and logic operations)

Theoretically, a computer could be designed and built with a particular high-level language as its machine language, but it would be *very* complex and expensive.
It would also be highly inflexible.

**Compilation:** programs are translated into machine language, which can be executed directly on the computer.

- *Advantage:* very fast program execution once the translation process is complete.

- *Disadvantage:* must translate the high-level code (time consuming). Subject to the von Neumann bottleneck.

**Pure Interpretation:** programs are interpreted by an interpreter with no translation whatsoever. The interpreter acts as a software simulation of a machine whose fetchexecute cycle deals with high-level language statements rather than machine instructions.

- *Advantage:* easy implementation of many source level debugging operations, because all run-time errors refer to source-level units.

- *Disadvantages:* 10x-100x slower than compiled languages because of statement decoding. More space required.

**Hybrid Implementation Systems:** translate high-level language programs to an intermediate language designed to allow for easy interpretation. This method is faster than pure interpretation because the source language statements are decoded only once.

Just-in-Time compilation

**Preprocessors:**

:P

## 1.8 - Programming Environments

:P

## Notes from Class

### 4 April 2018

- Machine Language (binary)
- Assembly Language (basic operations like ADD)
  - over time, developed macros/pseudo instructions
- Fortran
  - similar to Assembly in that it is:
    - imperative
    - von Neumann
    - state driven
- Slow evolution to higher abstraction
  - Algol (1960)
  - Pascal (1970)
  - C (1972)
  - Simula (1969)
  - Smalltalk (1980)

Object Oriented

Event Driven
- set up code to respond to events
- write the event responses
- no "linear" control flow
- control-flow is riven by events (user or system events)

Functional Language (LISP 1959)
- based on mathematical functions and lambda calculus
- Key ideas
  - functions as 1st class entities
  - **no state**
  - atoms and lists
  - functions and data have the same form (how?)
  - later developed into Scheme
- ML and Haskell

Declarative Languagess

Scripting Languages

Visual Languages

****

Terms to review (gosh my brain is dusty)
- plymorphism
- message-passing
- dynamic-binding
- single-entry/single-exit
- data abstraction
- inheritence
- 1st class entities


| | Assembly |
|-|-|
|1| Put data 1 in ACC |
|2| Add data 2 to ACC |
|3| Move ACC to data 3|

### 6 April 2018

Scheme: Interpreted language
- infinite loop waiting to read a statement, evaluate it, and write the result
  - read a list
  - EVAL function
  - display the result
- Primitive functions:

Expression vs. statements

functional

side-effects
