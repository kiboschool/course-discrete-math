# Divisibility Rules in Different Bases

Just like we have divisibility rules in base 10, we can have rules in any base.

## Divisors of the Base

If a number divides the base, this is similar to our divisibility by 2 and 5 rules in base-10.

Just look at the last digit!

$101_2$ is not divisible by $2$ since it ends in a $1$

$3F94_{16}$ is divisible by $2$ and $4$, but not $8$ or $16$ since it ends in a $4$.

$A3B5_{15}$ is divisible by $5$ since it ends in a $5$, but it is not divisible by $3$ since its last digit is $5$ (not divisible by 3).

> Check your understanding: Use a random number generator to generate a number between 2 and 10, then generate another number between 1 and 10,000. Using the first number as the base, can you determine if the second number has any easy-to-find divisors?

<details><summary>Check your answer</summary> 

Answers here will depend largely on the numbers generated, but use this for practice, and double check by converting the number back into base $10$ and using a calculator.

</details>

## Base - 1

We were able to determine a rule for divisibility by $9$ in base $10$. We can similarly find that for any base $b$, a number is divisible by $b-1$ if the digits (in that base) sum to a number that is divisible by $b-1$.

For example:

$2433_7$

$2 + 4 + 3 + 3 = 12$

This number is divisible by 6!

In fact, if we convert it,

$2 \cdot 7^3 + 4 \cdot 7^2 + 3 \cdot 7^1 + 3 \cdot 7^0 = 906$

$906$ is divisible by $2$ and $3$, therefore it is divisible by $6$!

So, $2433_7$ is divisible by $6$

> Check your understanding: Use a random number generator to generate a number between 2 and 10, then generate another number between 1 and 10,000. Using the first number as the base, can you determine if the second number is divisible by the base minus $1$?

<details><summary>Check your answer</summary> 

Answers here will depend largely on the numbers generated, but use this for practice, and double check by converting the number back into base $10$ and using a calculator.

</details>

## Base + 1

> Think about it: Can you come up with a divisibility rule for the base plus 1?
> Hint: divisibility by 11 would be an example here. What would happen in general?

## Multiplication in Different Bases

We know that 10 times any number in base 10 just moves all the digits one place value.

> Think about it: What happens if I multiply any number by $(10)_b$?
> Hint: Remember that this is just $b$ itself.