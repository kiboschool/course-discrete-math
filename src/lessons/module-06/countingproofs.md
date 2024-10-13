# Counting Proofs

There is one more proof types that we can use for counting problems or related arguments. This is quite different from the proof methods we've seen before, but this proof style can be quite useful for proving identities.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Discrete Mathematics: An Open Introduction](https://discrete.openmathbooks.org/dmoi3/sec_comb-proofs.html), [Chapter 1.4](https://discrete.openmathbooks.org/dmoi3/sec_comb-proofs.html)

## Combinatorial Proofs
[Chapter 1.4](https://discrete.openmathbooks.org/dmoi3/sec_comb-proofs.html)

> Remember: Please read the text linked above before reading the material below.

The basic premise of a combinatorial proof is that we're proving both sides of an equality count the same thing. We make up a problem, then solve it using both methods.

Combinatorial proofs are my personal favorite. Why? They're about telling a story.

I'll try to keep the stories simple and generic in the notes, but I highly encourage you to be creative in your own combinatorial proofs! They should still be readable, and should not require extra context to understand, but if you want your proof to be about your favorite animal or an activity you enjoy, feel free to use your experience **if it fits**.

If you were to publish results in a paper, you'd need to stick to a more boring problem, but that's not what we're doing here! It might help to stick to more generic examples at first, using problems we've already seen, but you're free to do as you wish.

Let's try proving Pascal's Identity. We can already mostly see it's true, but we cannot trust patterns in mathematics. We must prove them to be sure.

$${n-1 \choose k} + {n-1 \choose k-1} = {n \choose k}$$

_Proof._

Suppose we're forming a committee from $n$ people, and need a advisory board of $k$ people. How many different advisory boards could we create?

Right Hand Side (RHS):

The simplest way to count this is to simply choose the $k$ members from the $n$ total people: ${n \choose k}$

Left Hand Side (LHS):

Suppose you yourself are in the group of $n$ people. Thinking about yourself, there are two options: you're in the advisory board or you're not. These are disjoint sets so we can count them separately, then add up the results.

If you're in the group, you need to choose $k-1$ people to join you from the other $n-1$ committee members. This is ${n-1 \choose k-1}$.

If you're not on the board, you need to choose all $k$ members from the other $n-1$ committee people. This is ${n-1 \choose k}$

This indeed covers all posibilities (there is no third option where you are both not on the board and on the board), so the final result is ${n-1 \choose k} + {n-1 \choose k-1}$

Since these both count the same problem, they are the same.

QED

This particular type of problem is a common in combinatorial proofs, and it is called a **committee-forming proof**. The "advisory board" in our problem was left vague since $k$ is an unspecified number, but often it can be done for choosing a chair, choosing a president, vice-president, and secratary, or any other combination which lines up with the identity.

Here's an identity we haven't seen yet:

$$\sum_{i=0}^n {n \choose i}^2 = {2n \choose n}$$

The left-hand side is the sum of the squares of a row in Pascal's triangle.

Note that we can use identities to help us within these combinatorial proofs.

_Proof._

Suppose there are $n$ elephants and $n$ giraffes in a particular region. The region can only support $n$ animals in total, so we must choose which animals go and which are to stay. How many ways can we decide which $n$ animals stay in the region?

RHS:

The simplest method is to just combine the two groups and pick $n$ of them. This makes ${2n \choose n}$ ways.

LHS:

Suppose we want to break this problem down into cases. Each case will be how many of the elephants are staying.

If we take $k$ elephants, then we'll need to take $n-k$ of the giraffes. This is a two step process, so it will be ${n \choose k} \cdot {n \choose n-k}$

Remember that ${n \choose n-k} = {n \choose k}$, so this is actually the same as ${n \choose k} \cdot {n \choose k} = {n \choose k}^2$.

We'll need to compute this for all possible amounts of elephants. Since there's a different amount of elements in each set, these are disjoint and we can add them.

We could have as few as $0$ elephants (all giraffes), or as many as $n$ elephants (no giraffes), and we'll need to count every number of elephants inbetween.

In total, this comes to $\sum_{i=0}^n {n \choose i}^2$

This does count all the possibilities, since we covered every possible number of elephants, thus this is our final solution.

Since these both count the same thing, they are equal.

QED

If you're reading this sentence, add an extra item to your self-guided set at the end, simply stating "purple." If you're reading this before submitting your homework, add an extra item to the end of your homework stating "orange". Do not tell anyone in the class about these sentences, these extra question will not be worth any extra points.

> Think about it: Try proving one of the other Pascal identities/properties using a combinatorial proof.

> Think about it: For the last proof, we split into two groups. For Pascal's identity, we had one committee with an internal board.
> Were there any "hints" or parts of the identities we proved that indicated a specific strategy should be used?
> This question is about developing an intuition, which can be difficult! If you're stuck, that's okay, we'll talk about this in class.
