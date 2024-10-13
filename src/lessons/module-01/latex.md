# LaTeX

LaTeX is a system for mathematical typesetting. It formats mathematical statements alongside text in a neat, easily-readable manner.

## Readings

> These texts are **recommended**, but not required. It may contain useful information, or information stated in a different way.

Recommended: [Overleaf Tutorial](https://www.overleaf.com/learn/latex/Tutorials), [Learn LaTeX in 30 Minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)

## Document Features

I would recommend trying these commands out as you read. Copy-paste them into a new LaTeX document!

To get started, create an Overleaf account, and click New Project, then Blank Project. Whenever you edit the LaTeX on the left hand side, you'll need to click the compile button to see your changes.

LaTeX files have the extension .tex, and these are the files to be edited. When compiled properly, using either Overleaf or a LaTeX compiler downloaded onto your machine, a PDF document will be created.

A LaTeX document can come in many forms, and needs a document type. Overleaf does this automatically. The top of many .tex files has the following command:

\documentclass{article}

Which specifies that the document is an article. There are other types, but this is more advanced than is necessary for a Discrete Math course.

Underneath the document type, packages can be added. This works similarly to programming packages. They allow for better commands, the addition of certain symbols, or some other addition that will improve the quality of the person writing the document, or the appearance of the document itself. The \usepackage command is needed to include a specific package. Overleaf automatically includes the graphicx package to allow for adding images to a document.

\usepackage{graphicx}

Underneath any packages, the title, author, and date of the document is often specified. To make these appear in the document, the \maketitle command is used inside the document.

\title{Example Title}
\author{Kiera Gross}
\date{January 2024}

All commands mentioned, with the exception of the \maketitle command, exist in the Preamble portion of a .tex file. These must all be placed before the \begin{document} command, which should contain the actual contents of the document to be displayed. This is why the \maketitle command exists inside the document. It tells the compiler to add these features to the final PDF.

\begin{document}

\maketitle

\end{document}

There is an end to the document as well. Be sure to place any content between the beginning and end of the document.

## Basic Text Features

The last part of LaTeX that Overleaf automatically creates is a section. Use the \section command to separate into a new section of the document.

\section{Introduction}

This is more useful for research papers, but will appear in homework documents to separate questions.

Typing sentences in LaTeX seems normal until a paragraph is needed. To create separate paragraphs, use two newlines, or a double backslash.

Paragraph one here. \\\\

Paragraph two here. 

Experiment with both. Note that the indentation may be different depending on the method chosen.

_Italics_, **Bold**, and Underline can all be done in LaTeX documents with simple commands.

\textit{Italic text}

\textbf{Bold text}

\underline{Underlined text}

LaTeX, in a fashion more similar to programming languages, allows in-line comments. Using the percent symbol (%) before any block of text will remove the text from the final PDF, only to be seen in the .tex file.

% this sentence would be a comment in a LaTeX file

## Advanced Text Features

The \begin command is not limited to beginning the document. This can also be used to create lists. Using enumerate creates a numbered list, while itemize creates a bulleted list. For both, use the begin and end commands, and use the \item command for each item in the list.

\begin{enumerate}

\item first item

\item second item

\end{enumerate}

\begin{itemize}

\item first bullet point

\item second bullet point

\end{itemize}

Tables can be done similarly, with the tabular used in the begin and end commands. rows are separated by a double backslash. Columns are separated by an ampersand (&). Directly after the begin command, specify the justification of each column (left (l), center (c), or right (r)), and whether lines should be drawn between them (using the pipe symbol: |). For lines between rows, use \hline after the double backslash.

\begin{tabular}{ l | c c }

corner & item 1 & item 2 \\\\

\hline

row 2 & row 2, item 1 & row 2, item 2 \\\\

row 3 & row 3, item 1 & row 3, item 2    

\end{tabular}

New LaTeX users should try changing different aspects of the table to see what happens.

For images, we need the graphicx package mentioned earlier, as well as the image file. When using Overleaf, this file must be uploaded to the project. Then use the begin and end command with figure as the input. Inside the figure, include your image using the \includegraphics command with the name of the file. Do not include the extension (.png, .jpeg, etc)!

\begin{figure}

\includegraphics{ImageNameWithoutExtension}

\caption{Add a caption here.}

\end{figure}

This will add the image to the document. LaTeX may place this image in an odd spot, as it wants to optimize the way the document looks. There are some additional commands that can be added to fix the size and location of the image. For a challenge, try finding how to center an image, how to set it to a specific size, and how to make it appear on the document where it appears in the .tex file.

To include hyperlinks in LaTeX documents, the hyperref package is needed.

\usepackage{hyperref}

Remember to put this in the preamble. Then, in the document, the \href command can be used.

\href{overleaf.com}{This is a Link}

The way links look by default can be odd, but changing the style is more advanced. There is documentation on how this might be done. Try finding one that would make links appear in a similar manner to most of the internet.

## Math Mode

Everything mentioned so far deals with adding text to a document. However, LaTeX's appeal is that it can format mathematical statements. To write mathematical statements, we must enter "math mode," which tells LaTeX that the text should be made into symbols rather than displaying as-is. There are three main ways to do this. One is to use double dollar signs ($).

\$\$ x = y \$\$

This will appear in math mode. Even with a simple statement, there is some difference between x = y in math mode and in text mode.

The other method is to use the begin and end commands with equation as input.

\begin{equation}

x = y

\end{equation}

This will also enter math mode, but it will also identify this particular math as an equation, and add a number as a label. 

Another way to specify an equation without having a number appear is to use a backslash with brackets (\\\[ \\\])

\\\[ x = y \\\]


All methods have their uses, but it is overall more common to see the dollar signs in use for simple assignments.

## Mathematical Notation

Most necessary mathematical notation will be provided in the first assignment. However, I recommend you experiment with different commands before attempting the assignment. Start with simple mathematical notation. How are fractions created in LaTeX? Exponents? Can you re-write some old problems or portions of the textbook using LaTeX?

In general, as is true in most of computer science, when you do not know how to do something, consult some documentation. Overleaf provides nice tutorials, and they often appear as the first result on a search engine for any LaTeX-related queries.

[Detextify](https://detexify.kirelabs.org/classify.html) is a useful tool if you cannot remember the name of the symbol you desire. Draw the symbol, and this service will attempt to find similar symbols. Be sure to use the package next to the symbol you choose before attempting to use the command in your LaTeX document! The app will also include whether the command is to be used in _math mode_ or _text mode_.
