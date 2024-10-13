## Overcounting (and Correction)

This method has actually already been discussed. Remember how we fixed a permutation to get a combination? This uses the method of overcounting. If we know we are overcounting by a specific amount, we can correct that by removing the overcounted amount after we count everything.

Often, this is done using division, as was the case with permutation/combination. For example, if there are a group of 20 people, and everyone shakes hands with everyone once, how can we count the number of handshakes?

Note that there are 19 people that each person has to shake hands with, so our initial answer might be $20 \cdot 19$. However, this counts every handshake twice, as we count it once for each person involved in the handshake. Therefore the answer is $\frac{20 \cdot 19}{2}$.

> Think about it: We can also count the number of handshakes starting at a specific person: the first person has 19 handshakes to do, the next person only has 18 hands to shake (since they already shook hands with the first person), the next person has 17 and so on. Do we still get the same answer if we complete the problem this way?

This can be used to deal with rotations and reflections as well. Imagine there are 10 people sitting down at a circular table and we want to know how many ways people could be seated.

We can start by pretending the people are in a line, and therefore there's simply $10!$ ways to arrange the people.

However, the seating is only really different if some person is sitting next to someone different. If we simply rotate where people are sitting by one seat, we don't want to count this again.

Note that there are 10 rotations around the table. So each arrangement has 10 extra rotations that are included. Therefore, we divide by 10 and get that the true answer is $9!$.

> Think about it: What would happen for a group of 15 people around a table? 20? For n people around a circular table, what is the general answer?
> Can you think of a way to justify this general solution, other than stating we're dividing by the rotations?

A common type of problem in combinatorics is the rearrangement of letters. For example, how many ways can we rearrange the letters of the word MATHEMATICS?

There are 11 letters, so $11!$ would be a simple answer. However, there are some repeated letters. If we swapped the two As, it doesn't actually make a difference. For every valid different combination, there will be $1$ more ($2$ in total) that is the same, but with the As swapped. Same for the Ms and Ts. Therefore, we take $\frac{11!}{2\cdot 2\cdot 2}$

> Think first: What happens for a letter that appears 3 times in a word?

Consider the word Lollipop. L appears 3 times! There will be $3!$ L "orders" that can happen, even if we don't see them. If we labeled them to make them different, we can easily see this is a permutation problem, hence the $3!$.

For lollipop, we have $\frac{8!}{3!2!2!}$.

Sometimes, reframing a problem as a letter arrangement problem can be helpful, as these are easy to solve, and have a known solution method!

The principle of inclusion-exclusion is also a method of correcting some amount of overcounting.

## Pigeonhole Principle

Pigeons are a domesticated species of bird used to deliver messages. As they needed a place to stay when not doing this task, people built structures with a number of places (holes) for these pigeons to roost. However, if there were $n$ pigeons and $n-1$ places to roost, at least one of these pigeonholes would need to have more than one pigeon in it. Note that we are not guaranteed that there will be a box with two pigeons in it. All the pigeons could choose to try and squeeze into one hole! But it is true that in the best case scenario, each hole would have one pigeon and one would have two.

This is the idea behind pigeonhole principle: if there are $n$ items and $n-1$ boxes, or any number of boxes less than $n$, it is guaranteed that at least one box must contain more than one item.

This idea can be used for certain counting problems, though it's used in many places outside of combinatorics as well.

For example, imagine there's a drawer with 6 white socks, 6 grey socks, and 8 black socks. How many times would you have to take a sock from the drawer to guarantee a pair of matching socks?

Because there are only 3 colors, we're guaranteed that on the 4th sock, there's at least one matching pair. The 3 colors are our pigeonholes/boxes, and the socks themselves are the pigeons.

Pigeonhole principle can be applied to ensure more than _any number_ are in a specific category as well. We're not restricted to showing there must be at least 2 pigeons in a box. The same reasoning applies: lay out the best case scenario, where all the boxes have fewer than the desired number, then show that when they're all at "maximum capacity," we still have some left over.

For example, consider a box of 24 donuts being left in an office of 5 people. If the box is empty at the end of the day, can we show that at least one person ate at least 5 donuts?

If every person takes 4 donuts, there will still be 4 leftover. This cannot be, since the box was empty, so we must make at least one person take 5 donuts.

Remember, we cannot guarantee any one person ate exactly 5 donuts, or that all people ate a certain number. There could be some donut-eating champion in the office who took all 24 before the others had a chance to even take one.

Pigeonhole allows us to make an "at least" condition, which is not strong, but can still be powerful in the right set of circumstances.