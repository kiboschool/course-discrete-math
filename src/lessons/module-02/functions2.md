## Cardinality and Countability
[Chapter 7.2](https://discretemath.org/ads/s-properties-of-functions.html)

> Remember: Please read the text linked above before reading the material below.

When a function is Bijective, it means that every element of the domain maps to a unique input of the codomain. As these are sets, this implies that the size (cardinality) of these sets is the same.

We can use this to prove a concept called **countability**. We define an infinite set as **countable**, or countably infinite, if it there is a bijective function from the natural numbers to the set. It's called countability as the natural numbers are also known as the counting numbers, as they are the numbers we typically use when counting.

Sets which are infinite, but not countably infinite are called **uncountable**.

In mathematics, we have a concept around different sizes of infinity. One of these sizes is countably infinite. Think about the difference between the infinity of the natural numbers and the infinity of the real numbers. There are infinite real numbers between each set of numbers in the natural numbers, so in some sense, it makes them different sizes of infinity.

The following is a fun TedEd video about Hilbert's Hotel, a thought experiment which highlights how little we understand infinity. Please watch it and bring any questions you have to class!

<div class="embed"><iframe src="https://www.youtube.com/embed/Uj3_KqkI9Zo?si=sRIc6XjlIkSonYu0" title="The Infinite Hotel Paradox" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

We can show the positive even numbers (plus zero) are countable using the function $f(x) = 2x$

Showing it's injective:

$f(x) = f(y)$

$2x = 2y$

$x = y$

Showing it's surjective:

$y = 2x$

$x = \frac{y}{2}$

Since $y$ is even, $\frac{y}{2}$ is always a natural number.

So this function is bijective.

The output is all even numbers, and thus the positive even numbers plus zero are countable!

> Check your understanding: Can you prove that the positive odd numbers are countable?

<details><summary>Check your answer</summary>

The proof here is almost exactly the same as the one above, just with $f(x) = 2x - 1$ or $f(x) = 2x + 1$.

However, we need to be careful. If we consider the natural numbers starting at $0$, as we typically do in this course, we'll use $f(x) = 2x + 1$, and if we consider them to start at $1$, we need to use $f(x) = 2x - 1$. If we swap these, we either include $-1$, or don't include $1$.

We proved in a previous Check your understanding that functions of this form were always bijective, we just need to adjust it to the integers and odd integers (rather than real numbers to real numbers), and it will also be bijective.

The tricky part is that in surjective, if you have $\frac{y - 1}{2}$ this will be an integer if $y$ is an odd integer.

Since it's bijective and outputs the odd integers, the positive odd integers are countable.

</details>

> Think about it: The rational numbers are countable. Can you figure out how this is true? What sort of function would allow us to prove this?