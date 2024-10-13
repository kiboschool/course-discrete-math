# Linear Congruences: Multiple Systems

We've found ways to complete a one-variable equivalences, just like normal one-variable equations.

## Solving Two-System Equations

Say we have two systems:

$2x + 3 = 2y$

$4x + 7 = y$

We can solve this using a few methods, but I will focus on the substitution method.

Since $y = 4x + 7$, We can substitute $4x + 7$ for $y$

$2x + 3 = 2(4x + 7)$

Now we have an equation in terms of $x$! We follow our usual steps to solve, then we can plug $x$ into one of the equations and solve for $y$

## Solving Two-System Congruences

While we could use multiple variables in congruences, the problem becomes more interesting (and less difficult) if we keep to one variable, but different moduli.

$x \equiv 4 \mod{5}$

$x \equiv 6 \mod{7}$

We want an $x$ that fits **both** equivalences.

>Think first: How do we solve this? Can we change the substitution method to fit with mods?

Keep in mind for this that $x$ is not necessarily equal to $4$, just equivalent. However, we can say that

$x = 5n + 4$

Where $n$ is an integer. Now we have strict equality, so we can substitute it in!

$5n + 4 \equiv 6 \mod{7}$

Let's solve this for $n$ as normal. First subtract $4$ from both sides.

$5n \equiv 2 \mod{7}$

Then multiply both sides by $5^{-1} \mod{7}$. Remember: we can find this value through the extended euclidean, but for these small numbers, trial and error may be faster. In this case, $3$ is the inverse we're looking for, so

$n \equiv 6 \mod{7}$

In this case, it happens to be that $n$ is the same modulus as $x \mod{7}$, but this just happens to be a coincidence. Our next step is to see what $n$ is equal to.

$n = 7m + 6$

Now we can substitute this in our $x$ equality from before.

$x = 5(7m + 6) + 4$

$x = 35m + 30 + 4$

$x = 35m + 34$

Now we have to notice a few things:

1. $35 = 5 \cdot 7$

2. $x = 35m + 34$ means that $x \equiv 34 \mod{35}$

3. $34$, and numbers that are equivalent to $34 \mod{35}$ work for our above equivalences.

Therefore,

$x \equiv 34 \mod{35}$

is our answer.

> Think about it: There's actually another clever way to solve this problem, if you know the answer will be some residue $\mod{35}$. Can you find it?

## Multiple Systems

What if there are three or more sets of congruences? We can use the same method! We are guaranteed a unique solution by the Chinese Remainder Theorem if the moduli are all pairwise **relatively prime**. Two numbers are relatively prime if their GCD is $1$. We'll explore in the next section.

The video below shows how to solve a three congruence system.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/LInNgWMtFEs?si=96HoclKmaZqI1sRj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>

## Quadratics

We can also solve problems like

$x^2 + 3x + 2 \equiv 0 \mod{7}$

>Think first: How can we go about solving this?
>Hint: Think about Diophantine Equations

Whatever happens, we know the left hand side is a multiple of $7$. Let's do the typical quadratic thing and factor.

$(x + 1)(x + 2) \equiv 0 \mod{7}$

>Think first: What would you do for $(x + 1)(x + 2) = 0$?

Since these are multiplied, and $7$ is prime, the answers are when one of the factors is equivalent to zero (meaning divisible by 7).

$x \equiv 6, 5 \mod{7}$

As it turns out, we can do this even if the modulus is composite, we just need to check some other combinations.

For example, if we had $\mod{35}$, we would need to check 35 as well as 5 and 7. Note that for it to multiply correctly, one has to be equivalent to $5$ while the other is equivalent to $7$, since

$5 \cdot 7 \equiv 0 \mod{35}$

but

$5 \cdot 6 \not\equiv 0 \mod{35}$

We should also check both directions: 5 then 7, and 7 then 5.

I will not ask you to solve for non-prime moduli. The ideas behind quadratics and other polynomials could be a good project topic, if combined with some other material!