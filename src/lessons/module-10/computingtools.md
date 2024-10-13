# Computing Tools

We often use tools when programming, but we should be thinking deeper about why we can use them, where they come from, and why they work.

## Random Number Generation

(Psuedo) Random number generation can be done via a modulus. Watch the video below for a basic idea:

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/BYR5sbJHqsU?si=7NF5-DWinP97qCnQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

We can also find "random" numbers according to a distribution, like the normal distribution.

First, we generate a random value between 0 and 1. This could be some string of digits after a decimal.

Then, we look at a graph of the normal distribution. In particuluar, we look at the CDF, if you already know that name. What this graph shows is the probability that any value lower than x would appear. For example, if the mean of our normal distribution is 1, then there is a 50% chance that any random value that appears would be less than that. So the graph would line up at (1, 0.5).

We then use this random number to go backwards to get a value. For example, if our randomly generated number was 0.5, we would return 1, since that is the value we stated above.

If we think about this, it should make sense. There should be a cluster of similar values that get around 0.5 on our graph, and therefore, we have more values around the center, which is what we want for a normal distribution.

If we want a specific distribution of random numbers, we can also use something called Acceptance-Rejection method. This method works when we can't find the graph as described above, or if it's hard to calculate.

This method is a little more complex, but the basic premise is this: you generate a random number, then "test" to see if it fits your distribution. If it doesn't, you reject it and try again, if it does, that's your output.

## Data Structures

As mentioned previously, graphs, and in particular trees, are a common data structure in computer science. There are other mathematical structures used as well, but the majority of the rest of mathematics completed in data structures is about time complexity.

Finding the time complexity often involves solving a recurrence, something we discussed back in week 3.

I won't go into too much detail here, as these topics should be covered more thoroughly in DSA 1 and 2. However, the video below gives an interesting application.

I encourage you to try to think of the solution first, before the video continues.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/4NKlKyO5Jr0?si=6az1f6q7lVC4GDBo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

> Think about it: What do you remember from DSA 1 that we discussed here?