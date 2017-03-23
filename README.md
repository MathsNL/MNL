# Mathematical Notation Language

This repository will be the main source of documentation behind MNL, as well 
as discussion on the project.  MNL is an alternative notation for mathematics, 
with the intentions of reducing ambiguity and verbosity, and improving 
the intuitive aspect of mathematical notation.

Currently, MNL is only a conceptual notation, which we hope to turn into a 
plain (typed) text notation, as well as support for direct conversion between 
writing, text, LaTeX and a programming language, which will likely be 
functional.

## Background
Our interest in this project
started with personal grievances with the standard notation.

Also, as mathematicians that enjoy programming and programmers that enjoy 
mathematics, we want a notation that allows us to type out our mathematics 
without TeX or lots of brackets and clunky notation. We also don't want to 
over-complicate things, so we'll strip down a lot of the duplicates and 
context-grammars in the standard notation.

We also want to be able to convert MNL to standard notation through an
intermediate language, as well as to mathematics libraries in common use
such as TeX and SVG. From here, PDFs can be generated easily, allowing an
easy conversion between mathematics and text on a screen.

As mentioned above, we're all programmers here. It would also be useful to have 
a system like wolfram alpha to parse MNL files and get out a new MNL file with 
solutions or simplified versions of functions, expressions and equations.

## Aims

### Minimising verbosity
Some notation for mathematics can be 
verbose compared to others (compare, for example, the simple notation for 
indices, yet the need for an entire $\log$ function for a relatively similar 
operation).  We aim to minimise this verbosity (of course, not all notation 
can be minimal) and, through this, allow quick and easy writing and typing 
of mathematics.  

### Removing ambiguity
The standard equals operator ($=$) can be an equivalence, an identity, a 
relation, or an assignment.  Whilst these operations are similar, they can 
be very different and using the same operator is ambiguous. We aim to remove 
this ambiguity, and make different operations clearly different.  
### Improving clarity
Along a similar vein, we aim to improve notation such that similar operations 
appear similar (but not the same). This is necessary such that those learning 
mathematics can intuitively see that the operations are similar. A perfect 
example is that of logs, indices and roots. These operations are all very 
similar, yet the notation is hugely different.  

### Written--Typed conversion
As both programmers and mathematicians, we aim to make conversion between 
written and typed mathematics simple. Whether this be from written notation 
to \TeX, or written notation to standard typed text.

## How can I help?

At present, this project is motivated purely by interest and is handled by 
the main contributors only. However, any suggestions and discussion on the 
language and notation is invaluable and we encourage it. 

If you have any thoughts, disagreements, clarifications or ideas, feel free 
to open an issue and discuss it with us.
