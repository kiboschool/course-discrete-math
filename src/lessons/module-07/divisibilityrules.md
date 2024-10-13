# Divisibility Rules

Many people already know some of these divisibility rules, but identifying where they start can help in creating new rules or memorizing other known rules.

## Divisibility by 2

Many of us can look at a number and immediately determine if it is even. We just look at the last digit: if this is even, then the whole number is even.

We tend to take this as a fact, not thinking about why it works. Looking at place values can help us figure this out.

We think in base ten, so for any number, we can represent it as a sum of values multiplied by powers of 10.

$54398 = 5 \cdot 10^4 + 4 \cdot 10^3 + 3 \cdot 10^2 + 9 \cdot 10^1 + 8 \cdot 10^0$

Look closely at this statement. All values except for the last digit are divisible by $10$. This means they must also be divisible by $2$! The only value we need to check is the last digit. If it's even, everything is even, if it's odd, we'll have an odd value.

## Divisibility by 4

There is a less commonly known rule for divisibility by 4: looking at the last two digits.

> Think first: Based on what we did above, can you figure out how this rule works?

$54328 = 5 \cdot 10^4 + 4 \cdot 10^3 + 3 \cdot 10^2 + 2 \cdot 10^1 + 8 \cdot 10^0$

Notice that $10^2 = 100$ is divisible by 4! So all digits except the tens and ones are divisible by 4, therefore, we look at those last two!

> Think about it: Can you come up with a rule for divisibility by 8?

## Divisibility by 5

Because $10$ is divisible by $5$ along with $2$, we have a similar rule for divisibility by 5: look at the last digit.

> Think about it: Can you come up with a rule for divisibility by 25? What about 125?

## Divisibility by 9

There's a somewhat-known rule for divisibility by 9 or 3. Let's see if we can start from our place values first, then reach the rule.

We know a number can be expressed in terms of 10, but we want 9 instead, so let's try doing $9 + 1$ wherever we see a 10

$54324 = 5 \cdot 10^4 + 4 \cdot 10^3 + 3 \cdot 10^2 + 2 \cdot 10^1 + 4 \cdot 10^0 = 5 \cdot (9 + 1)^4 + 4 \cdot (9 + 1)^3 + 3 \cdot (9 + 1)^2 + 2 \cdot (9 + 1)^1 + 4 \cdot (9 + 1)^0$

Note that for the expansions of all of these, every term will have some power of $9$ except for the $1^n$ term.

Therefore, each expanded term is divisible by $9$ except for that last $1$. This means, we're really just considering each digit since $1$ times any number is itself.

$5 + 4 + 3 + 2 + 4 = 18$

Since the sum of the digits is divisible by $9$, we can say the whole number is!

### Divisibility by 3

Since $9$ is divisible by $3$, the same rules and steps apply, just that the sum of the digits needs to be divisible by $3$ instead of $9$.

## Divisibility by 11

> Think about it: Can you come up with a divisibility rule for 11s?
> Hint: Remember we had 9 + 1 = 10? What happens if you say 11 - 1 = 10? Be careful of the negative and what happens in the expansion.