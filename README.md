# Mathematical Notation Language

This repository will be the main source of documentation behind MNL.  
MNL is a conceptual notation potentially to be made into a functional programming language.

## Goals
As mathematicians that enjoy programming and programmers that enjoy mathematics, we want
a notation that allows us to type out our mathematics without TeX or lots of brackets (This isn't Lisp!)
We also don't want to over-complicate things, so we'll strip down a lot of the duplicates and context-grammars in the Standard Notation.

Another thing that would want to do is convert MNL to Standard Notation through an intermediate language to your favourite maths libraries,
such as TeX or SVG. From there you can go to PDF with one of the countless systems.

As mentioned above, we're all programmers here. It would be useful to have a system like wolfram alpha to parse MNL files
and get out a new MNL file with solutions or simplified versions of functions, expressions and equations.

## Language
MNL consists of 6 different components

*	Constants
*	Functions
*	Variables
*	Operations
*	Attributions
*	Text

###### The any of the following examples will be written in verbose standard notation.

### Constants
Constants are the same as those that exist within standard notation.
The only thing that may be changed is that MNL will provide a standard way to identify constants.

### Functions
Functions take inputs and return a single output. Functions could be as simple as 
`x` or more more complicated like `2 * x + 3 * y * y + 1 / z`

Functions almost have a recursive definition. Core functions exist as constants or variables
Complex functions consist of any function, either combined with another function via operators or modified using attributes

### Variables
Variables are a special case function. The most basic of function that cannot be described as a constant.
They consist of a name and have any value you want them to have,
but a value is not required for a variable to be used

### Operations
Operations cannot exist on their own. They require an operator to be paired with 2 functions, commonly with one function on either side of the operator

Operations combine two functions into one. For example

`2 + 3` Is exactly the same as `5`

### Attributions 
Attribution modifies a function to get a new function. This requires an attributer and a single function.
Common attributes in standard notation is the negative symbol.

`-f(x)` turns the function `f(x)` into the function `(0 - 1) * f(x)`

### Text
Text allows editors to write about their mathematics in much more detail that could otherwise be achieved.
This isn't exactly a mathematical notation but it it a common component of every mathematical work and therefore
we want to include it into MNL.