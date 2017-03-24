# Function notation

## Assignment
To declare a funciton, use a colon followed by an equality sign `:=`. For example

`f(x) := x^2 + 2`

The function, f(x), shown above will be used as an example for the rest of this document.

## Evaluation
Evaluation is used when getting the value of a function. Evaluation uses an equals. For example

`f(5) = 5^2 + 2 = 27`

## Composition
For when you want to run a function on itself many times, composition can be used. A notation for this is still undecided but some ideas have been proposed.
```f(f(x)) == f_2(x)```
The main argument against this is that in the following example `x_2(5)` is indistinguishable from `f_2(5)`
```
x_2(5) == x_2 . 5

f_2(5) == f(f(5))
```

Alternatively, we could have the subscript follow the brackets. 
```f(f(x)) == f(x)_2```
This would remove the above ambiguity but differs much more than the current system which could cause some confusion.

Finally, a more controversial idea but still fair to question is replacing the parenthesis in functions for square brackets which would stop them from being used to structure algebra
```
f [x] := x^2 + 2
f [5] = 5^2 + 2 = 27
```

Or we could do something else all together.
```
g x; y) := x + y
2 + g 6; 5) = 2 + 6 + 5 = 13
```
In this case, g is a function that adds together x and y. 

We may begin looking into programming languages for inspiration. Opinions and suggestions **greatly** appreciated.

## Inversion
Inversion does the opposite of a function. The three main ideas for showing inversion are

1.	Prefix the function with 'inv', `invf(f(x)) == x`
2.	Use a negative composition value. 

### Negative Composition
If negative composition is accepted, this would make composing functions have similar rules to composing powers. 

*I will be using the first of the syntaxs in the [Composition](#composition) section for the following examples*

Let's say we have the function `f(x) := x^2 + 2`, when parsing itself as an argument, you now have two layers of the function, e.g. `f( f(x) )`. Parsing that as an argument to `f(x)` again, will make it have three layers and so on, adding 1 each time. `f(x) == f_1(x)`, the `1` is assumed in most cases but the one gives us important information. 
```
g(x) := f_3(x) == f( f( f(x) ) )

g(f_2(x)) == f_3( f_2(x) ) == f( f( f( f( f(x) ) ) ) )
	== f_5(x)
```
The example above shows that you add the compositions when combining them together. This is what gives us the idea of negative composition. `f_-1(x)` removes a layer, as adding negative one is the same as subtracting one.

This rule is similar to `x^n . x^m == x^(n+m)`. You may also remember that there's a second 'power rule', `(x^n)^m == x^(nm)`, well this also exists with composition.
```
g(x) := f_3(x)
g_2(x) == g(f_3(x)) == f_3(f_3(x))
```

In general
```
f_n(f_m(x)) == f_{n+m}(x)

g(x) := f_n(x)
g_m(x) == f_{nm}(x)
```
