---
layout: post
title: Complexity classes 
subtitle: A short guide to hard problems by Kevin Hartnett
tags: [magazine,computer,science]
---

What's easy for a computer to do, and what’s almost impossible? Those questions form the core of
computational complexity.
![Complexity classes](https://d2r55xnwy6nx47.cloudfront.net/uploads/2018/07/Problem_classes_2880lede-2880x1010.jpg)

| Class | Stands for | What reseachers want to know?
| :--- | :--- | :--- |
| P | Polynomial | Is P same as NP? |
| NP | Nondeterministic P | P=NP? |
| PH | P Hierarchy | PH is different form P? |
| PSPACE | P Space | Is PSPACE different from P? |
| BQP | Bounded-error Quantum P | BQP is contained in NP? |
| EXPTIME | Exponential Time | PSPACE doesn't contain EXPTIME |
| BPP | Bounded-error Probabilistic P | BPP=P? |

** Polynomial time **
Algorithms in P must stop and give the right answer in at most n<sup>c<\sup> time where n is
the length of the input and c is some constant.
  
** Nondeterministic Polynomial **
A problem is in NP if, given a “yes” answer, there is a short proof that establishes
the answer is correct. If the input is a string, X, and you need to decide if the answer is “yes,” then a
short proof would be another string, Y, that can be used to verify in polynomial time that the answer
is indeed “yes.” (Y is sometimes referred to as a “short witness” — all problems in NP have “short
witnesses” that allow them to be verified quickly.)

** Polynomial Hierarchy **
PH contains problems with some number of alternating “quantifiers” that make
the problems more complex. Here’s an example of a problem with alternating quantifiers: Given X,
does there exist Y such that for every Z there exists W such that R happens? The more quantifiers a
problem contains, the more complex it is and the higher up it is in the polynomial hierarchy.

** Polynomial Space **
In PSPACE you don’t care about time, you care only about the amount of memory
required to run an algorithm. Computer scientists have proven that PSPACE contains PH, which
contains NP, which contains P.

** Bounded-error Quantum Polynomial **
All problems that can be solved in polynomial time by a quantum computer.

** Exponential Time **
EXP contains all the previous classes — P, NP, PH, PSPACE and BQP. Researchers
have proven that it’s different from P — they have found problems in EXP that are not in P.

** Bounded-error Probabilistic Polynomial **
BPP is exactly the same as P, but with the difference that the algorithm is allowed
to include steps where its decision-making is randomized. Algorithms in BPP are required only to
give the right answer with a probability close to 1.



