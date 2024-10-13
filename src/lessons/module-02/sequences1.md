## Special Sequences
[Chapter 2.2](https://discrete.openmathbooks.org/dmoi3/sec_seq-arithgeom.html)

> Remember: Please read the text linked above before reading the material below.

There are two main types of sequences that have very nice ways to solve for the nth term, or for the sum of the sequence.

### Arithmetic Sequences

An **arithmetic sequence** is a sequence where each term is $k$ more than the previous term. This $k$ is known as the **common difference**. An arithmetic sequence can be defined by the initial term ($a_0$) and the common difference.

Earlier, we defined a sequence

$$a_n = a_{n-1} + 2$$

Let's consider this sequence with $a_0 = 1$. The common difference will be $2$, since this is what we add to each term. This would give us the sequence of positive odd numbers! So, it turns out that odd numbers are an arithmetic sequence.

> Check your understanding: How could we transform this series to instead get the sequence of positive even numbers?

<details><summary>Check your answer</summary>

Let $a_0 = 2$. Note that $0$ is not positive, so we can't include it. 

</details>

In general, an arithmetic sequence can be written:

$$a_n = a_{n-1} + k$$

However, there's an easier way of finding the $a_n$th term.

Notice:

$a_1 = a_0 + k$

$a_2 = a_1 + k = (a_0 + k) + k = a_0 + 2k$

$a_3 = a_2 + k = (a_0 + 2k) + k = a_0 + 3k$

A pattern begins to appear. We should be able to reason through this as well. At the $a_n$ term, $k$ has been added $n$ times in total since the start. So,

$$a_n = a_0 + nk$$

Notice that this is not the $n$th term, but the $n+1$st term, since we start at $a_0$.

If we wish to find the final solution to an arithmetic **series**, this is simple. Add the terms. However, a long series could prove a challenge.

Let us start with the simple example of the sequence of positive integers up to $n$

$$1, 2, 3, 4, ... , n-1, n$$

If we start adding from the start of this sequence, there seems to be no pattern in the results, other than adding one more than one was added previously. This doesn't help us for a general case, like the one given above.

However, addition is commutative, we can add these terms in any order.

We can notice if we take terms from the front and back of the sequence, the sum is always $n+1$, so we rearrange the series to sum it:

$1 + n$ + $2 + (n-1)$ + $3 + (n-2)$ + ...

Our next task is to find how many $n + 1$ terms we have.

If we're taking from both sides, when we stop, we'll be at the middle of the sequence. Half of the sequence will be before this point, and half will be after. We will have created a group once per term on the left hand side of this midpoint, so in total, there should be $\frac{n}{2}$ of these $n + 1$ terms.

Therefore, our total should be $\frac{(n + 1)n}{2}$

This gives us the **closed form** sum of a finite arithmetic series from $1$ to $n$ with common difference $1$. A **closed form** is just a single expression that is the solution to an expression with a much longer form. 

$$1 + 2 + 3 + ... + (n-1) + n = \sum_{i=1}^n i = \frac{(n + 1)n}{2}$$

Another way to view this process is to think of writing our series backwards:

$$n + (n-1) + (n-2) + ... + 2 + 1$$

This is still the same as our original, we just moved around additions again!

If we add this series to our original series, matching the terms together, we find that same phenomenon of the $n+1$ sum.

$$n + (n-1) + (n-2) + ... + 2 + 1$$
$$+ 1, 2, 3, 4, ... , (n-1), n$$
$$(n+1) + (n+1) + (n+1) + ... + (n+1) + (n+1)$$

Here, it may be easier to see that there are $n$ of these $n+1$ terms, since there's one for every member of the sequence.

However, we've added our sum to itself, so our answer is $2$ times more than what it should be, and we get the same closed form as before: $\frac{(n+1)n}{2}$

> Think about it: How can we expand this closed form to any arithmetic series? 
> Try finding the closed form of the sum of even numbers from $2$ to $n$. This has a common difference of two instead of one. What happens there?
>
> And what happens if you try to find the sum starting from some other value, like $4$ instead of $1$ in our original sequence with common difference $1$?
>
> If you get stuck, try computing a few of the series and seeing if you notice a pattern in the answers other than the common difference. Compare these answers to each other, and to the answers we would get for the series we solved above. Stick to positive integer terms in your experiments, we'll get to fractions and negative terms after the next topic.

### Geometric Sequences

A **Geometric sequence** is a sequence where each term is $k$ times the previous term. This $k$ is known as the common ratio. A Geometric sequence can be defined by the first term and the **common ratio**.

Instead of adding $2$, if we start at $1$, and multiply by $2$ to form each term, we get the sequence of powers of $2$:

$$1, 2, 4, 8, 16, 32, ... $$

>Check your understanding: What happens if the starting number is changed to a $2$? A $3$? A $0$?

<details><summary>Check your answer</summary>

$2$: the sequence shifts forward by one value. These should still be powers of $2$

$3$: Every power of two is just multiplied by a single $3$.

$0$: All the terms would be zero. Boring!

</details>

In general, a geometric sequence can be written:

$$a_n = ka_{n-1}$$

With a defined $a_0$ term.

To find the $n$th term, let's think about the sequence from the start.

The first term will be $a_0$

$a_1 = ka_0$

$a_2 = ka_1 = k(ka_0) = k^2a_0$

$a_3 = ka_2 = k(k^2a_0) = k^3a_0$

For the $a_n$th term, we will have

$a_n = k^na_0$

Similar to the arithmetic sequence, this is the $n+1$st term in the sequence as a whole, since we start at $a_0$.

If we wish to find the closed form of the geometric series, we need to be even more clever than before.

Let's consider the powers of two up to $2^n$

$1 + 2 + 4 + ... + 2^{n-1} + 2^n$

We can't match terms from both ends this time, but we can do other things to the entire series if we undo the changes at the end.

Consider the same series, multiplied by $2$

$2 + 4 + 8 + ... + 2^n + 2^{n+1}$

This series has almost all the same terms! Let's call our series $S$. This makes the second series we found $2S$.

If we subtract our original series from the new series, all terms but two will cancel with each other! The last term of the second series and the first term of the first.

$2S - S = 2^{n+1} - 1$

If we want to know what $S$ is, we can solve algebraically

$S(2-1) = 2^{n+1} - 1$

$S = \frac{2^{n+1} - 1}{2 - 1}$

This answer for the series of powers of two should make sense for those familiar with binary. Adding every power of two up to $2^n$ would represent a $1$ in each digit. If $1$ was added, it would turn into the next power of $2$, $2^{n+1}$. Therefore the value is $2^{n+1} - 1$.

>Think about it: How would this change for powers of three? What would we multiply the series by in the first step? What is the general form for a series for $b$ to a power? What would change if the starting term was different?

### Infinite Arithmetic and Geometric Sequences

These have been closed forms for finite series. What if we want the sum of an infinite series? How can we tell if the sum should result in infinity or a finite value?

Infinite arithmetic series always turn out to be infinite in their final sum, unless the common difference is zero, and our first term is also zero. This should make sense, as there is no number we can add an infinite amount of times that wouldn't result in infinity, even if it was slow to reach infinity.

For geometric series, we can multiply by a common ratio between $-1$ and $1$. This will ensure the terms shrink as the series continues.

We can find the closed form in a similar way to the finite version. We'll have $S$ and $kS$, where $k$ is the common ratio. Because there are infinite terms, now the "last" term of $kS$ will also cancel, since each term in $kS$ is also present in $S$. The first term, $a_0$, in $S$ will be the only term that is not present in the other series.

$kS - S = -a_0$

Multiplying by $-1$ on both sides,

$S - kS = a_0$

$S(1-k) = a_0$

$S = \frac{a_0}{1-k}$

This is the closed form for a geometric series.

This should make sense from our finite closed form. The $2^{n+1}$ term grows because $2 > 1$. If the base of the exponent, let's call it $k$, was a fraction, as $n$ increases, $k^n$ becomes smaller until it is practically $0$.

Of the terms left, if the top and bottom of the fraction are multiplied by $-1$, we are left with the first term on top, and $1 - 2$ in the denominator, where $2$ is the common difference.

There is no real difference in the equation for an infinite geometric series, we just assume that $k^n$ vanishes as $n$ increases.
