# The Extended Euclidean Algorithm

The Extended Euclidean Algorithm, as implied by its name, is an extension of the Euclidean Algorithm. This allows us to do many things, including solving our inverse-finding problem.

## Magic Box Method

Try watching the video below for a good idea at how to follow the steps of the Extended Euclidean Algorithm.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/IwRtISxAHY4?si=qfhiFJb78216E_iu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

## Linear Equations

As described in the video above, we can think of the equation

$ax + by = GCD(a,b)$

in terms of different $x$ and $y$ values that result in different values (usually different values from the $GCD(a,b)$).

Our first two sets of values are usually $(0,1)$ and $(1,0)$ since we know the outcome easily: $b$ and $a$ respectively.

From here we can take these equations and follow the steps of the euclidean algorithm with the entire equation.

As an example, let's work with $114$ and $935$.

Via the traditional euclidean algorithm, we would say:

$935 = 114 \cdot 8 + 23$

$114 = 23 \cdot 4 + 22$

$23 = 22 \cdot 1 + 1$

$22 = 1 \cdot 22 + 0$

So the GCD is $1$. $114$ should have an inverse mod $935$ and vice versa.

We want to solve:

$114x + 935y = 1$

Start with $(0,1)$ and $(1,0)$

$114(0) + 935(1) = 935$

$114(1) + 935(0) = 114$

We already know from the euclidean algorithm how many copies of $114$ go into $935$, so multiply the bottom equation by $8$ and subtract!

$114(0) + 935(1) = 935$

$-8(114(1) + 935(0) = 114)$

or

$114(0) + 935(1) = 935$

$+(114(-8) + 935(0) = -912)$

$=114(-8) + 935(1) = 23$

Then we take the last two equations and continue our next steps!

$114(1) + 935(0) = 114$

$-4(114(-8) + 935(1) = 23)$

$= 114(1 + 12) + 935(-4) = 22$

We already know we're close to the end since we did the Euclidean Algorithm already!

$114(-8) + 935(1) = 23$

$-(114(13) + 935(-4) = 22)$

$=114(-8-13) + 935(1 + 4) = 1$

$114(-21) + 935(5) = 1$

Now to think about inverses, think about this equation $\mod{935}$

$114(-21) + 935(5) \equiv 114(-21) + 0 \equiv 1 \mod{935}$

$114(-21) \equiv 1 \mod{935}$

Which is what we want in an inverse!

$114^{-1} \equiv 914 \mod{935}$

### Code

The following euclidean algorithm takes advantage of times we can remove a smaller number multiple times in one step.

>Think about it: Can you adapt this code to create code for the extended euclidean algorithm?

<div style="position: relative;">
<iframe src="https://trinket.io/embed/python/6982f4d448" width="100%" height="356" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
