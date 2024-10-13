## Solving Recurrence Relations: Linear Recurrence Relations
[Chapter 8.3](https://discretemath.org/ads/s-recurrence-relations.html)

> Remember: Please read the text linked above before reading the material below.S

The chapter above details exactly how linear recurrences (those which are only made up of ) can be solve. The most important part of this is the idea behind the method. There are many problems in mathematics that can be reduced to solving for the roots of an equation.

The same applies here. When we transform a recurrence into a function, the roots can be converted into a solution using a clever bit of math.

## Solving Recurrence Relations: Intuition

One method of solving a recurrence relations involves knowing or guessing the final solution. If you have the closed form, or believe you have the closed form, you can plug this in for the terms in the recurrence for $r_n$. If the final result matches the expected form for $r_n$, then the solution is correct! If not, some information could be gathered.

Suppose I tell you the solution to the below recurrence is $\log_2{(n)}$, for $n = 2^k$.

$$T(1) = 0$$
$$T(n) = T(\frac{n}{2}) + 1$$

We can plug in $T(\frac{n}{2}) = \log_2{(\frac{n}{2})}$

$$T(n) = \log_2{(\frac{n}{2})} + 1$$

Let's let $n = 2^k$

$$T(2^k) = \log_2{(\frac{2^k}{2})} + 1 = \log_2{(2^{k-1})} = 1 = k - 1 + 1 = k = \log_2{(2^k)}$$

We've now shown that this solution works, since we didn't pick any specific value for $n$.

> Check your understanding: What do you think the solution might be for $T(n) = T(\frac{n}{3}) + 1$, where $n = 3^k$? Check your answer using this substitution method.

<details><summary>Check your answer</summary>

This is simply $\log_3{(n)}$. The substitution method is very similar to the one above, just replacing mentions of base $2$ with base $3$.

</details>

## Solving Recursive Problems Iteratively
[Discrete Mathematics: An Open Introduction, Chapter 2.4](https://discrete.openmathbooks.org/dmoi3/sec_recurrence.html)

One way we can guess at a final solution is to iteratively substitute in the value of the right hand side. We can see what pattern forms, and use it to find a solution.

For example, we might have 

$$T(1) = 1$$
$$T(n) = 2T(n-1) + 1$$

If we substitute $T(n-1) = 2T(n-2) + 1$, we'll have

$$T(n) = 2(2T(n-2) + 1) + 1$$

> Check your understanding: Why is $T(n-1) = 2T(n-2) + 1$?

<details><summary>Check your answer</summary>

This is just the definition of the recurence, replacing $n$ with $n-1$

</details>

Likewise, $T(n-2) = 2T(n-3) + 1$

$$T(n) = 2(2(2T(n-3) + 1) + 1) + 1$$

> Think first: Do you see a pattern here? What would this look like if we kept going until $T(n-k)$ was the term on the right side?

We should note that the number of $2$s is the same as the number being subtracted from $n$. We should also note that there are parentheses every time. Let's look at the form we just created, when the $2$s are distributed.

$$T(n) = 2(2(2T(n-3) + 1) + 1) + 1 = 2^3T(n-3) + 2^2 + 2^1 + 1$$

I kept these $2$s as powers for a reason.

> Think first: if you didn't before, do you see the pattern now?

We should get 

$$T(n) = 2^kT(n-k) + 2^{k-1} + 2^{k-2} + ... + 2^2 + 2^1 + 1$$

Note that when $k = n-1$, $T(n-k) = T(n-(n-1)) = T(1)$, which is our base case of $1$.

So, when we iterate down to the lowest level, we'll have

$$T(n) = 2^{n-1}\cdot 1 + 2^{n-2} + 2^{n-3} + ... + 2^2 + 2^1 + 1$$

As we know from the series content, the sum of powers of $2$ is $2^n - 1$.

Thus, we get our solution! If we wanted to double check, we could substitute this value in, and see if it holds.

$$T(n) = 2T(n-1) + 1 = 2(2^{n-1} - 1) + 1 = 2^n - 1$$

> Think about it: Can you come up with a general solution for $T(n) = bT(n-1) + 1$, where $b$ is some real number?

## Solving Recurrence Relations: Other Methods

There are many methods out there for solving recurrence relations. However, they tend to be application-specific, and a little harder, require a background in calculus, or are weirder than the methods above. A good project could discuss the Master Theorem, which is a general set of rules for solving certain recurrence relations.

## Recurrence and Recursion

Recursive code can be often described using a recurrence relation.

def fibonacci(n):
    if n == 0 or n == 1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

The code above will calculate the $n$th fibonacci number. We should be able to see that the base case translates to the first term(s) of the sequence, and the recurrence is seen in the recursive call.

Simply take the name of the function, and replace it with a capital letter. If you set it equal to the recursive call (with the same changes made), you should get a recurrence relation.

> Check your understanding: Find a recursive function you wrote, or one on the internet. Can you write a recurrence relation based on this function? Is there a simple, closed form solution to this recurrence?

<details><summary>Check your answer</summary>

Answers will vary, but you can test the time of the function by running multiple times with larger values and timing how long it takes to run, or you can test the values you get by running the function multiple times and comparing to your mathematical answers.

</details>

## Applications: Analysis of Algorithms
[Chapter 8.4](https://discretemath.org/ads/s-some-common-rrs.html)

> Remember: Please read the text linked above before reading the material below.

Recurrence relations are often used to describe how an algorithm runs, as many algorithm are recursive in nature. From this recurrence relation, we can determine about how long an algorithm will run, given an input of size $n$. The reading above gives an analysis of the Binary Search algorithm using recurrence relations.