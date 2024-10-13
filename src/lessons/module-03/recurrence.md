# Recurrence Relations

Recurrence relations are related to the idea of recursive functions. Here, we discuss the mathematical structure of recrrences and how to solve them, as well as some applications of recurrence relations.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Applied Discrete Structures](https://discretemath.org/ads/chapter_8.html), [Chapter 8.1, 8.3-8.4](https://discretemath.org/ads/s-faces-of-recursion.html)

[Discrete Mathematics: An Open Introduction, Chapter 2.4](https://discrete.openmathbooks.org/dmoi3/sec_recurrence.html)

## Examples of Recurrence Relations
[Chapter 8.1](https://discretemath.org/ads/s-faces-of-recursion.html)

> Remember: Please read the text linked above before reading the material below.

In the last module, we discussed some particular sequences. The geometric and airthmetic sequences are technically both recurrence relations, since they are defined by a reference to themselves.

The Fibonacci sequence is perhaps one of the most popular recurrence relations. This relation is special as it references itself twice. Each term in the sequence is the sum of the two previous terms, where the first two terms are $0$ and $1$ (or $1$ and $1$ depending on who you ask).

$$1, 1, 2, 3, 5, 8, 13, 21, ... $$

To write this in the form of a recurrence relation, we say 

$$f_0 = 1, f_1 = 1$$

$$f_n = f_{n-1} + f_{n-2}$$

> Check your understanding: What does the fibonacci sequence look like if the first two terms were $1$ and $2$ instead of $1$ and $1$? How much of a difference does this make? What about starting with $2$ and $3$? $3$ and $4$?

<details><summary>Check your answer</summary>

$1$ and $2$ already exist in the fibonacci, this would just move everything up by one.

Similarly, with $2$ and $3$ everything would get moved up by $2$.

However, $4$ is not in the fibonacci sequence, so this would be different.

$3, 4, 7, 11, 18, 29, 47, 76, ... $

</details>

A lesser known variant is the Tribonacci sequence, which takes the sum of the last three terms instead.

$$t_0 = 1, t_1 = 1, t_2 = 2$$

$$t_n = t_{n-1} + t_{n-2} + t_{n-3}$$

> Check your understanding: Write out the first $10$ terms of this sequence. How different is it from the Fibonacci sequence?

<details><summary>Check your answer</summary>

$1, 1, 2, 4, 7, 13, 24, 44, 81, 149, ... $

It's quite different, from the moment the recurrence starts.

</details>

## Iteration
[Chapter 8.1](https://discretemath.org/ads/s-faces-of-recursion.html)

> Remember: Please read the text linked above before reading the material below.

Just like programming, many recurrsive relations can be evaluated iteratively rather than recursively. However, there is no such thing as "iterative relations." Instead, this can be a method used in solving recurrence relations.

## Recurrence Relations
[Chapter 8.3](https://discretemath.org/ads/s-recurrence-relations.html)

> Remember: Please read the text linked above before reading the material below.

Recurrence relations are simply sequences for which almost all terms are defined by previous terms of the sequence. The arithmetic and geometric sequences, the fibonacci sequence, and the tribonacci sequence are all examples of recurrence relations. However, these do not cover all the potential ways a recurrence relation can be created or defined.

A recurrence relation could reference a term farther back than the one before it, and the sequences can include negative values:

$$r_0, r_1, r_2 = 1$$

$$r_n = 3r_{n-3} - r_{n-2}$$

$$1, 1, 1, 2, 2, 1, 4, 5, -1, 7, 16, -10, ...$$

You can also perform different types of operations, like raising to a power, taking a logarithm, a root, or any other mathematical operation.

$$r_0 = 1$$

$$r_n = (r_{n-1} + 1)^2$$

$$1, 4, 25, 676, 458329$$

A relation is not a recurrence relation if it does not reference itself. Not all sequences are recurrence relations. For example, the sequence of square numbers is not a recurrence relation, since it depends on the index of each term, not a function on any prior term.

> Check your understanding: Create one recurrence relation, and one sequence that is not a recurrence relation.

<details><summary>Check your answer</summary>

Answers will vary, but remember that a recurrence relation must meaningfully reference itself.

</details>