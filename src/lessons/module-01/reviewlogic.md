# Review: Logic

Mathematical Logic allows us to mathematically state arguments and solve them.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Applied Discrete Structures](https://discretemath.org/ads/chapter3.html), [Chapter 3.1-3.4](https://discretemath.org/ads/s-propositions-logic-operators.html)

## Truth, Logical Operators, and Truth Tables
[Chapter 3.1](https://discretemath.org/ads/s-propositions-logic-operators.html)
[Chapter 3.2](https://discretemath.org/ads/s-truth-tables.html)

> Remember: Please read the texts linked above before reading the material below.

Consider the sentence "Kibo is an institution that allows students to earn a degree in Computer Science." We know this sentence to be truthful. However, "Kibo is an institution that allows students to earn a degree in History" is not truthful. Both of these sentences are considered **propositions**, since we can assign them a truth value. Propositions are either True (correct), or False (incorrect). We can represent these propositions as variables, and speak in a mathematical language.

Let p represent "Kibo is an institution that allows students to earn a degree in Computer Science" and q represent "Kibo is an institution that allows students to earn a degree in History." We say that p has the value True, often represented numerically as a 1, and q has the value False, often represented numerically as a 0.

Instead of investigating specific statements, let us use p and q as variables, which may have value 0 or value 1. We define operations on propositions to indicate how propositions may be combined. These are called **Logical Operators**. Many of them have names that indicate how we might phrase the combined propositions in English.

One such operator is the "or" operator, which combines two propositions, and can be written symbolically as:

$$p \vee q$$

"p or q" is true when at least one of p or q is true. Note that this includes if p and q are both true! To aid in viewing all potential outcomes of a set of propositions, we use **Truth Tables**.

| $p$ | $q$ | $$p \vee q$$ |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

In the table we see all possible combinations of p and q, with the final column being the proposition we are investigating. The table shows that the only time $p \vee q$ is False (0), is when both p and q are false.

A related operator is the "and" operator, which also combines two propositions, and can be written symbolically as:

$$p \wedge q$$

"p and q" is true when both p and q are true.

| $p$ | $q$ | $$p \wedge q$$ |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 1 | 1 |

This table shows us the definition of the "and" operator. Note that the p and q columns are the same as before, since we are just viewing all possible combinations of p and q.

There is one important operator which is only defined on one proposition. This is the "not" operator, which can be written symbolically as:

$$ \neg p $$

| $p$ | $ \neg p $ |
|---|---|
| 0 | 1 |
| 1 | 0 |

Here our truth table only needs to consider p, so it is much shorter.

In algebra, our most common operators are addition (+) and multiplication (*), which can be combined to create much larger statements. We can do the same with our logical operators!

| $p$ | $q$ | $p \wedge q$ | $(p \wedge q) \vee p$ |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 1 |
| 0 | 1 | 0 | 0 |
| 1 | 1 | 1 | 1 |

This table shows us that $(p \wedge q) \vee p$ is true when p is true, which makes sense as the "or" operator needs only one proposition to be true, and $p \wedge q$ is more restrictive than p. Note that parentheses here work just like algebra: the expression in the parentheses is evaluated first.

Let's try a harder statement! 

$\neg( \neg p \wedge \neg q)$

When we create our truth table, we will include columns for each operator individually. This allows us to combine them easier, and with fewer mistakes. First, we will do columns for $\neg p$ and $\neg q$ since they appear in our expression.

| $p$ | $q$ | $\neg p$ | $\neg q$ |
|---|---|---|---|
| 0 | 0 | 1 | 1 | 
| 1 | 0 | 0 | 1 | 
| 0 | 1 | 1 | 0 | 
| 1 | 1 | 0 | 0 |

Then the "and" statement that is in parantheses.

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg p \wedge \neg q$ |
|---|---|---|---|---|
| 0 | 0 | 1 | 1 | 1 | 
| 1 | 0 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 0 | 
| 1 | 1 | 0 | 0 | 0 |

Finally the negation of that "and" statement.

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg p \wedge \neg q$ | $\neg( \neg p \wedge \neg q)$ |
|---|---|---|---|---|---|
| 0 | 0 | 1 | 1 | 1 | 0 | 
| 1 | 0 | 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 0 | 0 | 1 | 
| 1 | 1 | 0 | 0 | 0 | 1 |

The final column contains the truth values for our statement! Do you recognize this column?

| $p$ | $q$ | $$p \vee q$$ |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

It has the same truth values as $p \vee q$! We can see that our original statement does not have any "or" operators, so how do they have the same column values in a truth table?

In our original statement, we take combine two negations with an "and". We can see in our table that this is only true when both values are false. Therefore, the negation of our "and" is true everywhere except where both values are false, which is the definition of the "or" operator.

We say two propositions are **equivalent** if their truth values are always the same. We can express this symbolically.

$\neg( \neg p \wedge \neg q) \equiv p \vee q$

In this case, we have proved equivalence using truth tables. If the columns in a truth table are the same for two statements, they are equivalent.

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg p \wedge \neg q$ | $\neg( \neg p \wedge \neg q)$ | $$p \vee q$$ |
|---|---|---|---|---|---|---|
| 0 | 0 | 1 | 1 | 1 | 0 | 0 |
| 1 | 0 | 0 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 0 | 1 | 1 |
| 1 | 1 | 0 | 0 | 0 | 1 | 1 |

If there is even one difference between the columns, the statements are not equivalent. For example, $p \vee q \not\equiv q$, since the second row is different.
