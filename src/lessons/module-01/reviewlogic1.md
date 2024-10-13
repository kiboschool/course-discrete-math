## Implication
[Chapter 3.3](https://discretemath.org/ads/s-equivalence-implication.html)

> Remember: Please read the text linked above before reading the material below.

There is one more operator that is important for us to know. An **implication** creates an "if/then" statement.

$$p \rightarrow q$$

This denotes that p implies q, or in other words, if p is true, then q is true.

| $p$ | $q$ | $p \rightarrow q$ |
|---|---|---|
| 0 | 0 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

Note that when p is false, $p \rightarrow q$ is true. This is because it is a one-way implication. If p is not true, we have not stated whether q should be true or false. The only place where $p \rightarrow q$ is false is when p is true and q is false. This idea of implication gives us another way to state $p \rightarrow q$ using our simple operators. Since the negation of $p \rightarrow q$ is $p \wedge \neg q$, $p \rightarrow q$ is equivalent to $\neg(p \wedge \neg q)$. Try building a truth table yourself for practice!

We can also use implication both ways. This has its own special symbol.

$(p \rightarrow q) \wedge (q \rightarrow p) \equiv p \Longleftrightarrow q $

This can be stated as "p is true if and only if q is true." Mathematicians often abbreviate "if and only if" as "iff." This double implication is another way to say two statements are equivalent.

When doing algebra, we learn that parentheses are evaluated first, then exponents, then multiplication/division, and finally addition/subtraction, all completed from left to right. A similar set of rules applies for logical operators.

First, parentheses, then negation, then "and", then "or", then implication, and finally double implication, all evaluated from left to right when there are multiple of the same type.
