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
