## Equivalence Relations

[Chapter 6.3](https://discretemath.org/ads/s-properties-of-relations.html)

> Remember: Please read the text linked above before reading the material below.

You should notice that for equality (of real numbers), the relation is reflexive, symmetric, and transitive. Any relation that has these three properties is known as an **equivalence relation**.

Let's look at some other equivalence relations.

Let R be a relation on the set of integers. aRb when a and b have the same remainder when they are divided by 7.

This is reflexive, since any number will have the same remainder as itself when divided by 7.

This is symmetric since numbers will always have the same remainder when dividing by 7. The order we say them in does not matter.

This is transitive. Let a and b have the same remainder k. If bRc, then c also has remainder k. Since a and c have remainder k, then aRc.

7 is not a special number, we could replace it with any other positive integer and still have an equivalence relation. This is how equivalence under modulus is defined, which we will re-visit in a few weeks.

A silly example would be a relation defined on people, where two people are related if they have the same last name.

In Geometry, one equivalence relation would be a relation on triangles where two triangles are related only if they are similar to each other.

> Check your understanding: Try proving to yourself that one of the relations mentioned above is an equivalence relation. Remember, you need to show that it is symmetric, reflexive and transitive.

<details><summary>Check your answer</summary>

Your answer here depends on the relation chosen, but just be sure to show that it is symmetric, reflexive, and transitive, as we did in the example above.

</details>

A special example of a relation that is not an equivalence relation is the empty relation on a non-empty set. This relation is symmetric and transitive, since there are no numbers to compare in the relation. However, this is not reflexive since there are numbers in the set which are not related to each other.
