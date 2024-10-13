# Inverses in Modular Arithmetic

## Readings

No readings for this section yet, as there are some advanced topics we will discuss later to help with inverses.

## Normal Inverses

In mathematics, we do have multiplicative inverses for almost every number!

$2 / 2 = 1$

$3 / 3 = 1$

$\frac{2}{5} / \frac{2}{5} = 1$

The problem is that this involves division.

>Think first: How can we complete this idea without division?

## Modular Inverses

Instead of dividing, we'll take the idea of multiplying by the reciprocol.

$2 / 2 = 2 \cdot \frac{1}{2} = 1$

The problem still remains that we don't have fractions in our mod world, so we define a new term.

A number, $a^{-1}$ is called the modular inverse of $a$ $\mod{n}$ if

$a \cdot a^{-1} \equiv 1 \mod{n}$

Note that this definition depends on $a$ and $n$, so for example,

$3^{-1} \equiv 2 \mod{5}$, since $3 \cdot 2 = 6 \equiv 1 \mod{5}$

However, 

$3^{-1} \equiv 5 \mod{7}$, since $3 \cdot 5 = 15 \equiv 1 \mod{7}$

I found these equivalences for us, can you find the inverse for the following?

$3^{-1} \mod{11}$

This gets harder as the mod gets bigger, but with $11$, we can still just guess and check, as there are only $11$ distinct residues $\mod{11}$

$3 \cdot 1 = 3$

$3 \cdot 2 = 6$

$3 \cdot 3 = 9$

$3 \cdot 4 = 12$

We can stop here! $12 \equiv 1 \mod{11}$

>Think first: What happens if you try to find $3^{-1} \mod{6}$? Can you form a general rule for when you think this problem will occur?

## Does an Inverse Exist?

Watch the following video, which starts with the same material here, but ends with reasoning as to which numbers have inverses.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/6kVjaDJh9QM?si=YaFbfNapaczk2CI9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>