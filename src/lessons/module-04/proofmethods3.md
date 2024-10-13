## Cases
[Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

> Remember: Please read the text linked above before reading the material below.

Sometimes, we need to split a condition up into cases in order to prove a statement. These cases should cover all the possibilities that could happen, but we can split them up any way we'd like. Cases can be used in proofs of any type.

However, we do not want a large number of cases. If you find yourself splitting up into many cases, there may be a better proof style to use.

#### $m + n$ is only odd if $m$ is odd and $n$ is even, or if $m$ is even and $n$ is odd.

_Proof._

$m$ and $n$ can each either be even or odd.

Case 1: $m$ is even and $n$ is odd.

$m = 2k$, $n = 2j + 1$ by definition of even and odd.

$m + n = 2k + 2j + 1 = 2(k+j) + 1$ Since $k$ and $j$ are integers, $k + j$ is an integer, and $2(k+j) + 1$ is odd by definition of odd.

Case 2: $m$ is odd and $n$ is even.

This case is the same as case 1.

>Think about it: Why can I skip this case?

Case 3: $m$ and $n$ are odd.

$m = 2k + 1$, $n = 2j + 1$ by definition of odd.

$m + n = 2k + 1 + 2j + 1 = 2k + 2j + 2 = 2(k + j + 1)$ Since $k$, $j$, and $1$ are integers, $k + j + 1$ is an integer, and $2(k + j + 1)$ is even.

Case 4: $m$ and $n$ are even.

$m = 2k$, $n = 2j$ by definition of even.

$m + n = 2k + 2j = 2k + 2j= 2(k + j)$ Since $k$ and $j$ are integers, $k + j$ is an integer, and $2(k + j)$ is even.

Therefore, the only cases where $m + n$ is odd is when only one of $m$ and $n$ is odd (and the other is even).

Q.E.D.

> Think about it: What might be some good ways we can split numbers into cases? Even/odd is given above, are there any other categories that split nicely like this?

> Think about it: What do you think a good number of cases would be? What would a bad number be? Is there a clear line where you should stop thinking in cases, because there are too many?

## Proof of Existential Statements or Disproof of Universal Statements
[Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

> Remember: Please read the text linked above before reading the material below.

There are only two cases where a proof is as simple as showing an example. Proving an existential statement, or disproving a universal statement. 

For the first you simply need to show it exists, so find one! 

When disproving a universal statement, even one counterexample will make it false. If you find a counter example, you are done.

#### All Prime numbers are odd.

This is not true. $2$ is a prime number, and is even.

#### There exists an even prime number.

$2$ is an even prime number, therefore this statement is true.

There are very few cases where you will prove a statement true with an example. It is far more common to disprove statements in this manner.

> Think about it: Why do you think there are very few proofs of these types?