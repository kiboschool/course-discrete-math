# Divisibility

Divisibility is an important concept to Number Theory. We will discuss a few ways of thinking about divisibility here.

## Divisibility

There are many terms similar to divisibility that you may already be familiar with:

If $n$ is divisible by $d$, this means:

- $d$ is a factor of $n$
- $d$ divides $n$
- $d | n$ (A symbol, read as "divides")

And if $d \neq 0$,

- $n$ is a multiple of $d$.

$n$ is divisible by $d$ if 

$\frac{n}{d} = k$ where $k \in \mathbb{Z}$.

> Think about it: Why does $d$ need to be non-zero for multiple to the same as divisibility?

If $d$ does not divide $n$, we can express this as 

$d \nmid n$

> Check your understanding: List all numbers that divide 6. List all numbers that divide 9. List all numbers that divide 11.

<details><summary>Check your answer</summary>

For $6$: $-6, -3, -2, -1, 1, 2, 3, 6$

For $9$: $-9, -3, -1, 1, 3, 9$

For $11$: $-11, -1, 1, 11$

</details>

> Check your understanding: There is a specific term for numbers that are divisible by 2. What is it?

<details><summary>Check your answer</summary>

Even!

</details>

## Quotient-Remainder Form / Division Algorithm
[Chapter 2.1](https://math.gordon.edu/ntic/ntic/section-div-alg.html)

From the previous example, we know $4$ does not divide 6. We can write these numbers in quotient-remainder form as follows:

$6 = 4 \cdot 1 + 2$

Where $2$ is the remaining amount (remainder) left over when we have divided 6 by 4 as much as we can.

In this case, 1 is the quotient, and 4 is sometimes known as the dividend.

In any case, there is a theorem that tells us the following:

For any integers $n$ and $d$, there are unique integers $q$ and $r$, with $0 \leq r < n$ such that

$n = d\cdot q + r$.

> Check your understanding: What are $q$ and $r$ for $n=13$, $d=6$? What about $n=13$, $d=-6$? What about $n=-13$, $d=6$?

<details><summary>Check your answer</summary>

$13 = 6 \cdot 2 + 1$

$13 = -6 \cdot -2 + 1$

$-13 = 6 \cdot -3 + 5$

</details>

Quotient-Remainder form can be useful for future topics, so keep this in mind.

## Divisibility of Large Numbers

If a number is divisible by 10, can you say any other numbers it might be divisible by?

Since 10 is divisible by 2 and 5, we can use this to say any number divisible by 10 is also divisible by 2 and 5!

This is simple to see:

$n = 10k = 5 \cdot 2k = 5(2k)$ which is a multiple of $5$!

If a number is divisible by a number, k, it is also divisible by any factors of k.

We can also use this the other way around:

If a number is divisible by $2$ and $5$, then it is divisible by $10$.

We have to be careful, though.

> Think about it: Can you think of three numbers where this doesn't work?
> Hint: $3$, $6$, and $18$ is an example. 