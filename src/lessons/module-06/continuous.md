# Continuous Probability

[Chapter 2](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=49)

Imagine a situation where there are infinitely many options, like a number line. How do we decide probabilities?

Instead of counting, we consider area. Watch the following video to see how (and why) we use area to calculate probability.

<div class=embed><iframe  src="https://www.youtube.com/embed/ZA4JkHKZM50?si=77V9ikh-jDdmrBWJ" title="Why 'probability of 0' does not mean 'impossible' | Probabilities of probabilities, part 2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

The problem in this video is a little more complex than needed. A classic continuous probability problem involves two friends trying to meet.

For some reason, two friends decide not to tell each other what time they will arrive at a local meeting spot. Each will arrive at some random time between 4:00 PM and 5:00 PM, however, they are impatient, and if the other person doesn't arrive within 15 minutes of their arrival, they will leave. What is the probability they actually meet?

We can represent one friend's arrival on the x-axis, and the other friend's arrival on the y-axis, then color the portion where they will meet.

Here is a [link to a desmos graph](https://www.desmos.com/calculator/r8aya6onao) of what this looks like.

Keep in mind the total possibilities is the square defined by $x=0$, $y=0$, $x=60$, $y=60$, since we assume they arrive sometime in that range. The total area of outcomes is $60^2$

To find the area of the favorable outcomes, it might be easier to find the area of the triangles and subtract. Each triangle is $\frac{1}{2}45\cdot 45$, but there are two, so the total area of "unfavorable" outcomes is $45^2$. Our probability will be $\frac{60^2 - 45^2}{60^2}$.

Our formula for continuous probability becomes

$\frac{\text{Area of Favorable Outcomes}}{\text{Total Area of Outcomes}}$

> Think about it: How does this compare to our counting definition for discrete probabilities? Does it make sense?
