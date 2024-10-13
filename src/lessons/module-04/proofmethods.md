
# Proof Methods and Techniques

In mathematics, it is important to prove that something is true, rather than assume. Proofs require a deep understanding of logical thinking and intuition, one that helps with systematically solving problems.

## Readings

> Please read this first before moving on to the documents here on Anchor.
> As a reminder, and for reference, specific chapters are referenced at the beginning of the section for which they are relevant.
> Feel free to go back to the text(s), or review it if there's been a break since you last read the material.
> The readings on Anchor have some information in common with the text(s). This is to ensure you see the information from some different perspectives.

[Discrete Mathematics: An Open Introduction](https://discrete.openmathbooks.org/dmoi3/dmoi.html), [Chapter 3.2](https://discrete.openmathbooks.org/dmoi3/sec_logic-proofs.html)

[Applied Discrete Structures](https://discretemath.org/ads/ads.html) [Chapter 3.7](https://discretemath.org/ads/s-induction.html)

## General Proof Basics

All proofs start with the word proof. It indicates to the reader that the official proof is begining.

The contents of a proof will be different, depending on the claim being proven and the style of proof. Each step should logically follow from the line before it, though exactly what this means can vary. Some textbooks contain proofs which have large leaps in logic between steps, sometimes even large enough that homework may involve proving that the logical leap is valid.

In general, this is not good practice. A proof should be readable by a colleague, with no missing gaps or steps left to be proven. Each line should directly follow or reference a previous line, and some reason should be given that each line is true. Usually, a definition, theorem, or property will suffice.

Once the proof is complete, there are a few ways to denote the end. QED is a common ending, standing for "quod erat demonstrandum," a latin phrase that means "which was to be demonstrated. Sometimes people will write the English translation, or a similar sentiment such as "As desired." If you want to be sure people know where a proof ends, you can use a box, either a filled in or empty box. This is another common proof ending, and one that is not ambiguous.

In LaTeX, you can use the \\begin{proof} and \\end{proof} commands, and this box, along with the starting _Proof_ will be created for you.