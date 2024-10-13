<!--meta exposure: initial -->
<!--meta assessmentFormat: ProblemSet -->
<!--meta submissionVia: Gradescope -->
<!--meta instructionType: specific -->
<!--meta submissionFormatFlexibility: no -->
<!--meta submissionTopicFlexibility: no -->
<!--meta rubricAvailable: no -->
<!--meta rubricShared: no -->
<!--meta groupWork: yes -->
<!--meta automatedGrading: 0 -->
<!--meta studentInstructionsLink: course-discrete-mathematics/src/lessons/module-03/module3self.md -->
<!--meta topics:  -->

# Week 3: Self-Guided Problems

When you come to class, be ready to discuss these questions, and bring any additional questions you still have after this exercise!

## Submitting Your Work

Your work must be submitted to Anchor for degree credit and to Gradescope for grading.

**For any work completed outside of GitHub or Gradescope:**

1. **Typeset your work in LaTeX**.
 - You should use \\begin\{enumerate\} to create a numbered list, and your solutions to each problem should match with the corresponding number on the assignment.
 - For example, if an assignment has 10 numbered problems, your enumerate should have 10 \\item commands, with your solution(s) to problem 1 under the first \\item, problem 2 under the second and so on.
 - If you skip a problem, just leave the \\item blank, otherwise the numbers of your solutions will not match the assignment document.
2. Compile into a PDF. This can be done easily through an Overleaf account, otherwise you will need to install LaTeX.
3. Submit the pdf to [Gradescope](https://www.gradescope.com) via the appropriate submission link for the course.
4. Upload the pdf to Anchor using the form below.

> **Note:** Anchor submissions can occur at any time during the term, but it is **critical** that you upload all of your work to
> Anchor before the last day of the term.  Gradescope submissions must be submitted before the deadline (or the late deadline, if applicable).

#### It is required that all assignments are submitted as a PDF generated from a LaTeX document.

#### Assignments submitted in any other form will earn zero credit.

### Self-Guided Problems cannot be submitted late for any reason

This is due to the fact we discuss them in the class. Be sure to stay on top of these Self-Guided problems, and remember it is better to turn in an incomplete set than an empty one.

## Problems

1. Identify whether each of the following is recurrence or just a sequence.

- $a_n = 2a_{n-1} + 2$
- $a_n = 2a_{\frac{n}{2}}$
- $a_n = a_{n-2} + a_{0}$
- $a_n = a_0 + a_1 + a_2$

2. Solve the following recurrence relations. For the first three, assume $R(0) = 1$, for the last, assume $R(0) = k$:

- $R(n) = 5R(n-1)$
- $R(n) = bR(n-1)$, where $b$ is an integer.
- $R(n) = 5R(n-1) + 1$
- $R(n) = bR(n-1) + k$, where $b$ is an integer, and $k$ is an integer.

3. For one of these, show your solution is true by plugging in the closed form value of $R(n-1)$ on the right-hand side, and using algebraic steps that end in the closed form for $R(n)$. 

4. Write a recursive function for 1 example from problem 1, and 2 examples from problem 2. Take a screenshot of the code, and include it in your submission.

5. Try solving the problem 1 relation by inputting different values of n into your code. Do you believe there's a closed form solution? If so, what is it?

6. Compare your solution to the problem 2 relations by testing multiple n values with your code. Does your closed form line up with your code?
