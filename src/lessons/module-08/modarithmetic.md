# Modular Arithmetic

It's important to understand how we can manipulate modular equivalences while keeping the equivalence. We have similar rules to algebra, with a few notable differences.

## Readings

[Chapter 4](https://math.gordon.edu/ntic/ntic/chapter-intro-congruence.html)

## Modulo: An Equivalence Relation

As it turns out, numbers mod n form an equivalence relation. This means many rules used in standard equality can apply here, but we must be careful.

### Addition

Just like in normal equations, we can add the same number to both sides and the equivalence holds. We'll work $\mod{10}$ since for most numbers, the last digit tells us the remainder. We'll revisit why I said "most" at the end.

$3 \equiv 13 \mod{10}$

$7 \equiv 17 \mod{10}$

$10 \equiv 20 \mod{10}$

We can also do more. We can add _equivalent_ numbers to both sides of a congruence.

Since $n$ is always equivalent to $0 \mod{n}$, we can always add $n$ to any side, without adding $n$ to both sides, since adding zero to the other side would just give the same number.

$3 \equiv 13 \mod{10}$

$13 \equiv 13 \mod{10}$

We can even add multiples of $n$!

$23 \equiv 13 \mod{10}$

Likewise, even if we have just one number, it's always fine to add zero (or the equivalent of zero) just like real numbers. Adding any multiple of $n$ will not change final value. It will always have the same residue!

$3 \equiv 13 \equiv 23 \equiv 33 \mod{10}$

This allows us to easily convert negative values into positive by adding copies of $n$ until we reach the residue.

$-17 + 10 + 10 \equiv 3 \mod{10}$

Note that the rule of "last digit determines the remainder mod $10$" does not work with negatives!

### Subtraction

Similar to addition, we can subtract equivalent values on either side, and subtracting zero (or values equivalent to zero) does nothing to the residue of the number.

This should make sense, as subtraction is just adding a negative value. Since we have negative values and addition, all the properties still hold true.

### Multiplication

Multiplication is similar as well: We can multiply equivalent values, but instead of multiplying by zero, we can multiply by $1$ (or equivalent values) to keep the original number's residue equivalent.

This should mostly make sense, as multiplication is just repeated addition. Instead of multiplying by $3$, we could add the same value to itself $3$ times!

The multiplication by $1$ is similar to real numbers multiplication, but let's make sure it works by using our quotient-remainder form. Let $b$ be a number which is equivalent to $1 \mod{n}$.

$a = k \cdot n + r$

$b = j \cdot n + 1$

$a \cdot b = (k \cdot n + r)(j \cdot n + 1) = kjn^2 + jrn + kn + r = (kjn + jr + k)n + r$

Since the last result is an integer times $n$ plus $r$, it has the same remainder as $a$!

### Division?

With division, we have a tricky problem. We can't have fractions as a remainder, so fractions simply don't exist in a modulus.

This means we can't just divide normally, as much as we'd like to do so.

Even in cases where it looks like we can divide evenly, the result might not be true. Consider:

$4 \equiv 6 \mod{2}$

$2 \not\equiv 3 \mod{2}$

We'll figure out how to handle this in the next section.

## Another Way to Look At Mod

This video showcases another way to view modular arithmetic that may help you think about mods in a more visual way.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/Nd3psPoGww8?si=nv9ugWmzm9GN412M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

>Think first: How would you preform addition, subtraction, and multiplication on this clock?