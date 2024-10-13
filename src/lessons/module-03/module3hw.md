<!--meta exposure: repeat -->
<!--meta assessmentFormat: ProblemSet -->
<!--meta submissionVia: Gradescope -->
<!--meta instructionType: specific -->
<!--meta submissionFormatFlexibility: no -->
<!--meta submissionTopicFlexibility: no -->
<!--meta rubricAvailable: no -->
<!--meta rubricShared: no -->
<!--meta groupWork: no -->
<!--meta automatedGrading: 0 -->
<!--meta studentInstructionsLink: course-discrete-mathematics/src/lessons/module-03/module3hw.md -->
<!--meta topics:  -->

# Homework Set 3

## Submitting Your Work

Your work must be submitted to Anchor for degree credit and to Gradescope for grading.

**For any work completed outside of GitHub or Gradescope:**

1. **Typeset your work in LaTeX**.
 - You should use \\begin\{enumerate\} to create a numbered list, and your solutions to each problem should match with the corresponding number on the assignment.
 - For example, if an assignment has 10 numbered problems, your enumerate should have 10 \\item commands, with your solution(s) to problem 1 under the first \\item, problem 2 under the second and so on.
 - If you skip a problem, just leave the \\item blank, otherwise the numbers of your solutions will not match the assignment document.
[Here is an example Overleaf document showcasing this format.](https://www.overleaf.com/read/zqjgpnxycycd#e88392)
2. Compile into a PDF. This can be done easily through an Overleaf account, otherwise you will need to install LaTeX.
3. Submit the pdf to [Gradescope](https://www.gradescope.com) via the appropriate submission link for the course.
4. Upload the pdf to Anchor using the form below.

> **Note:** Anchor submissions can occur at any time during the term, but it is **critical** that you upload all of your work to
> Anchor before the last day of the term.  Gradescope submissions must be submitted before the deadline (or the late deadline, if applicable).

#### It is required that all assignments are submitted as a PDF generated from a LaTeX document.

#### Assignments submitted in any other form will earn zero credit.

1. **[15 points]** Determine whether the following problems are recursive problems.

    a. $R(0) = 1$, $R(1) = 1$, $R(n) = 2R(n-1) + R(n-2)$

    b. $R(1) = 0$, $R(n) = 5R(n-1)$
    
    c. $R(0) = 0$, $R(n) = n$
    
    d. $R(1) = 1$, $R(n) = 2R(\frac{n}{2}) + 5$
    
    e. $R(1) = 1$, $R(n) = R(1)$


2. Solve the following recurrence relations:

    a. **[5 points]** $R(0) = 3$, $R(n) = 3R(n-1)$
    
    b. **[10 points]** $R(0) = k$, $R(n) = bR(n-1)$, where $b$ and $k$ are integers.
    
    c. **[5 points]** $R(1) = 0$, $R(n) = R(\frac{n}{5}) + 1$, where $n$ is always of the form $n = 5^k$
    
    d. **[10 points]** $R(1) = 0$, $R(n) = R(\frac{n}{b}) + c$, where $n$ is always of the form $n = b^k$, and $b, c$ are integers.

3. **[35 points]** Show that the following recursive relations have the closed forms given.

    a. $R(1) = 1$, $R(n) = R(n-1) + 2n-1$. Closed form: $n^2$
    
    b. $R(1) = 1$, $R(n) = \frac{n}{n-1}R(n-1)$. Closed form: $n$
    
    c. $R(1) = 1$, $R(n) = R(n-1) + n$. Closed form: $\frac{n(n+1)}{2}$
    
    d. $R(0) = 1$, $R(1) = 1$, $R(n) = 2R(n-1) - R(n-2)$. Closed form: $1$
    
    e. $R(1) = 5$, $R(n) = 5R(\frac{n}{2})$, where $n = 2^k$. Closed form: $5^{k+1}$
    
    f. $R(1) = 1$, $R(n) = R(\frac{n}{2}) + n$, where $n = 2^k$. Closed form: $2n-1$
    
    g. $R(1) = 0$, $R(n) = R(\frac{n}{2}) + \log_2{(n)}$, where $n = 2^k$. Closed form: $\frac{k(k+1)}{2}$

4. **[10 points]** Write a recursive function for one of the problems in problem 2. Capture your code here, either by copying it to the LaTeX document, or inserting it as an image.
