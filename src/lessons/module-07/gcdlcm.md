# GCD and LCM

GCD and LCM are related concepts that are important in Number Theory. We'll revisit these concepts when we discuss the Euclidean Algorithm next week.

## GCD

GCD stands for Greatest Common Divisor, and evaluates to the largest divisor two numbers have in common, as the name suggests.

$GCD(10, 20) = 10$

$GCD(10, 15) = 5$

$GCD(10, 13) = 1$

Since $1$ is a divisor of all numbers, the minimum a GCD can be is $1$.

Note also that 

$k \cdot GCD(a, b) = GCD(k \cdot a, k \cdot b)$

So,

$GCD(10, 20) = 10 \cdot GCD(1, 2) = 10 \cdot 1 = 10$

## GCD From Prime Factorizations

Given two prime factorizations, can you find the GCD?

$n_1 = 2^3 3^2 5^2 7^1$

$n_2 = 2^4 3^1 5^3$

> Think first: What divides both?

We can see that $2$, and even all the way up to $2^3$ divides both numbers. Unfortunately, $2^4$ only divides one, so we can't go that high. Likewise, $3^1$ and $5^2$ go into both numbers. If I assemble these into one number:

$2^3 3^1 5^2$

This is the GCD!

In general, we can find the GCD of two numbers by looking for the lowest exponent in each prime factorization.

## LCM

The LCM stands for Least Common Multiple, and is the lowest integer that is a multiple of two numbers.

$LCM(10, 20) = 20$

$LCM(10, 15) = 30$

$LCM(10, 13) = 130$

Since the multiplication of two numbers is a multiple of both, the maximum LCM is the product of the two values.

$k \cdot LCM(a, b) = LCM(k \cdot a, k \cdot b)$

So,

$LCM(10, 20) = 10 \cdot LCM(1, 2) = 10 \cdot 2 = 20$

## LCM From Prime Factorizations

Given two prime factorizations, can you find the LCM?

$n_1 = 2^3 3^2 5^2 7^1$

$n_2 = 2^4 3^1 5^3$

> Think first: What would be a multiple of both numbers?

We can see that if we include $2^4$, then both numbers will be a divisor, at least in terms of $2$s. If we select fewer $2$s, then $n_2$ will not be a divisor. More $2$s are not needed.

Likewise, we can take $3^2$, $5^3$ and $7^1$ to cover both numbers.

$2^4 3^2 5^3 7^1$

This is the LCM!

In general, we can find the GCD of two numbers by looking for the highest exponent in each prime factorization.

## Relationship Between GCD and LCM

> Think first: If GCD takes the highest exponents and LCM takes the lowest, what is the relationship between the GCD, LCM, and the two numbers?

For two numbers, $a$ and $b$,

$a \cdot b = GCD(a,b) \cdot LCM(a,b)$

Since the GCD captures all the higher exponents, and LCM captures the lower exponents, between the two of them, all exponents are there!

This can be very helpful in solving problems quickly. If you can find the GCD easily, to find the LCM, you just need to compute $\frac{a \cdot b}{GCD(a,b)}$

## GCD and LCM of 3 or More Numbers

GCD and LCM can be defined on more than two numbers, this just doesn't allow us the nice relationship we just described. We will be working only with GCD and LCM on two numbers.