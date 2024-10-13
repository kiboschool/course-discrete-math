# Statistics 

Statistics is the science of probability. Using mathematical methods, we discuss what is or isn't likely to happen based on data, and define some new, helpful terms.

## Readings

[Introduction to Probability](https://math.dartmouth.edu/~prob/prob/prob.pdf)

## Mean, Median, Mode, Range

If you are given a list of numbers, and are told these are outcomes from a repeated event, what can you do with them?

### Mean

The mean of a set of numbers is simply the average. This tells us some information about the expected value, but does not give much information on its own.

### Median

The median of a set of numbers is the middle value, when ranked highest to lowest. Combined with the mean, we can use this to say some things about the distribution of values.

If the median is larger than the mean, that means there must be some very small numbers weighing the mean down.

If the median is smaller than the mean, the opposite must be true: some large values are making the mean larger.

If the mean and median are close to the same number, we can assume a relatively even distribution sometimes. However, we cannot guarantee this.

### Mode

The mode of a set of numbers is the most common value. If there are multiple that are just as common, they are all considered modes. The mode, and the number of values that are equal to the mode, can tell us some information as well.

### Range

The range of a set of numbers is the difference between the largest and smallest value. This tells us how wide our distribution is (roughly), though it doesn't tell us any information about how values are distributed between these points.

> Check your understanding: Go to [random.org](https://www.random.org/coins/) and flip 10 coins, keeping track of the number of heads that come up in the 10 flips. Do this at least 10 times, recording the numbers, then calculate the mean, median, mode, and range.

<details><summary>Check your answer</summary> 

I preformed this 20 times, getting the following results:

5, 4, 7, 3, 6, 3, 7, 8, 6, 6, 4, 3, 7, 5, 7, 5, 5, 5, 5, 8

Mean: 5.45

Median: 5

Mode: 5

Range: 5

These were remarkably consistent for me, but see what you find!

</details>

## Law of Large Numbers
[Chapter 8](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=313)

The Law of Large Numbers is a probability theorem that is very useful for statistics. There's a lot of mathematical terms in this theorem that I don't expect you to fully comprehend, but the big picture is important.

This theorem basically states if you have a process that happens many times (a large number of times), the mean of the values should be equal to the expected value generated probabilistically. Larger numbers should have means that get closer and closer to the expected value.

>Think about it: Try using the random.org coin flipper or dice roller 5, 10, 20, and 50 times (you can just do 50 times and use the first 5, 10, 20 values). Find the mean of each of these sets of numbers. How close is each to the true expected value?

## Confidence Intervals

Confidence intervals are another statistical tool which provides a range of values that you expect the result of an event to fall between. If this sounds familiar, it should be, as it was in the Central Limit Theorem video!

Confidence intervals are usually 95% or 99% based on the standard deviation of the normal distribution, though other values can be made using integration or specific tables.

These confidence intervals simply state an interval, then the confidence level (percent likelihood) that a new value will fall in this range.

Calculating these is a bit beyond the scope of this course, but there are tons of resources on this topic, and if you'd like to do a project on statistics, this may be a topic you could discuss!