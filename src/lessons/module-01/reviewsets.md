# Review: Set Theory

A set is a collection of unique elements. We use set notation to describe specific sets, and to denote operations that we can preform on sets.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Applied Discrete Structures](https://discretemath.org/ads/chapter_1.html), [Chapter 1.1-1.3](https://discretemath.org/ads/s-set-Notation-and-Relations.html)

## Set Definition and Notation

[Chapter 1.1](https://discretemath.org/ads/s-set-Notation-and-Relations.html)

> Remember: Please read the text linked above before reading the material below.

The most basic way to describe a set is as a collection of unique elements. These elements could be numbers, letters, or any object.

While sets are not ordered, sometimes it is easiest to describe a set by **enumerating** (listing) the objects it holds, separated by commas, inside a set of brackets.

For example, a set containing the integers between 1 and 10 can be described as written, or it can be described by writing

$$\{ 1, 2, 3, ..., 9, 10\}$$

Since this is a small list, we could also write all the numbers. But imagine a set containing numbers from 1 to 2000. $\{ 1, 2, 3, ..., 1999, 2000\}$ is much more concise than trying to write all 2000 values. Likewise, if we wanted to describe all positive integers, we might say:

$$\{1, 2, 3, 4, ...\}$$

We leave off the last number, since there is no "last" integer. 

The **cardinality** of a set is the number of elements it contains. Finite sets are sets that have a finite cardinality. For example, our first set has a cardinality of 10, and therefore it is a finite set. The set we have just defined has infinitely many elements. The cardinality of this set is infinite, making it an infinite set.

This way to describe sets work for simple operations on infinite sets, and for most finite sets, but consider this set description:

$$\{1, 2, 4, ... \}$$

This set could describe powers of 2, but it could also describe the sequence given by adding an increasing value to the previous number. 1 + 1 = 2, 2 + 2 = 4, and therefore, the next value would be 4 + 3 = 7. It is important when describing sets to only use enumeration when it is obvious what set it describes.

Mathematicians have developed **set notation**, which describes a set, or a combination of sets, using mathematical symbols.

**Set-Builder Notation** can help us construct sets. This is done by defining a variable (or sometimes multiple variables), then creating a mathematical statement with this variable. For any value of this variable, if the statement is true, this value is in the set. Usually the variable(s) and statement are separated by a pipe (|) or the abbreviation s.t., which stands for "such that."

For example, if we want to create our powers of two set, we could write

$$\{x | x = 2^k \text{ for some integer } k\}$$

$x = 2$ is true, since we can choose $k = 1$, while $x = 3$ is false, since we cannot find an integer $k$ for which $3 = 2^k$.

This writing is still more complicated than we would like it to be. It would be nice to represent this in only variables. For this, we will need to learn some more general set notation.

To denote that some value or variable is in a set, we use the symbol $\in$. For example, if value x is in set A, we can say 

$$x \in A$$

It is standard in mathematics to represent sets as uppercase letters. This helps to distinguish them from variables that may represent values.

We also have some common sets, which have specific letters that represent them. We use a fancy font or some extra lines in the letters to denote these sets. For example, $\mathbb{N}$ from the list below represents the Natural numbers, while N represents nothing (unless you've defined a set N).

| Set Name | Set Symbol | Set Description |
| --- | --- | --- |
| Integers | $\mathbb{Z}$ | The set containing all integers, positive and negative. These numbers are the numbers which are not fractions. |
| Natural Numbers | $\mathbb{N}$ | The set containing **positive** integers. | 
| Rational Numbers| $\mathbb{Q}$ | The set containing all numbers that can be represented as fractions. All numbers of the form $\frac{a}{b}$, where $a$ and $b$ are integers. |
| Real Numbers | $\mathbb{R}$ | The set containing all real numbers. This includes any non-imaginary number. |
| Empty Set | $\emptyset$ | The set containing no elements |

For most of these sets, the cardinality is infinity. We'll come back to these cardinalities later, as we'll find there are a few types of infinity. However, the empty set is considered to have cardinality of zero.

Now that we have some extra notation, we can combine our set notation knowledge with our logical statement knowledge to get

$$\{x | (\exists k \in \mathbb{Z}), x = 2^k \}$$

For a set of powers of two. It can be read "x such that, for some integer k, x is equal to 2 to the k power." We could, if we wished, add to the left hand side that x is an integer as well. Sometimes this helps when there are multiple conditions on x.

> Check your understanding: One of the following is the set of all postive real numbers, and the other is a set of all negative real numbers. Try reading the notation to determine which set is which.

$$\{x \in \mathbb{R}| x > 0 \}$$

$$\{x \in \mathbb{R}| x < 0 \}$$

<details><summary>Check your answer</summary>

The first is positive real numbers and the second is negative real numbers. This is a good reminder that 0 is neither positive nor negative.

</details>

> Think about it: Try using set-builder notation to define a set containing only even numbers. As a hint: remember that all even numbers are divisible by 2, and so can be written as 2 times some integer.