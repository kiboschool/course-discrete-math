# Useful Theorems

## A Cool Observation

This video highlights someone's observations about primes, how it relates to number theory, and an important theorem we can draw from it.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/EK32jo7i5LQ?si=nFIQJqZMPzZY2Fzz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

## Fermat's Little Theorem

Take 2 to a power $\mod{5}$. In fact, let's list out what these powers look like.

$2^0 \equiv 1 \mod{5}$

$2^1 \equiv 2 \mod{5}$

$2^2 \equiv 4 \mod{5}$

$2^3 \equiv 3 \mod{5}$

$2^4 \equiv 1 \mod{5}$

$2^5 \equiv 2 \mod{5}$

$2^6 \equiv 4 \mod{5}$

$2^7 \equiv 3 \mod{5}$

There seems to be a pattern here!

> Think first: Try finding powers of $2 \mod{7}$. What do you find?

Fermat has a little theorem that states:

If $p$ is a prime, then

$a^p \equiv a \mod{p}$

Which can also be stated as

$a^{p-1} \equiv 1 \mod{p}$

This happens for primes as we need to run through all residues, except for zero, before returning to $1$ in a prime modulus. Notice that the powers of two repeated in cycles through all of the residues of our mods above.

See the video below for a visual reason:

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/OoQ16YCYksw?si=36LLBsG5JDkgcgEO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

There is another theorem called Euler's Theorem which generalizes this, and could make a good project topic.

## Wilson's Theorem

Instead of looking at powers, let's look at multiplication.

What happens if I multiply all residues $\mod{5}$?

$4 \cdot 3 \cdot 2 \cdot 1 \equiv 24 \equiv 4 \equiv -1 \mod{5}$

> Think first: Try doing this $\mod{7}$. What happens?

It turns out this is true for all primes, and importantly, only true for primes. This is called Wilson's Theorem. But why does this work?

Watch the video below for an explanation:

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/VLFjOP7iFI0?si=iB8kBtO5GTIqVJFF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

>Think about it: Why doesn't this work for composite numbers?