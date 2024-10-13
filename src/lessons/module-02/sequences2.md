## Oscillating Sequences

It is frustrating that we cannot find a closed form for arithmetic series, and we can for geometric, but only under specific terms.

An Oscillating sequence cycles between values. This means an infinite series is either infinite, since it is either true that this cycle adds to a value, which will continue summing to infinity, or it's undefined if the cycle sums to zero, since we'd have to know that the infinite series ends on the last term of the cycle, or know the last term on which it ends, which we can't say.

For finite sums, finding a closed form can be difficult, since it will depend what point of the cycle the sum ends. It takes more consideration than the arithmetic or geometric sums do, but it is possible.

>Think about it: Start with the oscillating series that cycles over $1, 2, 3$. So this sequence is $1, 2, 3, 1, 2, 3, ...$. Find the sum for $1$ term, $2$ terms, all the way up to $12$ terms. Is there a pattern? How would you describe the sum for the $n$th term?

## Telescoping Sums

One last special series involves adding and subtracting terms. Specifically, a telescoping series is a series where these terms which are added and subtracted cancel each other out, except for the first and last term. For example, consider

$1 + 2 - 2 + 3 - 3 + 4 - 4 + ... + 9 - 9 + 10$

This makes closed forms very simple! The final answer for this series in particular will be $1 + 10 = 11$. If the series continues up to $n$, the resulting sum will be $n + 1$.

While not mathematically interesting when viewed in this way, finding a telescoping sum in a problem can make computation simple.

In general, it takes a sharp intuition to solve telescoping sum problems, as they are not always obvious.

Consider the sum of numbers where the $n$th term has the value

$\frac{1}{n(n+1)}$

This can be re-written as a telescoping series!

$\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}$

So the sum of this series will simply be $1 - \frac{1}{n+1}$, since all terms in the middle will cancel.
