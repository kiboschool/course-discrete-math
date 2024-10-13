## Multiplication Principle: Permutation and Combination
[Chapter 1.3](https://discrete.openmathbooks.org/dmoi3/sec_counting-combperm.html)

> Remember: Please read the text linked above before reading the material below.

From our sandwich example, we discussed picking vegetables twice, but getting two different kinds. You'll notice that no matter what vegetable is chosen, there are always 6 remaining. Therefore, if we want different vegetables, instead of multiplying by 7, we can multiply by 6.

> Check your understanding: What if I wanted 3 different vegetables? 4? What if I wanted them all? Does the number of ways to pick all vegetables make sense?

<details><summary>Check your answer</summary>
For 3 vegetables, we can do $7 \cdot 6 \cdot 5$, for 4, we multiply by the next number down (4). For all vegetables, we would do $7 \cdot 6 \cdot 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1$. 

This number is huge, and logically we can think about the problem a different way. If I select all the vegetables, there's really only one way to do this, unless we're worried about the order the vegetables get added to the sandwich.
</details>

From this idea, we have two different operations.

A **permutation** involves a situation where we're putting a group of things in order, or putting part of a group in order. This is the math we were doing with the vegetables.

Of course, when there are large numbers, and a large number of options being ordered, we want a faster way to write our answer. Mathematicians use **factorials** to express a number multiplied by all the positive integers below it. To denote this, we use an exclaimation point (!).

$$n! = n \cdot (n-1) \cdot (n-2) \cdot ... \cdot 3 \cdot 2 \cdot 1$$

Note though that our permutations for 2, 3, and 4 did not include all of these numbers. However, we can use another factorial to cancel out the remaining values.

For example, when we wanted 2 vegetables, we could say $\frac{7!}{5!}$ since the 5, 4, 3, 2, and 1 will cancel. Likewise, for 3 we could say $\frac{7!}{4!}$.

For general $n$ options, where we want to pick $k$ to be ordered, what would the form be?

> Think first: Try to come up with the form! Hint: in the first example, $n=7$ and $k=2$, and for the second, $n=7$, and $k=3$.

A permutation is often expressed P(n, k), and can be evaluated mathematically as

$$\frac{n!}{(n-k)!}$$

> Think first: if you have $n$ items, how many ways are there to order _all_ n of them?

This comes back to factorial, $n!$ is the number of ways to order $n$ items. This is a more true definition of factorial, which tells us what the value of 0! should be.

> Think first: What do you think 0! should be?

If we have no objects to arrange, there's 1 way to arrange them: do nothing! So, $0! = 1$.

Now, let's try to think about what realistically happens when we eat a sandwich. It doesn't really matter what order the worker puts on each vegetable.

We do know that for picking $7$ out of $7$ options, we want the answer to be $1$. Let's try to figure out how to modify our permutation formula to get the correct values.

Note that when we pick our items in order, we can count the number of ways they are ordered.

For each of the sets of k items we pick, there will be $k!$ orders we don't care about. Note that this type of problem should sound a little familiar.

Since each set has $k!$ extras, we can divide by a $k!$ to get rid of the extras from all the sets.

> Check your understanding: Why are we dividing instead of subtracting or doing any other operation?

<details><summary>Check your answer</summary>
This is very similar to our multiplication principle, it's just the reverse! For each unordered set, there are $k!$ orders, and all of these orders are counted in the final total. To undo multiplication, we use division, so dividing by $k!$ makes sense.
</details>

This operation: finding the number of unordered subsets of a larger set is called a combination, denoted ${n \choose k}$ and can be evaluated mathematically as

$${n \choose k} = \frac{n!}{k!(n-k)!}$$

We sometimes pronounce this as "n choose k" since we're choosing $k$ objects out of $n$ total objects. An easier way of writing this is $C(n, k)$, which you can use in Zoom chats or in messages if you're unable to use a mathematical expression tool. In LaTeX, we type \{ n \\choose k \} in math mode to write the more mathematical form.

> Check your understanding: Does the picking 7 from 7 result in the answer we expect (1)?

<details><summary>Check your answer</summary>
Yes! ${7 \choose 7} = \frac{7!}{7!(7-7)!} = \frac{7!}{7!} = 1$
</details>

It is possible to memorize the formulas for combination and permutation, but I would advise against simply trying to remember the formulas. This leads to some common errors that could be easily avoided if students instead remember the ideas behind each operation.

Thinking about ideas rather than the formulas will also help in combinatorial proofs.

> Check your understanding: What should ${7 \choose 0}$ logically be? What does it work out to be mathematically?

<details><summary>Check your answer</summary>
This is very similar to ${7 \choose 7}. If we want to order zero objects, there's one way to do that: do nothing.
${7 \choose 0} = \frac{7!}{0!(7-0)!} = \frac{7!}{7!} = 1$
</details>