# Counting Principles

There are two basic counting principles that are the basis of combinatorics. This information should largely be review from Mathematical Thinking, but perhaps a different way of thinking about the basics of combinatorics.

# Readings

[Discrete Mathematics: An Open Introduction](https://discrete.openmathbooks.org/dmoi3/ch_counting.html), [Chapter 1.1](https://discrete.openmathbooks.org/dmoi3/sec_counting-addmult.html) and [Chapter 1.3](https://discrete.openmathbooks.org/dmoi3/sec_counting-combperm.html)

## Counting as Sets

Research (Lockwood, 2014: A set-oriented perspective on solving counting problems) shows that thinking of problems as sets of outcomes can help develop the skills necessary to correctly apply combinatorial strategies. While the strategies themselves won't be discussed for a few sections, try to make sure as you're thinking through problems that you form a set of the desired outcomes (things you want to count), and consider how you might find the cardinality of this set.

## Addition Principle
[Chapter 1.1](https://discrete.openmathbooks.org/dmoi3/sec_counting-addmult.html)

> Remember: Please read the text linked above before reading the material below.

When events are disjoint, meaning they do not overlap, we can **add** the number of possibilities for each event together to find the total number of ways any of these events occur. This is the mathematical definition, the meaning is quite simple, just hard to apply.

As a reminder: "event" is just a mathematical term that refers to something happening. It could be drawing a card, drawing multiple cards, rolling a die, catching a fish, or lightening striking.

Therefore, this definition translates as "if there are multiple things that could happen, but they will not occur at the same time, we can use the addition principle. We can count the number of ways each thing could happen and add each of these values to find the total number of ways _any_ of these things could happen."

For example, imagine we have a deck of cards where there are 5 cards labeled 1 to 5 for each of these colors: red, orange, yellow, green, blue, and purple. We'll use this deck instead of a "standard card deck" to avoid confusion.

How many ways could a person pick a red or an orange card?

> Think first: What do you think the answer is?
> What are our sets of outcomes?

There are 5 red cards and 5 orange cards, these each being our desired sets with their cardinalities. In this deck, no card is red and orange (there is no element in the intersection), so we can just add these numbers. There are 10 ways to pick a red or an orange card.

> Check your understanding: Can we used this method for the question "how many ways could a person pick a red card or a card labeled 5"? Why or why not?

<details><summary>Check your answer</summary>
This cannot be done exactly the same way, since there is a red card labeled 5! We'll find ways to handle these issues soon.
</details>


## Multiplication Principle
[Chapter 1.1](https://discrete.openmathbooks.org/dmoi3/sec_counting-addmult.html)

> Remember: Please read the text linked above before reading the material below.

When events are independent, meaning each event does not effect any other events, and for each event, there are a certain number of outcomes for every other event, we can multiply the number of ways each event can happen.

This principle is a little more complicated, so let's break it down.

We have multiple events occuring, they might happen at about the same time, but for the multiplication principle, it's best to think of them sequentially, or one right after the other.

For example, if you can order 3 different kinds of meat, 4 different kinds of cheese, and 7 different kinds of vegetables on a sandwich, choosing each ingredient to be added is an event, and while they can be done in any order, or can even be added to a sandwich all at once, it's easiest to pick an order and stick to it.

First, we choose the meat. There's 3 ways to do this. For each meat, we could choose any of the 4 kinds of cheese, so we multiply these events. Likewise for the 12 sandwich types we have, we can add one of 7 different types of vegetables to each. Therefore, there are $12 \cdot 7 = 84$ different ways to make a sandwich if we can only pick one of each ingredient.

> Check your understanding: If you were allowed to pick two vegetables, but they had to be different, could you still use the multiplication principle? What if you could pick any two vegetables, including the same one twice?

<details><summary>Check your answer</summary>
If the vegetables have to be different, that effects our choice. If we pick one vegetable, now only 6 others remain. Don't worry, we'll fix this issue as well, though this is considered a part of the multiplication principle.

However, if we can just pick the same vegetable twice, there are always just $7$ choices. Therefore, we'd multiply by another $7$ to get $588$ different types of sandwiches.
</details>

> Think about it: What are some clues a problem should be solved using addition principle? What about multiplication principle?
> Can you form some general rules that determine which method should be used?