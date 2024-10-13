# Linear Congruences

Now that we can perform almost all the same operations we can on normal numbers, we can talk about solving equations in modular arithmetic.

## Simple Linear Congruences

As it turns out, we can do some minor manipulations to solve simple examples of linear congruences. Watch the following video and attempt the last example given!

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/KwxslifHITg?si=lVvQ9o2KII_3USi4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

## Solving Equations

Given an equation like:

$3x + 2 = 5$

How would you solve for x?

First subtract $2$ from both sides

$3x = 3$

Then divide by $3$

$x = 1$

The equation is solved!

Now that we know how to "divide" in a congruence, we can solve any simple equation like this easily!

## Solving Linear Congruences

Consider

$3x + 2 \equiv 5 \mod{7}$

The first step, subtracting by $2$ is the same here.

$3x \equiv 3 \mod{7}$

Here is where we would find the inverse of $3$ and multiply both sides by $3^{-1}$. However, before we go through the effort of finding it, consider what happens to the righthand side when we multiply by $3^{-1}$

$3 \cdot 3^{-1} \equiv 1 \mod{7}$

Because we know there is an inverse, and how it works, we don't even have to find it! we can just skip to the next step and fake divide by $3$ on both sides. Again, this only works because $3$ has an inverse $\mod{7}$. If $GCD(3, 7)$ was not $1$, we could not do this, and would have to just test random $x$ values.

Note our answer to this is 

$x \equiv 1 \mod{7}$

Because we're working with congruences, there are actually infinitely many answers! All $x$ which are one more than a multiple of $7$ work for this equation.

Let's do another example that's not so simple:

$3x - 2 \equiv 4 \mod{7}$

First step: add $2$ to both sides

$3x \equiv 6 \mod{7}$

At first, it seems we must now find the inverse of $3$ $\mod{7}$, but let's think about the right-hand side again.

$6 = 2 \cdot 3$

If I multiply by $3^{-1}$, the $3$ would disappear, and the two would remain. We can still divide!

$x \equiv 2 \mod{7}$

Unfortunately, there may be times where the solution is not so nice.

$3x \equiv 5 \mod{7}$

Here, we would have to find $3^{-1}$, then multiply. Luckily, we now know the extended euclidean, which will easily generate the inverse.

$3x \equiv 3 \mod{6}$

Even though the left-hand side is divisible by $3$, we can't divide. $3$ is not relatively prime to $6$. Instead, because $6$ is small, we can test values.

$x \equiv 1 \mod{6}$ works

$x \equiv 2 \mod{6}$ does not work

$x \equiv 3 \mod{6}$ works

$x \equiv 4 \mod{6}$ does not work

$x \equiv 5 \mod{6}$ works

$x \equiv 6 \mod{6}$ does not work

Now we have our answers:

$x \equiv 1, 3, 5 \mod{6}$

> Check your understanding: Generate three numbers, a, b, and c, and a prime number p, then try to solve the equivalence

> $ax + b \equiv c \mod{p}$

You will not be able to memorize all these rules, practice will help you feel more comfortable working with modular arithmetic.