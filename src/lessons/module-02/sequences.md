# Sequences

Sequences, like sets, are a mathematical structure. They allow us to talk about numbers in sequence, as the name implies.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Discrete Mathematics: An Open Introduction](https://discrete.openmathbooks.org/dmoi3/ch_sequences.html), [Chapter 2.1-2.2](https://discrete.openmathbooks.org/dmoi3/sec_seq_intro.html)

Recommended: [What does it feel like to invent math?](https://www.youtube.com/watch?v=XFDM1ip5HdU) by [3Blue1Brown](https://www.youtube.com/@3blue1brown)

## Sequence Definition

[Chapter 2.1](https://discrete.openmathbooks.org/dmoi3/sec_seq_intro.html)

> Remember: Please read the text linked above before reading the material below.

A **sequence** is an ordered list of objects. We'll only be discussing numerical sequences here. The sequence of natural numbers could be written:

$$0, 1, 2, 3, ...$$

In fact, we usually use the natural numbers as indices when writing out a general sequence. We do this because, in mathematical terms, a sequence is a function from the natural numbers to a value.

$$a_0, a_1, a_2, a_3, ...$$

If we want to discuss the $k$th item in a sequence, we sometimes say $a_{k-1}$. 

> Check your understanding: Why is the kth item $a_{k-1}$?

<details><summary>Check your answer</summary>

Just like indexes on a list, we have the problem that we start our labels at $0$ but verbal labels start at $1$ (the first item).

</details>

Likewise, to refer to the whole sequence we put one representative in parentheses.

$$(a_n)$$

We only do this with variables. We can do this to refer to a series if we have defined what $a_n$ is, usually in terms of previous members of the sequence, or some other mathematical statement.

For example, if we want the sequence of square numbers,

$$a_n = n^2$$

Or if we want a sequence where each number is two more than the previous number,

$$a_n = a_{n-1} + 2$$

Note that we should define $a_0$ for each sequence as well, so we can tell where it starts.

> Check your understanding: if $a_0 = 0$ and $a_n = a_{n-1} + 2$, what types of numbers are in this sequence? There should be a good name that refers to the numbers listed here. What happens when $a_0 = 1$ instead?

<details><summary>Check your answer</summary>

For the first sequence, we get the positive even numbers (plus zero).

The second sequence gives the positive odd numbers.

</details>

Since a sequence is a function, any function that has a domain of the natural numbers can be easily transformed into a sequence. For example,

$$a_n = 2n + 3$$

Would be a sequence where each value are integer values of the function $f(x) = 2x + 3$. Note that $a_0$ is defined already.

> Check your understanding: what would $a_0$ be for this sequence?

<details><summary>Check your answer</summary>

Since it's the natural numbers, the first $x$ value is $0$, and our $a_0 = 2 \cdot 0 + 3 = 3$

</details>

We can also define sequences in terms of other sequences. This is the idea behind partial sums.

Pretend there is a Kibo course where students learn five new topics each week. The sequence of topics learned per day would simply be

$$5, 5, 5, 5, ...$$

However, what if we want to measure how much a student has learned so far?

On the first day, they learn 5 topics.

On the second day, they learn 5 more topics, for a total of $5 + 5 = 10$. This is a **partial sum** of our initial sequence. We add the first term to the second to get the second day total.

And this continues, each day $5$ topics are added.

$$5, 5+5, 5+5+5, 5+5+5+5, ...$$

A **sequence of partial sums** is created by taking the sum of $a_0$ to $a_{n-1}$ for the $n$th term of the sequence.

> Check your understanding: If our initial sequence is the odd numbers, what does the sequence of partial sums look like? Try finding a few terms, and see if you can spot the pattern.

<details><summary>Check your answer</summary>

$1 = 1$

$1 + 3 = 4$

$1 + 3 + 5 = 9$

$1 + 3 + 5 + 7 = 16$

These are the square numbers! The partial sum sequence would be:

$1, 4, 9, 16, 25, ... $

</details>

## Sequence Versus Series

A **series** is defined as being the sum of each term in a sequence. For example, if we have the sequence of the positive integers, the series would be the sum of the posititive integers, which would be infinite. In general, many infinite series may end up resulting in an infinite answer, however, some have a solution! If we have a finite sequence, there should be a finite answer, though how easy this is to compute depends on the series.

These terms are related, and it is easy to get them confused, especially since they are similar sounding words. However, a sequence should never contain a sum, and a series should usually have some final answer when computed (which may be infinity).
