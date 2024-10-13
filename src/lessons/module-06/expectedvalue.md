# Expected Value
[Chapter 6.1](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=233)

## Expected Value

The expected value is almost exactly what it sounds like. The expected value results in the average value that is expected if something happens many times. It could be the most likely outcome, or it could be a value that is impossible to achieve.

When rolling a standard, fair 6-sided die, what is the expected value?

> Think first: What do you think it is?

The middle value is between 3 and 4 so a good guess might be either 3 or 4, or to split it, 3.5. It turns out that 3.5 is, in fact the answer. We can calculate this by computing a weighted average.

$\frac{1 + 2 + 3 + 4 + 5 + 6}{6} = \frac{21}{6} = \frac{7}{2}$

This works because each option is equally likely. What about our die with three ones, two twos and one three?

For each value, we can multiply it by the probability it happens, which also gives a weighted average. You'll notice this is what we also did in the previous problem, since all values were divided by $6$.

$\frac{1}{2}1 + \frac{1}{3}2 + \frac{1}{6}3 = \frac{1}{2} + \frac{2}{3} + \frac{1}{2} = \frac{5}{3}$

> Think about it: Does $\frac{5}{3}$ make sense as an answer here?

In general, the formula for the expected value of discrete probability problems is

$\sum_{x \in S} p(x) \cdot x$

Where $S$ is the sample space, $x$ represents an outcome, and $p(x)$ is the probability of $x$.

This can apply for situations where sets of outcomes and associated probabilities are given.

For example, assume we are told that a college class has 21 20-year olds, 23 21-year olds, 11 22-year olds, and 3 31-year olds. If you choose a person at random, what do you expect their age to be?

$\frac{21}{21+23+11+3}\cdot 20 + \frac{23}{21+23+11+3}\cdot 21 \frac{11}{21+23+11+3}\cdot 22 + \frac{3}{21+23+11+3}\cdot 31$

If we use a calculator, we find this to be about 21.34.

> Think about it: Does this answer make sense?

## Recursive Games

Expected value can sometimes be calculated for recursive probability problems.

Imagine a game where you roll a die and you recieve the value you roll, except if you roll a 1, in which case you add one to your current value, then roll again.

> Think first: Make an estimate of what you think the expected value should be.

The expected value is

$E = \frac{1}{6}2 + \frac{1}{6}3 + \frac{1}{6}4 + \frac{1}{6}5 + \frac{1}{6}6 + \frac{1}{6}(1 + \text{ rolling again })$

Note that when you roll again, the expected value is exactly the same formula, so we can replace "rolling again" with $E$

$E = \frac{2}{6} + \frac{3}{6} + \frac{4}{6} + \frac{5}{6} + \frac{6}{6} + \frac{1}{6}(1 + E)$

$E = \frac{20}{6} + \frac{1}{6}(1 + E)$

$6E = 20 + 1 + E$

$5E = 21$

$E = \frac{21}{5}$

This is a little over $4$, which is not much more than the original expected value for a die roll.

> Think about it: Does this make sense?

## Continuous Expected Value

As mentioned in the continuous probability section, sums turn into integrals. The same happens with expected values!

Since calculus is not a prerequisite, we won't go into any more detail here.