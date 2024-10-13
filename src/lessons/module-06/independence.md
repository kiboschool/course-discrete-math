## Independence
[Chapter 4](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=147)

Since probabilities on a finite set of outcomes involve counting, we often add or multiply probabilities.

## Combining Probabilities: Addition

The probability of rolling a 1 or a 6 on a fair 6-sided die is the probability of rolling a 1 plus the probability of rolling a 6.

By definition: $P(1 \text{ or } 6) = \frac{2}{6}$

By addition: $P(1 \text{ or } 6) = \frac{1}{6} + \frac{1}{6} = \frac{2}{6}$

However, just like with counting, we need to be careful.

What is the probability of drawing a red card or a card labeled "k" from our Kibo deck?

> Think first: What do you think the answer will be?

If we just add as before, we would have $\frac{20}{120} + \frac{30}{120} = \frac{50}{120} = \frac{5}{12}$

If we follow the definition, to count the number of cards labeled "k" or red cards, we would need to follow the principle of inclusion-exclusion.

$20 + 30 - 5 = 45$

The probability would be $\frac{45}{120} = \frac{3}{8}$

We have two different answers!

> Think first: Can you find the mistake in the first method?

When adding probabilities, the principle of Inclusion-Exclusion applies! There's an overlap in the events of "drawing a red card" and "drawing a card labeled 'k'," which needs to be removed.

The formula for finding probabilities of event $A$ or event $B$ happening, is therefore:

$P(A \cup B) = P(A) + P(B) - P(A \cap B)$

Note that when $A \cap B$ is empty (the events have nothing in common), $P(A \cap B)$ will be zero! This means that this formula works regardless of whether or not the events overlap. When $P(A \cap B)$ is zero, $A$ and $B$ are called **Mutually Exclusive** or **Disjoint**.

## Combining Probabilities: Multiplication

The probability of rolling a 1 and then a 6 is the probability of rolling a 1 times the probability of rolling a 6.

Multiplying: $\frac{1}{6} \cdot \frac{1}{6} = \frac{1}{36}$

Definition: $\frac{1}{36}$, since there are $36$ different ordered dice rolls.

However, we need to be careful.

Consider the probability of drawing a red card, then an orange card.

Multiplying: $\frac{20}{120} \cdot \frac{20}{120} = \frac{1}{6} \cdot \frac{1}{6} = \frac{1}{36}$

Definition: $\frac{20 \cdot 20}{120 \cdot 119}$, since drawing a red, then an orange is $20 \cdot 20$ and drawing any two cards is $120 \cdot 119$.

These are once again different!

When events do not effect each other, they are called **Independent**. Two events, $A$ and $B$ are independent if

$P(A \text{ and } B) = P(A) \cdot P(B)$

If this is not true, events are considered dependent.

> Think first: Why didn't multiplying work here? Is there a way you could fix what we did, like we did for addition?