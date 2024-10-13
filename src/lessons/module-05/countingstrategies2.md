## Sticks and Stones / Stars and Bars
[Chapter 1.5](https://discrete.openmathbooks.org/dmoi3/sec_stars-and-bars.html)

> Remember: Please read the text linked above before reading the material below.

Imagine there's a bag of 30 candies to split between 5 children. The fair thing to do would be to either split evenly (6 each) or to split based on the ages of the children, but we just want to know how many ways we could distribute this candy, making sure each child gets at least one piece.

Imagine we line the candies up, and line the children up separately.

> Think first: How could we use some sticks to mark one way to distribute the candies to the children?

We can just place some sticks between the candies, where the first set (from the beginning to the first stick goes to the first child, the next set goes to the next child and so on.

> Think first: Draw a picture of this for 10 candies and 3 kids. How many sticks did you need to use?
> Do another picture for 10 candies and 4 kids. How many sticks did you need to use then?
> What about 12 candies and 4 kids? How many sticks do you need?
> For all of the above, how many places can you put the first stick? After the first is placed, how many places can you place the second stick?

We'll note that we don't need as many sticks as we have children, but one less than that number, since the first and last groups have one stick definining the right and left borders.

It's also important to note that if we want to guarantee each child gets at least one candy, we can only place sticks in between two pieces of candy. This means the number of gaps defines where we can place sticks, which is also the number of candies minus one.

Since the order we place this sticks doesn't matter, this is a combination problem, where there are $n-1$ gaps (for $n$ candies), and $k-1$ sticks to place/places to choose (for $k$ children). This means the problem is ${n-1 \choose k-1}$ in general, or ${30-1 \choose 5-1}$ in the case of our specific problem.

Now what if we don't care if a child doesn't get any candy?

> Think first: what changes about our requirements?
> Do the number of sticks change?
> Where can we place sticks?

The number of sticks should remain the same, as this still defines how much each child recieves. Likewise, this is still a combinations problem, as the order of how we place the sticks doesn't matter.

When we are allowed to give a child no candy, this means we can now place sticks before the line of candy, and multiple sticks between two pieces of candy. We can try to change how we did the previous problem to accommodate this, or we can realize this re-shapes our problem into something else.

We're just arranging the $n$ candies and the $k-1$ sticks. We can reframe this as a letter problem. If we have $n$ Cs and $k-1$ Ss, how many distinct arrangements of these letters can we create?

This is simply $\frac{(n + k - 1)!}{n!(k-1)!}

Notice that this is the same as ${n+k-1 \choose k-1}$ or ${n+k-1 \choose n}$.

> Check your understanding: How is this problem the same as a combination?

<details><summary>Check your answer</summary>
This is the same as choosing the $k-1$ spots the sticks go out of a total of $n+k-1$ spots and placing the $n$ candies around it or vice versa.
</details>

These situations are both considered as the stars and bars (or sticks and stones) method. The candies are the stars/stones, and the sticks are the bars/sticks.

This method works for many types of problems, including the ones mentioned in the chapter involving integer-valued solutions to simple functions.

> Think about it: Try to come up with a problem that can be solved using stars and bars, then solve it using stars and bars.