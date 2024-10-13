# Primes and Prime Factorization

Primes are incredibly important for a number of reasons, so let's be sure to get the definition right.

## Prime Numbers

Many people will naively define primes as "A number which is divisible by 1 and itself" or as "A number which is divisible by two numbers."

These definitions both fail to correctly define a prime number.

> Think first: Can you find the problems with these?

Think of your favorite prime number. By our definition in the last section, what are its divisors?

You should find 4 numbers: $1$, $p$, $-1$, and $-p$ where $p$ is your prime number.

A more acceptable definition of prime is to say "a number which is divisible by exactly 2 positive integers."

An even better definition allows us to see the usefulness of primes.

A composite number is a number that is not prime. This means it should have some divisor, other than 1, that is strictly less than the number.

For example, $6 = 3 \cdot 2$ where $3$ and $2$ are both strictly less than 6.

This is often how composite numbers are defined in the world of Number Theory.

A **composite number** is an integer greater than 1 which can be written as a product of two strictly smaller positive integers.

Then we can define a prime as follows:

A **prime number** is an integer greater than 1 which cannot be written as a product of two strictly smaller positive integers.

We consider primes and composites only amongst the positive integers, excluding $1$. We will see why $1$ cannot fit in either category later on, but for now know that $1$ is neither prime nor composite, just like zero is neither positive nor negative.

## Prime Factorization

Take your favorite composite number and break it down into factors. Keep breaking it down until you can no longer do so. You should end up with a multiplication of prime numbers. This is the basic idea behind prime factorization.

$400 = 40 \cdot 10 = 4 \cdot 10 \cdot 2 \cdot 5 = 2 \cdot 2 \cdot 2 \cdot 5 \cdot 2 \cdot 5 = 2^4 \cdot 5^2$

A number $n$ can be written in the form

$n = p_1^{x_1}\cdot p_2^{x_2} \cdot p_3^{x_3} \cdot ... \cdot p_n^{x_n}$

Where $p_i$ are all distinct prime numbers, written in order from smallest to largest, and $x_i$ are positive integer exponents.

In fact, we can say something stronger

### The Fundamental Theorem of Arithmetic

The Fundamental Theorem of Arithmetic states that any positive integer $n$ has a unique prime factorization of the form described above.

> Check your understanding: Can you see now why $1$ cannot be prime nor composite?

<details><summary>Check your answer</summary>

$1$ obviously cannot be composite, as it cannot be expressed as a product of strictly smaller positive integers.

However, if $1$ was prime, we could create infinitely many prime factorizations for any number!

$400 = 2^4 \cdot 5^2 = 1^1 \cdot 2^4 \cdot 5^2 = 1^2 \cdot 2^4 \cdot 5^2 = ...$

</details>

## Infinitely Many Primes

As the values of numbers increase, primes seem to be less and less common. However, we can prove that there are infinitely many prime numbers.

Proof.

Assume there are only finitely many primes. Let $P$ be the product of all primes.

Consider the number $P+1$.

$P+1$ is not divisible by any prime (it would leave remainder 1).

Therefore, $P+1$ is not composite, as it cannot be written as a product of strictly smaller positive integers.

However, $P+1$ is larger than all primes, and therefore cannot be any of our finite primes.

Contradiction: This means there is a number that is both not prime and not composite. All numbers greater than 1 are either prime or composite.

Therefore, there cannot be finitely many primes.

QED.