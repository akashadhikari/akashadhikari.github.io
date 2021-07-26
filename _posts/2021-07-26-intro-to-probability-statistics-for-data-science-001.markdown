---
layout: post
title:  "Intro to Probability: Statistics for Data Science"
date:   2021-07-26 06:33:06 +0545
categories: machinelearning
---

### The Fundamental Counting Rules

Let A and B are two questions that can be solved by 2 methods and 3 methods respectively. In how many ways A or B (at least one of them) can be solved?

Answer: 2 methods from A and 3 methods from B, i.e 5 ways.

John is assembling a computer. He has a choice of chips from 2 brands, a hard drive from 4 brands, a memory from 3, and an accessory bundle from 5 local stores. How many different ways can John order the parts?

Answer: 2*4*3*5 = 120 different ways

A test contains 20 questions each having 4 choices. If there is only one right answer to each question, in how many ways can a student mark the test paper?

Answer: 4 possibilities from the first question * 4 from the second * 4 from the third... (up to 20 times) = 4^20 possibilities

The first problem defines the Sum Rule and the remaining two comprise the Product Rule.

### Permutation and Combination

In the simplest of words, permutation means to *arrange* and combination means to *select*.

Consider three letters A, B, and C. The permutations of three letters taken two at a time will be AB, BC, CA, AC, CB, and BA. The order matters in this case. While in the case of combination, the result will be AB, BC, and CA.

![permutation-combination](/assets/permutation-combination.png){:class="img-responsive"}

A **permutation** of given things or elements or objects is an arrangement of these things in a row in some order.

The total number of permutations of a set of *n* different objects selected *r* at a time without repetition denoted by P(n,r) or *nPr*  is defined as:

P(n,r) = n(n-1)(n-2) ... (n-r+1)

In factorial notation, P(n,r) = n!/(n-r)!  where (n≥r). It also holds true for r=0.

A **combination** of given things means any selection of one or more things without regard to order.

The number of combinations of n different objects, taken r at a time (without repetition) is:

C(n,r) = P(n,r)/r! = n(n-1)(n-2)...(n-r+1)/r!

In factorial notation, C(n,r) = n!/r!(n-r)! where n≥r.

### Event

The outcome or a set of outcomes of an activity is called an event.

For example, while rolling a die, getting the outcome in the form of odd number E={1,3,5}; went number E={2,4,6}, getting the prime numbers, etc. are events.

**Exhaustive Cases or Events:** It includes all possible outcomes of a random experiment. For example:

In flipping a coin once, S={H,T} and exhaustive cases = 2^1 = 2.

In flipping a coin twice, S={HH,HT,TH,TT} and exhaustive cases = 2^2 = 4.

In rolling a die once, S={1,2,3,4,5,6} and exhaustive cases = 6^1 = 6.

In rolling a die twice, exhaustive cases = 6^2 = 36.

**Exhaustive (partition) set of events:** A set of disjoint events E1, E2, ..., En is collectively said to be an exhaustive set of events if the union of these events is the sample space S. For example, in rolling a die, E1 = {1,3,5} and E2={2,4,6} are exhaustive events because of E1 U E2 = S.

**Favorable cases or events:** The number of outcomes of a random experiment that describe the possible set of actual outcomes is called favorable cases to the event. In a pack of cards, the number of favorable cases of a king is 4, and the black card is 26. In rolling a die once, the number of favorable cases of getting an event number is 3.

### Types of Events

**Simple and compound events:** Simple (elementary) events cannot be broken down further whereas compound (composite) events consist of more than one outcome. For example, while rolling a die, the event of getting 1 is simple whereas the event f getting an even number is composite. 

**Mutually exclusive or Incompatible events:** Two or more events are said to be mutually exclusive (or **disjoint events** or **incompatible events**) if the happening of any one event excluded the happening of another event. For example, in a coin-toss experiment, either H or a T occurs at a time but not both. Likewise, in a die-roll experiment if the events are A = {1,3,5}, B= {2,4,6} and C = primes = {2,3,5}, A and B are mutually exclusive but A and C are not.

**Equally like or mutually symmetric events:** Two or more events are said to be equally likely  (or equiprobable) events if all the events have an equal chance of occurrence. If a fair die is rolled all the outcomes 1,2,3,4,5,6 are equally likely.

**Independent events:** Events are said to be independent of each other if the occurrence of any one of them does not affect and is not affected by the occurrence or non-occurrence of the other. If two coins are tossed together, the occurrence of the head or tail on the first coin does not affect the result of the second coin.

**Dependent events:** Contrastingly, if the occurrence of one event affects the outcomes of the other then the event is said to be dependent. If a second card is drawn from a pack of cards without the replacement of the first card, then the outcome of the second instance is affected.

**Complementary events:** Any two events are said to be complementary (or complement of each other) if (i) they are mutually exclusive and (ii) they are collectively exhaustive.

**Equal events:** Two events are said to be equal if A ⊂ B and B ⊂ A, This statement implies that all the points of A are also the points of B and vice-versa.

**Derived events:** For two events A and B, the event A or B i.e A ∪ B  is a derived event.

{% include share-bar.html %}