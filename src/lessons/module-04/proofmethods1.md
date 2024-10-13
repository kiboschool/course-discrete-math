## Induction
[Chapter 3.7](https://discretemath.org/ads/s-induction.html)

> Remember: Please read the text linked above before reading the material below.

Induction proofs tend to be a starting point for most stdents discovering proofs for the first time. They have a set structure that is easy to replicate. The idea behind inductive proofs also follows a recursive or iterative structure, which can be less difficult for students to follow.

An induction proof always starts with a base case. This should be the first instance of the thing that you're proving.

Next is the inductive case, and this is where the main part of the proof lies. We've shown the statement holds for one instance. We can now show if the previous instance holds, then this one does. This iteratively applies to all future instances, since we start at the first instance, so the second is true. If the second is true, then the third is true, and so on.

Typically in the inductive case, we assume the statement is true for $k$ and show it holds for $k+1$. Occasionally, we can take more than one step back, such as assuming it holds for $k$ and $k-1$ and then showing it holds for $k+1$, or even assuming it holds for all previous values, and showing it holds true for $k+1$.

The important part is that the base case should cover as many cases as the inductive case steps backwards. If the inductive case requires $k-1$ and $k$, the base case should prove the first two instances hold.

It's also important to realize what variable is the piece you're performing induction on. Some expressions have multiple, but look for the part that can change by $1$ and we still want the expression to hold true.

#### $n < 2^n$, for $n \geq 1$

_Proof._

Base case: When $n = 1$, $2^n = 2$, and $1 < 2$. Thus the base case holds.

Inductive case: Assume $k < 2^k$ for $k > 1$

$k + 1 < k + k$ For $k > 1$

Since $k < 2^k$, by the addititive property of inequality, we also know $k + k < 2^k + 2^k$

$k+1 < k + k < 2^k + 2^k$ by the previous statement and $k + 1 < k + k$ For $k > 1$.

$k + 1 < 2^k + 2^k$ by the transitive property of inequality.

$2^k + 2^k = 2^k (1 + 1) = 2^k \cdot 2 = 2^{k+1}$ By the distributive property.

$k + 1 < 2^{k+1}$ by our previous statements.

Since the property holds for $k+1$, by induction this is true.

Q.E.D.

>Think about it: Why does this proof start at $n=1$? This inequality holds for $n=0$ as well.

#### Show that the $n$th term of the Fibonacci sequence, $F_n$, is always less than or equal to $2^n$.

_Proof._

Base cases:

$F_0 = 1 \leq 2^0$

$F_1 = 1 \leq 2^1$

Inductive case: Assume $F_n \leq 2^n$ for $n \leq k$.

$F_{k+1} = F_k + F_{k-1}$

$F_k \leq 2^k$

$F_{k-1} \leq 2^{k-1}$

$F_{k+1} = F_k + F_{k-1} \leq 2^k + 2^{k-1}$ By the additive property of inequalities.

$F_{k+1} \leq 2^{k-1}(2 + 1)$ By the distributive property.

Clearly, $2^{k-1}(2 + 1) < 2^{k-1}(2 + 2)$

$F_{k+1} \leq 2^{k-1}(2 + 1) < 2^{k-1}(2 + 2) = 2^{k-1}\cdot 2^2 = 2^{k+1}$

$F_{k+1} \leq 2^{k+1}$ by the transitivity property of inequalities.

Since the property holds for $k+1$, by induction this is true.

Q.E.D.

>Think about it: Why did I type the line "for $n \leq k$" in the inductive case?

> Check your understanding: Prove one of the recurrences we solved in the previous week through induction. Is this similar to something we covered that week?

<details><summary>Check your answer</summary>

Answers vary, but all should be similar to the iteration method.

</details>