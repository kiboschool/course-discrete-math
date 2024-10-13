## Cartesian Product

[Chapter 1.3](https://discretemath.org/ads/s-cartesian_Products_and_Power_Sets.html)

> Remember: Please read the text linked above before reading the material below.

The **cartesian product** of two sets is all combinations of an element of the first set with an element of the second. Usually these combinations are denoted using an ordered pair. In set terms, this is

$$A \times B = \{(a, b) | (a \in A) \wedge (b \in B)\}$$

The above notation, similar to one version of a multiplication symbol, is how we represent the cross product.

For example, if A = \{r, o, b\}, and B = \{o, p, e\}, the cartesian product of A and B is

$$A \times B = \{(r, o), (r, p), (r, e), (o, o), (o, p), (o, e), (b, o), (b, p), (b, e)\} $$

The cardinality of the cross product of two sets is just the product of their cardinalities. In our example, we had a set of size 3, and another set of size 3, so their cross product had 9 elements.

> Check your understanding: What would the Cartesian product of $B \times A$ in this case? Is it the same as $A \times B$? In what cases would it be the same, and when would it be different?

<details><summary>Check your answer</summary>

$B \times A$ will be $\{ (o, r), (p, r), (e, r), (o, o), (p, o), (e, o), (o, b), (p, b), (e, b) \}$

Note that this is **not** the same as $A \times B$. These ordered pairs are different.

</details>

We can also compute the cross product for multiple sets, and show that the cardinality is still just the product of all set cardinalities.

> Think about it: Consider sets A, B, C, and D, which all contain 0 and 1. What would their cross product ($A \times B \times C \times D$) contain? How many elements are there in the cross product? Is there an easy way to describe all the ordered sets of four?

## Power Set

[Chapter 1.3](https://discretemath.org/ads/s-cartesian_Products_and_Power_Sets.html)

> Remember: Please read the text linked above before reading the material below.

The **power set** of a set is the set of all possible subsets. This includes the empty set, and the set itself since this is not a set of all proper subsets.

For example, if set A = \{k, i, b, o \}

The powerset of A is \{\{\}, \{k\}, \{i\}, \{b\}, \{o\}, \{k, i\}, \{k, b\}, \{k, o\}, \{i, b\}, \{i, o\}, \{b, o\}, \{k, i, b\}, \{k, b, o\}, \{k, i, o\}, \{i, b, o\}, \{k, i, b, o \}\}

The cardinality of a powerset is 2 to the power of the cardinality of the original set. We'll revisit why this is the case when we discuss counting.

> Think about it: Consider the set A containing only 0 and 1 again. What would the power set of this look like? How many elements would it contain? How is this set different from the cross product of A with itself?
