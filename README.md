# Bayes_Thoerem

## Naive Bayes Definition
_Naive Bayes is a simple yet effective probabilistic classification algorithm based on Bayes' Theorem. It is commonly used in text classification tasks (e.g., spam detection, sentiment analysis) due to its efficiency and effectiveness with high-dimensional data._
---

## Naive Assumption
> The "naive" part of Naive Bayes comes from the assumption that features are independent given the class label. In practice, this assumption is often violated, but the algorithm still performs well in many cases.

## Types of Naive Bayes
+ Gaussian Naive Bayes: Assumes features follow a normal distribution. Often used for continuous data.
+ Multinomial Naive Bayes: Suitable for discrete data, especially for text classification where the features are word frequencies or occurrences.
+ Bernoulli Naive Bayes: Assumes binary data (e.g., presence or absence of a word).

## Formula of Bayes Thoerem
$P(A∣B)= 
P(B)
P(B∣A)⋅P(A)
​
$

---
[Click to view Thoerem Formula](https://ibb.co/fXBB53F)

## Explanation
Assuming we have two machines producing spanners and to find out the probability of Machine 1 or 2 producing a bad spanner. We have the formula:

---

$P(Machine 1| defect) = P(defect | Machine 1) * P(Machine 1) / P(defect)$

+ The P(Machine 1) is given the condition (defect)

## Questions
_Represent the following following in bayes thoerem_

1. + Out of all defective parts: we can see that 50% came from machine 1 and 50% came from machine 2

### Answer: 
> Tips: The one looked for come first, if already got, it comes first like 50% is already got

_P(Machine 1 | Defect) = 50%_

2. + What is the probability that a part produced by machine 2 is defective?

### Answer
_P(Defect | Machine 2) = ?_ 

### Write the base Theorem formula for _P(Defect | Machine 2)_
$P(Defect | Machine 2) = P(Machine 2 | Defect) * P(Defect) / p(Machine 2) $


## Case 1
> Assuming you have two features of Salary and Age, to predict if one drives to work or walks to work.
> + [See the case Diagram](https://ibb.co/L1YcKQN)
> + To solve this we need __A PLAN ATTACK__: 
> Using the Naive Bayes, the steps are in the diagram:
> + [For Walks: click to view the formula](https://ibb.co/phnhyYJ)
> + [For drives: click to view the formula](https://ibb.co/8D8zrsj)
> + [Comparing the Two P(w) Vs P(d), click to view](https://ibb.co/CvmtLGZ)

---

## Calculations
### Step 1
> + To calculate the P(Walks)
> + [Click to view calculation for P(Walks)](https://ibb.co/c2jhWb2)
> + To calculate Marginal Likelihood:
> + [Click here to view P(X)](https://ibb.co/jMGVWDk)
> + To calculate Probability of Likelihood of P(X|Walks)
> + [Click here to view how to get P(X|Walks)](https://ibb.co/0fPmmxn)
> + Result of the Calculations:
> + [Click to view the result for the computation](https://ibb.co/zbgRG3c)

---

### Step 2: Do same for P(Drives|X) [See formula](https://ibb.co/sw85Vw8)
> + To calculate the P(Drives)
> + Class Activities:
> + Calculate for P(Drives|X)
> + [Compare result to the answer here, click to view](https://ibb.co/55y1956)

---
### Step 3: Compare the two probability
> + [Click here to see that bof walks is greater than that of drive](https://ibb.co/RQ86Wn0)
> + Hence, the new observation will be predicted as walks to work

---

## Why is the algorithm called the Naive Bayes theorem?
### Answer
> They rely on independence assumptions which often time not correct and bayes thoerem is the foundation of the Naive base thoerem.
> like the case we used, it assumes that salary and age has to be independent, and this probably not the case because there could be some sort of correlation between age and salary for example we may have correlation that as peoples age increases in the organization, salary is likely to increase. Hence, Naive bayes disregard the correlation and regard them as independent, hence Naive assumption

## Can we get rid of P(X)?
### Answer
> Yes, we can. It is observed that the P(X) is same for the two calculations. When the two formula is compared, you can strike out the P(X) and compare with the upper side of both formula.
> + [See the diagram for more](https://ibb.co/VnR9G3z)
