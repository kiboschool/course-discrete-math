# Modulo

You are likely already familiar with the idea of mods, but let's make sure you know all of the ways we can define mod!

## Readings

[Chapter 4](https://math.gordon.edu/ntic/ntic/chapter-intro-congruence.html)

## What is a mod?

The first definition we often hear for modulo is that two numbers are the same mod n if they both have the same remainder when divided by n.

This definition serves us well, but doesn't express the nature of modulo nor help us identify when it might be useful.

Suppose I ask you what day of the week your birthday will be on next year? What about in 10 years? What was the day of the week the day you were born?

If you've got a calendar, you can easily find your birthday this year, and it may even be easy to find the day of the week next year, but past that would take a lot of scrolling or future calendars.

Instead, we can recognize the year is a cycle of 365 days, and every 7 days the day of the week repeats.

The number of days until your next birthday will be 365 (most of the time), then we can explore how many weeks will occur in between. When we find out the number of days left over, we can find the day of the week.

This problem can be easily solved through modular arithmetic. Take the number of days until your next birthday, and divide by 7. If you get a remainder 0, it should be the same day you started on! Remainder 1 will be the next day, 2 will be two days after, and so on until a remainder 6 gives you 6 days later, and allows us to easily think about negative remainders.

The day that is 6 days after Monday is Sunday, but it's easier to describe this day as yesterday. This is one step back, or a negative $1$, meaning

$6 \equiv -1 \mod{7}$

Modulo can be used to solve many problems that are related to **cycles**, even ones which are not necessarily numeric, like days of the week.

## Modulo

Two numbers, a and b, are considered **equivalent** modulo n when certain criteria are met. We also sometimes call this a "congruence" modulo n. The below video shows a few different ways we can define what modulo means.

<div class=embed><iframe width="560" height="315" src="https://www.youtube.com/embed/6dZLq77gSGU?si=jaX4T8qubrmHuUPD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

To be clear: This relationship is symmetric, meaning all the rules written still apply when $a$ is swapped with $b$, for example:

$10$ and $14$ still obviously have the same remainder.

$14 = 4 \cdot 1 + 10$

$4 | (14 - 10)$

But let's discuss each of these definitions a little more.

### Remainder Definition

While we referenced this definition at the very start, we should discuss it more mathematically.

Similarly to the second rule, we can remember our quotient-remainder form and know that if $a \equiv b \mod{n}$, then

$a = k \cdot n + r$

$b = j \cdot n + r$

Where $k, j, r$ are integers, and in particular, $0 \leq r < n$ since $r$ is a remainder.

This allows us to create that second defintion, with a little algebra manipulation.

$a = (k-j)n + b$

>Think about it: Verify that this definition works from the equations above.

### Difference Definition

This definition is commonly used in proofs, because it can be helpful to know what things divide rather than their remainders.

We can also get this definition from the quotient-remainder form:

$a - b = k \cdot n + r - (j \cdot n + r) = k \cdot n - j \cdot n + r - r = (k-j)\cdot n$

When subtracted, the remainder cancels, leaving a result that is divisible by $n$.

### Addition in Modulo

This video also touches on adding something to both sides. We'll cover this topic more thouroughly in the next section.

## Residues

While we can have any number in a modulus, sometimes we like to reduce that number to its remainder. This is called the **residue** of a number, mod $n$.

The residue of $10 \mod{4}$ is $2$, and the residue of $14 \mod{4}$ is also $2$, which is why they are equivalent.