# Common notation

Spaces have no meaning at all, but use of spaces is advised to make work easier to read.
Semicolons or newlines can be used to close a statement.


## Representing Numbers

Digit separator: apostrophe/single-quote-mark `'`

`10 ^ 6 -> 1'000'000` 

Decimal: comma `,`

`2 / 5 -> 0,4`

## Operators

Addition: plus `+`

`5 + 6 -> 11`

Subtraction: hyphen/dash `-`

`3 - 2 -> 1`

Division: forward-slash `/`

Multiplication (avoid using cross unless performing cross multiplication): full-stop/period `.`

`2.3 -> 6`

Exponentiation: caret/circumflex `^`
```
x ^ 2 -> x . x
2 ^ 8 -> 256
```

## Calculus

### Integration
Integration is one of the core parts of calculus. 

Integral of y with respect to x from a to b `int(y)[x:=a; b]`
Integral of y with respect to x `int(y)[x]`

`int(y)` can be shortened to `I(y)`. 
Supported but advised against is the use of `integrate(y)`, which should only be used in speech

### Differentiation

Derived function of y with respect to x `dif(y)[x]`
Derivative of y with respect to x at a `dif(y)[x:=a]`

`dif(y)` can be shortened to `D(y)`. 
Supported but advised against is the use of `differentiate(y)`, which should only be used in speech

*Note: common functions are denoted with an initial capital.*
*Note: these notations are followed by -> to denote evaluation*
