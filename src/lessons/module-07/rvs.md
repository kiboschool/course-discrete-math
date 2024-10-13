# Random Variables

Random Variables are a probabilistic/statisical tool to discuss probability of events, usually continuous probability, but sometimes even discrete random variables can be useful.

## Readings

[Introduction to Probability](https://math.dartmouth.edu/~prob/prob/prob.pdf)

## Random Variable Defintion
[Chapter 1.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=9)

Random Variables, just like normal variables take the place of a value. In the case of Random Variables, their value is the outcome of an event.

For a die roll, a random variable could hold any integer value between 1 and 6 (inclusive).

For a coin flip, the value would be heads or tails.

When drawing a card, the value might be the numerical value if that's what we're considering. With Random Variables we almost always consider a numerical value.

Unlike normal variables, we usually do not solve for the value of random variables. Instead, we talk about their properties and use them as placeholders for the outcome of an event.

### Discrete/Continuous Random Variables
[Chapter 1.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=9)
[Chapter 2.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=49)

Just like probability problems, Random Variables can be made to reference discrete probabilities or continuous probabilities. For discrete probabilities, like the ones described above, it is easy to say what values a random variable might take on, and how likely it is to take on that value.

For continuous probability problems, this information is often visualized with probability density function. As discussed in the last module, this describes the probabilities over a range of values, which we can calculate by finding the area. Usually this is done with integrals, so we won't be solving any that require integration, but it's useful to know about this method of displaying probability.

## Expected Value of RVs
[Chapter 6.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=233)

The expected value of a random variable is simply the expected value of the event it is associated with. For example, the expected value of a random variable representing a standard, fair 6-sided die roll would be 3.5, as we've calculated before.

Since random variables are a placeholder, all the calculations we complete with them just reference the event, and the probabilities associated with the event.

## Variance
[Chapter 6.2](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=265)

The variance of a probability distribution (or of a random variable) measures how varied the results of the event are or can be. This is measured by squaring the difference between each outcome and the mean, then taking the average of these numbers.

For example, the variance of rolling a standard, fair, 6-sided die is

$Var(X) = [(1 - 3.5)^2 + (2 - 3.5)^2 + (3 - 3.5)^2 + (4 - 3.5)^2 + (5 - 3.5)^2 + (6 - 3.5)^2]/6 \approx 2.92$

The variance of choosing a random integer between 1 and 10 inclusive is $6$.

> Think about it: try to calculate this value.

When there are more options, there is more variance. Likewise, when the options are spread out more, there is more variance.

## Sums of Random Variables
[Chapter 7.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=293)
[Chapter 9](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=333)

Below is a required video that is a part of the readings this week. Feel free to pause, rewind, or take notes as needed.

<div class=embed><iframe  src="https://www.youtube.com/embed/zeJD6dqJ5lo?si=htGMpNnuaxYTEX3s" title="But What is Central Limit Theorem?" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

> Think about it: Try computing the 95% bounds for 1,000 die, for 10,000 die, and for 10 die. Combined with the 100 die example from the video, what do you notice?
