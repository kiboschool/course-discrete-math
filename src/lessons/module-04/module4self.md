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
<!--meta studentInstructionsLink: course-discrete-mathematics/src/lessons/module-04/module4self.md -->
<!--meta topics:  -->

# Week 4: Self-Guided Problems

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

1. Find the mistake in the following proofs:

- All odd numbers are prime.

Proof.

Every prime number, except for $2$, are odd.

Therefore, all odd numbers are prime.

QED

- All odd numbers $> 2$ are prime.

Proof.

Every even number greater than $2$ is composite (not prime).

Therefore, all odd numbers greater than $2$ are prime.

QED

- Every number is not prime.

Proof.

Base case: $1$ is not prime.

For every other number, we can determine that $n = 1 \cdot n$. So all other numbers are composite, since they can be written as a multiplication of two numbers

QED

2. Prove the following in at least 2 different ways:


- If $n^2$ is even, $n$ is even.
- The sum of the numbers from $1$ to $n$ is $\frac{n(n+1)}{2}$.
- The sum of any two odd numbers is even.


3. We can prove that $\sqrt{2}$ is irrational via this proof:

Proof.

Assume $\sqrt{2}$ is rational.

By definition of rational, $\sqrt{2} = \frac{p}{q}$ where $p$ and $q$ are integers, and $p$ and $q$ share no divisors. (Note: this is so the fraction is in simplest form).

Squaring both sides, we get $2 = \frac{p^2}{q^2}$

Multiplying both sides by $q^2$: $2q^2 = p^2$.

Since $q$ is an integer, $q^2$ is an integer, and by definition of even, $p^2$ is even. Below, you'll prove that if $n^2$ is even, $n$ is even, so we know $p$ is even.

Let $p = 2k$, where $k$ is an integer

$2q^2 = (2k)^2 = 4k^2$

Dividing by $2$: $q^2 = 2k^2$. Since $k$ is an integer, $k^2$ is an integer, and by definition of even, $q$ is even.

This is a contradiction: If $p$ and $q$ are both even, then the fraction is not in lowest terms, as we required.

Therefore, $\sqrt{2}$ is irrational.

QED

What other numbers can you prove are irrational using a similar proof? Complete the proof for one of these numbers.

4. Ask ChatGPT to prove a mathematical statement or theorem. How did it do? We will discuss where ChatGPT succeeds and fails in class, so try to come up with a unique claim for ChatGPT to prove.

5. Are there other indicators that were not discussed that could help decide what proof type should be used? What are they?

6. Of the 4 main proof types discussed this week, which do you find most challenging?