# Counting Strategies

We can use the basic principles along with factorials, combinations, and permutations to solve many different types of problems. There are many strategies to solve counting problems, and we'll discuss the most important ones here.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Discrete Mathematics: An Open Introduction](https://discrete.openmathbooks.org/dmoi3/ch_counting.html), [Chapter 1.2, 1.4-1.7](https://discrete.openmathbooks.org/dmoi3/sec_comb-proofs.html), [Chapter 5.1](https://discrete.openmathbooks.org/dmoi3/sec_addtops-genfun.html)

[Applied Discrete Structures](https://discretemath.org/ads/chapter_2.html)[Chapter 2.3-2.4](https://discretemath.org/ads/s-combinations-and-the-binomial-theorem.html), [Chapter 8.5](https://discretemath.org/ads/s-generating-functions.html)

## Casework

In problem solving, a common strategy is to break a problem into parts. In combinatorics, we call this casework when the parts are non-overlapping.

When we count a problem by parts, where each part has nothing in common with any other part, we can use the _addition principle_ to add up all of our values at the end.

For example, imagine drawing 3 cards from our kibo deck. How many ways could you draw at least 2 red cards?

If we need at least 2 red cards, 2 of the 3 could be red or 3 of the 3 could be red. So we can use these as our cases.

Case 1: How many ways are there to draw exactly 2 red cards in a hand of 3?

There are 20 red cards, and 100 cards that are not red. We can choose a red card, then another red card, then a card that's not red to get exactly 2 red cards in our hand.

Note that when we take one red card, there will only be 19 left, so we'll have to remember that when we multiply.

> Think first: What do you think the answer is?

When we have a few cards in our hand, the order does not matter, so we need to do a combination rather than a permutation on the red cards.

$$\frac{(20 \cdot 19)}{2} \cdot 100$$

While we could multiply these values and get a final result, we are starting to see values that will be large.

> In combinatorics, it's often worthwhile to leave final answers as a series of multiplications or additions, as long as there aren't too many.

So, we'll continue to the next case.

Case 2: How many ways are there to draw exactly 3 red cards in a hand of 3?

Even simpler here, the answer is ${20 \choose 3}$, as we just need to choose 3 red cards of the 20 possibilities.

Since these cases have nothing in common, we can add them to get the final solution.

$$\frac{(20 \cdot 19)}{2} \cdot 100 + {20 \choose 3}$$

This is the number of ways to draw 3 cards where at least 2 of the cards are red.

## Complementary Counting

> Think first: What would the universe minus $A^c$ be?

This would just be all things in A!

For counting problems, we can use this strategy to count the number of items in A, where A is the set of all events that follow the requirements of the problem.

First we count the universe (total), then the complement of A (all events that are not A), and we subtract to find the number of events that fit in set A.

For example, imagine we were asked instead how many ways a person could have fewer than 2 red cards in their hand out of 3 cards drawn.

We could do casework again for 0 or 1 red cards, but we've already computed the number of ways to get 2 or 3 cards, and we can use it here!

We also need to determine our universe. In total, we are pulling 3 cards from our deck of 120, so the number of total 3 card draws is ${120 \choose 3}$.

If we subtract the number of draws with 2 or 3 red cards, then we should only have sets which have less than 2 red cards!

Our answer is ${120 \choose 3} - (\frac{(20 \cdot 19)}{2} \cdot 100 + {20 \choose 3})$.

> Think about it: Try solving this problem using casework, then use a calculator to compute your answer and the one above. Did they match?

This is an example of using complementary counting when we already computed a value, but it's also useful for certain questions on their own.

For example, what if I asked the number of ways to draw 2 or more red cards in a hand of 10? It would be far easier to compute the two cases of 0 red cards and 1 red cards, then the cases of 2, 3, 4, or 5 red cards. Keep this in mind when deciding what strategy to use to solve a combinatorial problem.

Remember when we asked how many ways there were to draw a red card, a 5, or a card with a k?

We could also look for what's not included. The negation of this statment is not red and not a 5 and not a k. This allows us to use multiplication principle since we can break it down into stages. $(6-1) \cdot (5-1) \cdot (4-1) = 60$. $6-1$ for $6$ colors, minus red, $5-1$ for 5 numbers minus the five, and $4-1$ for 4 letters, minus the k. Note that $120 - 60 = 60$ which was our answer from earlier.

Sometimes using complementary counting allows us to change our technique. Here, we multiplied instead of adding and subtracting, and it was a fewer steps. When it comes to solving problems, both ways are valid, but if you want to be the fastest, identifying the best method will help. This is similar in nature to choosing which algorithm will best suit a problem. You have to identify which algorithms could be used, then decide based on the problem which will be most efficient. Eventually, many people develop an intuition, but this takes time and practice.