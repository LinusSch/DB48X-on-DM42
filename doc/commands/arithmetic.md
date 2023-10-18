# Arithmetic

## + (add)

Add two values.

* For integer, fractional, decimal or complex numbers, this performs the
  expected numerical addition. For example, `1 2 +` is `3`.
* For equations and symbols, build a sum, eliminating zero additions if
  [autosimplify](#autosimplify) is active.
* For lists, concatenate lists, or add objets to a list. For example, `{ A } { B
  } +` is `{ A B }`, and `{ A B C } "D" +` is `{ A B C "D" }`.
* For text, concatenate text, or concatenate the text representation of an
  object to an existing text. For example `"X" "Y" + ` gives `"XY"`, and
  `"X=" 1 +` gives `"X=1"`.

## - (sub)

Subtract two values

* For integer, fractional, decimal or complex numbers, this performs the
  expected numerical subtraction. For example, `1 2 -` is `-1`.
* For equations and symbols, build a difference, eliminating subtraction of 0 if
  [autosimplify](#autosimplify) is active.

## + (add)

Add two values.

* For integer, fractional, decimal or complex numbers, this performs the
  expected numerical addition. For example, `1 2 +` is `3`.
* For vectors and matrices, add individual elements. For example,
  `[ 1 2 3 ] [ 4 5 6 ] +` is `[ 5 7 9 ]`.
* For equations and symbols, build a sum, eliminating zero additions
  when [autosimplify](#autosimplify) is active.
* For lists, concatenate lists, or add objets to a list. For example, `{ A } { B
  } +` is `{ A B }`, and `{ A B C } "D" +` is `{ A B C "D" }`.
* For text, concatenate text, or concatenate the text representation of an
  object to an existing text. For example `"X" "Y" + ` gives `"XY"`, and
  `"X=" 1 +` gives `"X=1"`.

## - (sub)

Subtract two values

* For integer, fractional, decimal or complex numbers, this performs the
  expected numerical subtraction. For example, `1 2 -` is `-1`.
* For vectors and matrices, subtract individual elements. For example,
  `[ 1 2 3 ] [ 1 3 0 ] -` is `[ 0 -1 3 ]`.
* For equations and symbols, build a difference, eliminating subtraction of 0
  when [autosimplify](#autosimplify) is active.


## × (*, mul)

Multiply two values.

* For integer, fractional, decimal or complex numbers, this performs the
  expected numerical multiplication. For example, `3 2 *` is `6`.
* For vectors, multiply individual elements (this is a deviation from HP48).
  For example, `[ 1 2 3 ] [ 4 5 6 ] +` is `[ 4 10 18 ]`.
* For matrices, perform a matrix multiplication.
* For a matrix and a vector, apply the matrix to the vector.
* For equations and symbols, build a product, eliminating mulitplication by 1
  or 0 when [autosimplify](#autosimplify) is active.
* For a list and a positive integer, repeat the list For example, `{ A } 3 *`
  is `{ A A A }`.
* For a text and a positive integer, repeat the text. For example `"X" 3 * `
  gives `"XXX"`.


## ÷ (/, div)

Divide two values two values

* For integer, build a fraction. For example `1 7 /` gives `1/7`.
* For fractional, decimal or complex numbers, this performs the
  expected numerical division. For example, `1. 2. /` is `0.5`.
* For vectors, divide individual elements. For example,
  `[ 1 2 3 ] [ 3 2 1 ] /` is `[ 1/3 1 3 ]`.
* For equations and symbols, build a ratio, eliminating division by one
  and division of 0 when [autosimplify](#autosimplify) is active.


## ↑ (^, pow)

Raise to the power

* For integer, fractional, decimal or complex numbers, this raises the
  value in level 2 to the value in level 1. For example, `2 3 ↑` is `8`.
* For vectors, raise individual elements in the first vector to the power of the
  corresponding element in the second vector.
* For equations and synbols, build an expression, eliminating special cases
  when [autosimplify](#autosimplify) is active.


## xroot

Raise to the inverse power. `X Y xroot` is equivalent to `X Y inv pow`.


# Integer arithmetic and polynomials

## SETPREC
Set the current system precision


## GETPREC
Get the current system precision


## FLOOR
Largest integer less than the input


## CEIL
Smallest integer larger than the input


## IP
Integer part of a number


## FP
Fractional part of a number


## MODSTO
Set the current system modulo for all MOD operations


## MODRCL
Get the current system modulo


## POWMOD
Power operator MOD the current system modulo


## MOD
Remainder of the integer division


## SQ
Square of the input


## NEXTPRIME
Smallest prime number larger than the input


## FACTORIAL
Factorial of a number


## ISPRIME
Return true/false (1/0) if a number is prime or not


## MANT
Mantissa of a real number (M*10<sup>exp</sup>)


## XPON
Exponent of a number represented as (M*10<sup>exp</sup>)


## SIGN
Sign of a number, -1, 0 or 1.

For complex numbers, returns a unit number on the unit circle with the same
argument as the original number.


## PERCENT
Percentage of a number


## PERCENTCH
Percentage of change on a number


## PERCENTTOT
Get percentage of a total


## GCD
Greatest common divisor


## LCM
Least common multiple


## IDIV2
Integer division, get quoteiant and remainder


## IQUOT
Quotient of the integer division


## ADDTMOD
Addition operator MOD the current system modulo


## SUBTMOD
Subtraction operator MOD the current system modulo


## MULTMOD
Multiplication operator MOD the current system modulo


## PEVAL
Evaluation of polynomial given as vector of coefficients


## PCOEF
Coefficients of monic polynomial with the given roots


## IEGCD
Extended euclidean algorithm


## IABCUV
Find integers u,v to solve a*u+b*v=c


## PTCHEBYCHEFF
Nth Tchebycheff polynomial


## PLEGENDRE
Nth Legendre polynomial


## PHERMITE
Nth Hermite polynomial as used by physics


## PTCHEBYCHEFF2
Nth Tchebycheff polynomial of the second kind


## PHERMITE2
Nth Hermite polynomial as used in probabilities


## DIV2
Polynomial euclidean division as symbolic


## PDIV2
Polynomial euclidean division as coefficient vector


## PDER
Derivative of polynomial as coefficient vector


## PINT
Integration of polynomials as coefficient vector


## PMUL
Multiplication of polynomials as coefficient vectors


## PADD
Addition of polynomials as coefficient vector


## PSUB
Subtraction of polynomials as coefficient vector


## MIN
Smallest of 2 objects


## MAX
Largest of 2 objects


## RND
Round a number to the given number of figures


## TRNC
Truncate a number to the given number of figures


## DIGITS
Extract digits from a real number


## PROOT
All roots of a polynomial


## PREVPRIME
Largest prime smaller than the input


## FACTORS
Factorize a polynomial or number
