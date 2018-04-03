# CHAPTER 1: PRELIMINARIES

Short summary goes here.

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

Other criteria include: portability, generality, well-definedness 




## 1.4 - Influences on Language Design

## 1.5 - Language Categories

## 1.6 - Language Design Trade-Offs

## 1.7 - Implementation Methods

## 1.8 - Programming Environments
