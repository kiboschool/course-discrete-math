## Tautology and Contradiction
[Chapter 3.3](https://discretemath.org/ads/s-equivalence-implication.html)

> Remember: Please read the text linked above before reading the material below.

Consider the statement $p \vee \neg p$. In words, p or not p. With our mathematical definitions of these words, this statement is always true. Statements that are always true are known as **Tautologies**. If two statements, P and Q are equivalent, then $P \iff Q$ should be a tautology!

Now consider the statement $p \wedge \neg p$. This statement is always false, since p and not p cannot be true at the same time. Statements that are always false are known as **Contraditions**.

These ideas are helpful for proving equivalence, and for proof by contradiction, which we will discuss in detail in future weeks.

Try to come up with your own tautology, using at least two variables. Now try creating a contradiction. What types of operators work well to form either type? There is no right or wrong answer, but this may help us form intuition on when we might use a proof by contradiction.

## Logic Laws
[Chapter 3.4](https://discretemath.org/ads/s-logic-laws.html)

> Remember: Please read the text linked above before reading the material below.

Truth tables can help us prove equivalence, but there is also a set of laws for logical operators.

Some laws should be familiar. "and" and "or" are commutative and associative. This means in a statement of multiple "and" operators, we can evaluate in any order. Note that this does not apply to a mix of "and" and "or" operators.

The distributive law is also present. For example,

$p \vee (q \wedge r) \equiv (p \vee q) \wedge (p \vee r)$

Identities are present for "and" and "or":

$p \vee 0 \equiv p$ and $p \wedge 1 \equiv p$

We can also use p with itself. For both "and" and "or" these are equivalent to p.

$$p \vee p \equiv p$$

$$p \wedge p \equiv p$$

We also discussed an important tautology and an important contradiction in the previous section.

As is true in algebra, we also have that the negation of a negation cancels, and reveals the original value.

$$ \neg \neg p \equiv p$$

The last set of important laws are known as DeMorgan's Laws. They state:

$$\neg(p \wedge q) \equiv \neg p \vee \neg q$$

$$\neg(p \vee q) \equiv \neg p \wedge \neg q$$

When applied over a set of parentheses, a negation will change an "and" to an "or" or an "or" to an "and." Try building truth tables to justify that this is true.

These basic laws can be applied to any logical expression, and can be used to simplify complicated expressions.

For example, say we have the expression

$$\neg(p \vee q) \wedge (q \vee \neg r)$$

We can first distribute the negation on the first terms, using DeMogan's Law:

$$(\neg p \wedge \neg q) \wedge (q \vee \neg r)$$

Then we can use the associative law to move the parentheses.

$$\neg p \wedge (\neg q \wedge (q \vee \neg r))$$

We can use the distributive property on the right side:

$$\neg p \wedge ((\neg q \wedge q) \vee (\neg q \wedge \neg r))$$

$\neg q \wedge q$ is a contradiction, so it is automatically false. Luckily, this forms an identity with the right portion, as it's combined using the or operator. $(\neg q \wedge q) \vee (\neg q \wedge \neg r) = 0 \vee (\neg q \wedge \neg r) = (\neg q \wedge \neg r)$.

$$\neg p \wedge (\neg q \wedge \neg r)$$

Now we have an expression that is simpler than the one we started with.

> Check your understanding: Create a truth table to verify the two expressions are equivalent.

<details><summary>Check your answer</summary> 

The important columns in your truth table should look like this:

| p | q | r | $\neg p \wedge (\neg q \wedge \neg r)$ | $\neg(p \vee q) \wedge (q \vee \neg r)$ |
| --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 0 |
| 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 | 0 |
| 1 | 1 | 0 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 |

</details>

All laws so far have been about our basic operators. We already showed the negation of an implication, but we also have a way to express an implication using negations.

$$p \rightarrow q \equiv \neg q \rightarrow \neg p$$

This is called the contrapositive. This is a good way to check your understanding of implication. Does this identity make sense?

If p, then q is equivalent to saying if q is untrue, then p is untrue. This should make sense from our truth tables:

| $p$ | $q$ | $p \rightarrow q$ |
|---|---|---|
| 0 | 0 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

Note that many people make mistakes when evaluating implications. We have names for two of these errors.

The inverse error is when the negation is simply applied to the original expression.

$$p \rightarrow q \not\equiv \neg p \rightarrow \neg q$$

In a truth table, we can see

| $p$ | $q$ | $p \rightarrow q$ | $\neg p \rightarrow \neg q$ |
|---|---|---|---|
| 0 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 |
| 0 | 1 | 1 | 0 |
| 1 | 1 | 1 | 1 |

These are clearly not equivalent statements. This error tends to show itself in reasoning. For example,

If a student studies at Kibo, then they must be learning computer science.

Does not imply:

If a student does not study at Kibo, then they must not be learning computer science.

The converse error involves swapping p and q.

$$p \rightarrow q \not\equiv q \rightarrow p $$

| $p$ | $q$ | $p \rightarrow q$ | $q \rightarrow p$ |
|---|---|---|---|
| 0 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 |
| 0 | 1 | 1 | 0 |
| 1 | 1 | 1 | 1 |

You'll notice that these two errors themselves are actually equivalent! This is because inverse is the contrapositive of converse.

Again, this error is most prevelent in reasoning.

If a student studies at Kibo, then they must be learning computer science.

Does not imply:

If a person is learning computer science, then they must be a student at Kibo.

Clearly, inverse error and converse error are failures in reasoning. To aid in reasoning through a set of statements, we provide names for specific arguement types.

**Modus ponens** states that if you have $p \rightarrow q$ and you also know $p$ is true, then you must have $q$.

**Modus tollens** states that if you have $p \rightarrow q$ and you also know $q$ is false, then you must have $\neg p$.

We can use these laws to derive conclusions from multiple statements. For example,

If a student studies at Kibo, then they must be learning computer science.

You are a student at Kibo.

Therefore, we can say:

You are learning computer science.

This is an example of Modus Ponens.

> Check your understanding: Try creating your own example of Modus Tollens from the statement "If a student studies at Kibo, then they must be learning computer science."

<details><summary>Check your answer</summary> 

We already have the implication.

For modus tollens, we also need $\neg q$, or in this case, A student is not learning computer science.

Then we could say that student must not be a Kibo student.

</details>

Given a set of logical statements, we can use our laws, along with modus ponens and modus tollens to reach a conclusion.
