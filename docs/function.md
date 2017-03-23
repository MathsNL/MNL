# Function notation

## Assignment
To declare a function and assign it, you use a colon followed by an equality sign `:=`. For example

`f(x) := x^2 + 2`

The function, f(x), shown above will be used as an example for the rest of this document.

## Evaluation
Evaluation is used when getting the value of a function. Evaluation uses an arrow symbol, or dash greater-than `->`. For example

`f(5) -> 5^2 + 2 -> 27`

## Composition
For when you want to run a function on itself many times, composition can be used. A notation for this is still undecided but some ideas have been proposed.
```f(f(x)) -> f_2(x)```
The main argument against this is that in the following example `x_2(5)` is indistinguishable from `f_2(5)`
```
x_2(5) -> x_2 . 5

f_2(5) -> f(f(5))
```

Alternatively, we could have the subscript follow the brackets. 
```f(f(x)) -> f(x)_2```
This would remove the above ambiguity but differs much more than the current system which could cause some confusion.

Finally, a more controversial idea but still fair to question is replacing the parenthesis in functions for square brackets which would stop them from being used to structure algebra
```
f [x] := x^2 + 2
f [5] -> 5^2 + 2 -> 27
```

Or we could do something else all together.
```
g x; y) := x + y
2 + g 6; 5) -> 2 + 6 + 5 -> 13
```
In this case, g is a function that adds together x and y. Opinions and suggestions **greatly** appreciated.

## Inversion
Inversion does the opposite of a function. The three main ideas for showing inversion are

1.	Suffix the function with 'inv', `invf(f(x)) -> x`
2.	Use a negative composition value. 
	*	This will be expanded on when a composition notation has been determined as this has some interesting implications.