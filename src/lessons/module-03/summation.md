# Summation Notation

Summation Notation is an important piece of mathematical notation that allows us to express summations quickly.

## Summation Notation

Summation Notation is used to describe a sequence of terms which are added together. This is done using at least one variable, where each term is a function of this variable, and the lowest and highest values of the variable are stated. It uses the capital greek letter Sigma, an S for sum.

The following summation denotes the sum of the first $10$ positive integers.

$$\sum_{k=1}^{10} k$$

Here, the variable is $k$, the lowest value it takes is $1$, and the highest value it takes is $10$. When read out loud, we would say "the sum from $k$ equals 1 to $k$ equals 10 of $k$."

You can also do summations over multiple variables, or summations of summations. For example,

$$\sum_{k=1}^{10}\sum_{j=1}^{5}k^j$$

Gives the sum of the first $10$ positive integers, each to the value of the first $5$ numbers. We do the inner sum first, then the outer, just like nested loops.

$$\sum_{k=1}^{10}\sum_{j=1}^{5} k^j = 1^1 + 1^2 + 1^3 + 1^4 + 1^5 + 2^1 + 2^2 + 2^3 + 2^4 + 2^5 + ... + 10^1 + 10^2 + 10^3 + 10^4 + 10^5$$

Note that in this case, we can swap the summations and still have the same sum, just ordered differently.

$$\sum_{j=1}^{5}\sum_{k=1}^{10} k^j = 1^1 + 2^1 + ... + 10^1 + 1^2 + 2^2 + ... + 1^5 + 2^5 + ... + 10^5$$

If we want to denote an infinite series, we can set the top bound to infinity.

$$\sum_{k=1}^{\infty} k$$

> Check your understanding: What does this sum represent? What is its value?

<details><summary>Check your answer</summary>

This is simply the sum of the natural numbers, which is infinite.

</details>

In LaTeX, we use \sum to use summation notation, and sub/super-scripts for the bounds on the variable.

> Think about it: What would $\sum_{k=1}^{10} 1$ be?

## Capital Pi Notation

There is a lesser-known notation for multiplying many things in a row. Instead of a big sigma, we use a big pi symbol.

$\prod_{k=1}^{10} k = 1 \cdot 2 \cdot ... \cdot 10$

> Check your understanding: What's the value of $\prod_{k=1}^{10} 2k$?

<details><summary>Check your answer</summary>

$2^{10} \cdot 10!$

</details>
