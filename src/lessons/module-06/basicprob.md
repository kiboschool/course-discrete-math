# Basic Probability Definitions

## An Intuitive Definition

Imagine you have a six-sided die. What's the probability of rolling a one? What is the probability of rolling an even number?

> Think first: Answer these!

There are 6 options on the die, only one is a one, so there is a $\frac{1}{6}$ chance of rolling a one.

Likewise, there are 3 even numbers on the die, so there should be a $\frac{3}{6}$ or $\frac{1}{2}$ chance of rolling an even number.

As it turns out, these are the correct probabilities! In easy cases of dice, coins, and cards, finding the probability is simple.

> Check your Understanding: What is the probability of flipping a head on a fair coin? What is the probability of drawing a red card from our KIBO deck in the previous section? What is the probability that the sum of two 6-sided dice is 7?

<details><summary>Check your answer</summary>
Head: $\frac{1}{2}$
Red Card: $\frac{20}{120}$ or $\frac{1}{6}$
Sum: $\frac{6}{36}$ or $\frac{1}{6}$
</details>

> Think about it: The red-card probability can be found by counting all red cards and all cards in total, but is there an easier way to think about the problem to get the answer of $\frac{1}{6}$?

Imagine a die with 2 ones, 2 twos, and 2 threes.

> Think first: What is the new probability of rolling a one with this die?

There's a $\frac{1}{3}$ chance of rolling a one this time, from $\frac{2}{6}$.

What changed? To define probability better across all situations, we should use mathematical terms.

## Mathematical Definition of Probability

If we have a discrete set of equally likely outcomes, we can consider probability in the following way:

Let $S$ be our **sample space**, which is a set that contains all possible outcomes.

We can define the probability of an event, $e$ as

$p(e) = \frac{\text{Number of outcomes in }e}{\text{Total number of outcomes in }S}$

This is sometimes also written as

$\frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}}$

These definitions line up with how we intiutively decide probability above! But note that it has some conditions.

1. There needs to be a finite number of outcomes.
2. These outcomes must be equally likely.

On our die with only 1, 2, and 3, the outcomes are still equally likely, so we can use this definition. However, what if the die had only one 3 and three 1s?

> Think first: What do you think the probability is?

Half of the numbers on the die are 1, so this should be $\frac{1}{2}$

With this example, we can change the problem slightly to have something that fits the definition better.

Pretend each face of the die is a different color. That way, we have different outcomes for each face. Then, all outcomes are equally likely, so we just have to sum the ones that are favorable: the three faces that have a one on them.

Some problems can be adapted, but some cannot. For example, if I just told you I had an unfair die, and no other information, you could not find the probability. If I told you there were 3 ones, but did not tell you the die had 8 sides, you would get an incorrect result.

Knowing all of the faces, or at the very least, all of the relevant faces and the total number of faces on the die, allows us to know what all the outcomes are, and if we assume the die is fair, know how likely each face is to appear.

> Think about it: If you were told a coin flipped heads 70% of the time, could you figure out the probability it flips tails? How would you do so?

## Rules of Probability

There's also an unsaid, but important, condition that all possible probabilities over a sample space should sum to 1. Intuitively, this should make sense, the probability of a coin flipping either heads or tails should be 100%. In the case of finite outcomes, this is especially important, and it is something to consider with continuous probability, which we will discuss later.

> Think about it: Convince yourself that this condition is satisfied by the definitions above.