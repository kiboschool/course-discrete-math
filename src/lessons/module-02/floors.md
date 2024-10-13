# Floors and Ceilings

The floor and ceiling function are special functions that can be performed on numbers. This may be review, but is important to know for this week and moving forward.

## Floor

The floor function takes a number ($x$) as input and outputs the greatest integer less than or equal to the input. In math terms,

$$\lfloor x \rfloor = y \text{, } x-1 < y \leq x$$

> Check your understanding: What is $\lfloor 5 \rfloor$? What about $\lfloor 5.2 \rfloor$ or $\lfloor 5.7 \rfloor$? How is this different from rounding?

<details><summary>Check your answer</summary>

These are all $5$! Flooring always rounds down the number, rather than the typical rounding up for values closer to the next integer.

</details>

When values are negative, it can be a little confusing at first to apply the floor function.

$$\lfloor -5.2 \rfloor = -6$$

Remember: the negative integer less than $-5.2$ is $-6$. $-5$ is actually greater than $-5.2$.

> Check your understanding: What happens when you floor $\frac{n}{2}$ for $n = 1, 2, 3, ..., 10$? What about $\frac{n}{3}$?

<details><summary>Check your answer</summary>

$\lfloor \frac{n}{2} \rfloor = 0, 1, 1, 2, 2, 3, 3, 4, 4, 5$

It seems we get a sequence of values, each appearing twice (except for zero). This may be useful later...

$\lfloor \frac{n}{3} \rfloor = 0, 0, 1, 1, 1, 2, 2, 2, 3, 3$

Now we have triples, and zero only appears twice.

</details>

> Think about it: Can you describe what happens when we take $\lfloor \frac{n}{k} \rfloor$ over the positive integers, for any integer $k$?

## Ceiling

The ceiling function takes a number ($x$) as input and outputs the smallest integer greater than or equal to the input. In math terms,

$$\lceil x \rceil = y \text{, } x \leq y < x+1 $$

Instead of always rounding down, this is always rounding up. The examples used in the Check Your Understanding would now be all $6$s instead of all $5$s.

Likewise, for the negative numbers, the higher number will be the opposite of the positive integers. $\lceil -5.2 \rceil$ will be $-4$.

> Check your understanding: What happens to $\frac{n}{2}$ and $\frac{n}{3}$ when we apply ceiling to the first $10$ positive integers?

<details><summary>Check your answer</summary>

$\lceil \frac{n}{2} \rceil = 1, 1, 2, 2, 3, 3, 4, 4, 5, 5$

Now the sequence of values has no zero, so all terms are doubled!

$\lceil \frac{n}{3} \rceil = 1, 1, 1, 2, 2, 2, 3, 3, 3, 4$

Now we have triples, and once again, no zero.

</details>

> Think about it: How is the ceiling of $\frac{n}{k}$ different from the floor for the sequence of positive integers, when $k$ is an integer?