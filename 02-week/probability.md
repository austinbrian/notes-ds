# Intro to Probability and Interdependence
------
## Probability
**Experiment** - procedure that can be repeated infinitely many times and has a well-defined set of outcomes
..* **Event**: Any collection of outcomes from an experiment
..* **Sample space**: Set of all possible outcomes from an experiment

*Ex:* Flipping a coin twice
..**Event**: two results of coins
..**Sample space**: {{H,H},
..                   {H,T},
..                   {T,H},
..                   {T,T}}

## Sets
A set is a well-defined collection of distinct objects.
  * Can't have duplicates in a set
  * It's convenient to create a set in python:
  * `set(somelist)` = unique items in "somelist"

### Union
*A* ∪ *B* = the set of elements in *A* **OR** *B*

### Intersection
*A* ∩ *B* = the set of elements in *A* **AND** *B*

*A* = {2,4,6,8}
*B* = {2,3,5,7}

*A* ∪ *B* = {2,3,4,5,6,7,8}
*A* ∩ *B* = {2}

The non-intersection is called the **complement**.
*P(A^c)* = 1 - *P(A)*

## Probability Basics
For event *A* the probability that A occurs is:
.... *P(A)* =  number of outcomes in *A* / number of all possible outcomes

## Probability Rules
*P/(A|B)* = (*P(A ∪ B)*)/(*P(B)*)
Note: *A|B* means “*A* given *B*” or “*A* conditional on the fact that *B* happens.”

Probability practice
1. Find US birth results in twin females (.5*.66*(1/90))
2. Find US birth results in identical twin females (.5*.66*(1/90) * .333)
Assumption is that US twin prevalence is the same as global twin prevalence

Fraternal twins = .25 both female, .25 both male
Identical twins = .5 both female
All twins = .333 identical

## Independence
*P(A*∩*B)* = *P(A|B)P(B)*
Making the assumption that *P(A)* is equal to *P(A|B)* can cause huge problems, since it assumes that the two probabilities are independent.

Areas where independence is important:
* Considering joint probabilities
* Most modeling techniques
* Sampling without replacement
* Training/testing sets
