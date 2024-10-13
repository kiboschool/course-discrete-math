# Chinese Remainder Theorem

We quote Chinese Remainder Theorem, but why do we know it's true?

Consider a $5$ by $7$ grid, where the columns are residues mod 5 and the rows are residues mod 7. Lebel these accordingly, with the bottom right square representing 0 for both, and counting up on the row and column.

We found that $34$ is the solution for 4 and 6 (respectively).

We can also pretty easily fill in that 0 and 0 would be 0.

Likewise, if both are 1, 2, 3, or 4, then the answer should just be that residue.

>Think first: Draw this grid on paper, and try to fill in more of the boxes, either by solving the system or noticing a pattern.

I **highly encourage** you to write out the table yourself first, but you should see that the answers are listed in order if you keep following a diagonal line.

In particular, if the line reaches the top side, you continue by wrapping around to the bottom edge, and if the line hits the right hand side, it should wrap around to start again at the left.

Consider this: Every time we increase by 7, we move 7 to the right. This means every time we touch the right border, we reach a number that's divisible by 7.

The same happens with 5 along the top.

If we are able to move through every box, there will be $35$ different answers, which is the number of residues mod $35$.

We will only reach the top right-hand corner if we have a multiple of 5 and 7. Since their LCM is $35$, this is the lowest possible number of boxes we will need to pass through. We have unique solutions!

I will demo this in class, but feel free to experiment with the tool below. Note that it does not do the same thing as described above, but shows another way to find the solution. The green stripe is the remainder of the second modulus, and the blue boxes are the remainders of the first modulus. Where they intersect is the answer!

<div style="position: relative;"><iframe scrolling="no" frameborder="0" src="https://www.wolframcloud.com/obj/demonstrations/Published/SeeingTheChineseRemainderTheorem?_view=EMBED" style="border:0;"></iframe></div>