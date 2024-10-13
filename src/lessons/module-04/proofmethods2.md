## Direct
[Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

> Remember: Please read the text linked above before reading the material below.

Direct proofs simply involve proving something as stated. If the statement is of the form $p \rightarrow q$, start at $p$ and end at $q$ through a series of definitions, theorems, and properties.

If the statement is not in the form of an implication, start with something that is known to be true, or a definition of some part of the statement and end with the statement being proven. Usually the starting place in these situations is some qualification that must be met for the statement to be true, such as a number being positive, or of a certain form.

#### If $n$ is an even number greater than 2, it is not prime.

_Proof._

Suppose $n$ is an even number.

By definition of even, $n$ is divisible by $2$.

Since $n < 2$, this means $n$ is divisible by a positive number less than itself that is not equal to $1$.

By definition, $n$ is composite.

Q.E.D.

#### The square of an even number is divisible by $4$.

_Proof._

Let $n$ be an even number.

By definition of even, we can write $n = 2k$ where $k$ is some integer.

$n^2 = (2k)^2 = 4k^2$

Since an integer times an integer is an integer, $k^2 = m$, where $m$ is an integer.

$n^2 = 4m$, where $m$ is an integer. By definition of divisibility, that means $n^2$ is divisible by $4$.

Q.E.D.

>Think about it: Why did this proof start with $n$ being an even number?

## Contrapositive
[Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

> Remember: Please read the text linked above before reading the material below.

Instead of starting with $p$ and ending with $q$, we convert the statement to $\neg q \rightarrow \neg p$, and start at $\neg q$.

Once converted, the proof is exactly the same as a direct proof.

#### If $n$ is a prime number greater than $2$, then it is odd.

We can convert this statement into "If $n$ is an even number greater than 2, it is not prime," which we proved above.

> Think about it: If contrapositive uses a direct proof after converting the statement, what does this mean for every statement we prove via a direct proof? What about each statement we prove through the contrapositive?

## Contradiction
[Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

> Remember: Please read the text linked above before reading the material below.

A proof by contradiction starts by assuming the statement is false. Then we show some contradiction occurs. In logical terms, if $p \rightarrow q$ is our implication. We state $p \wedge \neg q$. Then we show this statement is always false by finding some contradiction, meaning the negation of this negation (our original statement) is always true.

The contradiction must occur throughout all cases, all situations for this method to work. It is not enough to negate a statement and show one counterexample, as this only shows the original statement is true in one circumstance.

#### If $n$ is a prime number greater than $2$, then it is odd.

_Proof._

Assume this is false, that is, assume there is some $n > 2$ such that $n$ is a prime number and it is even.

By definition of even, $n$ is divisible by $2$.

Since $n > 2$, $n \neq 2$.

This means $n$ is composite.

This is a contradiction.

Therefore, if $n$ is a prime number greater than $2$, then it is odd.

Q.E.D.

>Think about it: We proved this problem for both contradiction and contrapositive. What are the differences? Do you think all statements that can be proven through contradiction can also be proven through contrapostive? Do you think all statements that can be proven through the contrapositive can be proven via contradiction? If the answer is no to either of these, try to think of an example which could not easily be proven by the other.