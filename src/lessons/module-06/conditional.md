## Conditional Probability
[Chapter 4](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=141)

Conditional probability allows us to find the probability of an event given that another event has occurred. There are two ways to think about this type of event. It could be true that a physical change from the first event effects the second event. It could also be true that if the first event is true, or falls into a certain category, it changes the probability of the second event. For this section, we'll focus on the first type, as the second will be covered in the section on Bayes' Theorem.

For example, when drawing cards from a deck, if we don't place the cards back, the chance we pull a certain type of card changes each draw. Not only does the size of the deck change, but we could pull a card in the category of what we would like to draw next.

What is the probability you draw a red card as your second card?

This depends:

If your first card was not red, then it should be $\frac{20}{119}$ for the 20 red cards remaining in the deck of 120 minus the first card you drew.

If your first card is red, then it should be $\frac{19}{119}$ for the 19 red cards left in the deck of 119.

Each of these separately is a conditional probability. The first is the chance of drawing a red card given that you've drawn a non-red card, and the second is the chance of drawing a red card given that you have drawn a red card already.

While this answers the question of what conditional probability is, how do we combine these into one probability?

> Think first: What do you think you should do?

The conditional probabilities assume the event has already occurred, so we need to bring in the probabilities of the first events themselves.

The overall probability of drawing a non-red card, then drawing a red card is $\frac{100}{120} \cdot \frac{20}{119}$

The overall probability of drawing a red card, then drawing another red card is $\frac{20}{120} \cdot \frac{19}{119}$

Since these events do not have anything in common, we can add them to get the total probability.

$\frac{100}{120} \cdot \frac{20}{119} + \frac{20}{120} \cdot \frac{19}{119} = \frac{100 \cdot 20}{120 \cdot 119} + \frac{20 \cdot 19}{120 \cdot 119} = \frac{100 \cdot 20 + 20 \cdot 19}{120 \cdot 119} = \frac{100 + 19}{6 \cdot 119} = \frac{1}{6}$

Note that it's the same probability as drawing a red card from the deck.

> Think about it: Can you figure out why the probability the second card drawn is red is the same as the probability that the first card drawn is red?

Conditional probability is denoted with a bar (|) read as "given", so the probability of $A$ given $B$ would be denoted:

$P(A|B)$

We can also note here that this provides the solution we needed to our multiplication problem!

$P(A \cap B) = P(A|B)\cdot P(B)$

Note that we can do this both ways:

$P(A \cap B) = P(B|A)\cdot P(A)$

Just like with addition, if there's no change from the first event happening, then

$P(A|B) = P(A)$

Since the probability is unaffected.

> Check your understanding: What is the probability that the sum of two dice is even? Try doing this by calculating the probability the sum is even when the first die is odd, and the probability the sum is even when the first die is even. Does the answer make sense?

<details><summary>Check your answer</summary>

$P(\text{Sum is even} | \text{First die odd}) = \frac{1}{2}$, since we need another odd number.

$P(\text{Sum is even} | \text{First die even}) = \frac{1}{2}$, since we need another even number.

$P(\text{Die rolls even}) = P(\text{Die rolls odd}) = \frac{1}{2}$.

So the total probability is $P(\text{Sum is even} | \text{First die odd}) \cdot P(\text{Die rolls odd}) + P(\text{Sum is even} | \text{First die even}) \cdot P(\text{Die rolls even}) = \frac{1}{2} \cdot \frac{1}{2} + \frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4} + \frac{1}{4} = \frac{1}{2}$

This should make sense, as it's just 50/50 odds of rolling even or odd in the first place. The sum is no different.

</details>