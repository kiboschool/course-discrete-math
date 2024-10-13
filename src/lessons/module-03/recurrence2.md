## Examples of Recurrence Relation Problems

Other than Fibonacci, there are a few more famous recurrence relation problems. It can sometimes be difficult to see how a problem can be solved recursively. 

> Think about it: Try to think about each problem presented. What are some indications that the problem is recursive?

#### Number of Ways to Step

Suppose you are climbing a Mayan pyramid. These have many stairs, so you wish to save time. You can take one stair at a time, or you can skip some steps. The height of the stairs and the length of your legs mean you can either skip one or two steps when climbing the pyramid. How many different ways could you climb this structure, starting at the bottom?

First, we notice that once you make your decision on your first step size, you will have a number of stairs left based on the step you took. However, when this is accounted for, the same problem remains: what size will your next step be? This problem is recursive in nature.

Let $M(n)$ be the number of ways to climb $n$ stairs. Then, if you step once, you'll have $n-1$ stairs to climb ($M(n-1)$), if you skip a step, there will be $n-2$ steps ($M(n-2)$), and if you skip $2$ steps, there will be $n-3$ stairs left to climb ($M(n-3)$). Since we're counting the total number of ways to climb these stairs, we can simply add these values together.

The last step is to consider the starting values, which are really considering cases of a small number of stairs. If there are less than $3$ stairs, we can't skip $2$ steps, so let's consider $n = 1, 2, $ and $3$.

If there is $1$ step left, we can only climb the one step in one way. If there are two steps, we can either skip the middle one or climb them both, meaning $2$ ways in total. If there are $3$ steps, we can either skip $2$ and be done, or we can skip $2$, then climb $1$, climb $1$, then skip $2$, or simply climb them one at a time, leaving $4$ ways in total.

Our final recurrence is:

$$M(1) = 1, M(2) = 2, M(3) = 4$$

$$M(n) = M(n-1) + M(n-2) + M(n-3)$$

Which we'll notice is a Tribonacci-like recurrence.

#### Parenthesizing Multiplications

Suppose you have a list of things to multiply:

$$x_0 \cdot x_1 \cdot x_2 \cdot ... \cdot x_n$$

However, you want to determine how many ways you can parenthesize this multiplication. In how many ways can these be grouped? We consider an expression fully grouped if each set of parentheses have at most two terms in them. A term could be something inside a set of parentheses, or could be an $x_i$. For example:

$$ (x_1 \cdot ( ( x_2 \cdot x_3) \cdot x_4) \cdot x_5) $$

Is fully parenthesized. If any were removed, it wouldn't be.

Taking a look at the simplest examples:

One $x$ value on its own just needs a set of parentheses around it. The same for a set of two.

For a set of three, we can split the first term away, or the last term away to create one set. Then another set of parentheses around the whole thing.

In general, if we have $n$ $x$ values, we can split this into two smaller groups, then parenthesize these groups. We can split anywhere from just after the first value, to just before the last value, so any of the $n-1$ spots in between.

Let $S$ be our set of multiplications, with $S_{i, j}$ representing the subset of $S$ from the $i$th term to the $j$th term. We can show our recurrence is this:

$$ S(n) = 1, \text{ for } n = 1, 2$$
$$ S(n) = (S_{1,1} \cdot S_{2, n}) + (S{1, 2} \cdot S_{3, n}) + ... + (S_{1, n-1} \cdot S_{n, n}) $$

Where $n$ is the number of $x$ values in the multiplication. We multiply in each step since for each combinations of the first term, we can pair this with all combinations of the second. Then we add all of our cases of where we split.

> Check your understanding: Try to find the first few values of this recurrence (at least up to 10).

<details><summary>Check your answer</summary>

$1, 1, 2, 5, 14, 42, 132, 429, 1430, 4862$

</details>

> Think about it: Do these numbers make sense? You should notice a rapid growth in the value of $S(n)$. Does that align with the problem?

#### The Towers of Hanoi

The Towers of Hanoi is a problem based on a number of disks of decreasing size placed on one of three pegs. Watch the video below to learn more about it and understand its recursive nature.

<div class=embed><iframe  src="https://www.youtube.com/embed/2SUvWfNJSsM?si=cadiaMTIUGAEACRV" title="Binary, Hanoi, and Sierpinski: Part 1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

> Think about it: From the code given, can you write the recurrence relation for towers of Hanoi? Does this solve to $2^n - 1$, as expected from this video?

The second part of this video talks about a constrained version of this problem. It involves ternary and graphs, which we will visit again in later weeks. For now, focus on the recursive nature of the problem.

<div class=embed><iframe src="https://www.youtube.com/embed/bdMfjfT0lKk?si=OX11T2BeJtPu3Abv" title="Binary, Hanoi, and Sierpinski: Part 2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

> Think about it: If this is ternary, instead of binary, what happens to the solution? Can you figure out what the recurrnce looks like in this constrained case?