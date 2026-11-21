A **remainder** is the amount left over after dividing one integer by another.

When a number cannot be divided evenly, the remainder represents the part that is left after removing as many complete groups as possible.

Remainders are important in [[Number Theory]], especially in [[Modular Arithmetic]], [[Congruence]], and [[Base Conversion]].

## 1. Division Algorithm

The Division Algorithm states that for any integer $a$ and positive integer $b$, there exist unique integers $q$ and $r$ such that:

$$
a=bq+r
$$

Where:

- $a$ = Dividend (the number being divided).
- $b$ = Divisor (the number dividing the dividend).
- $q$ = Quotient (the integer result of division).
- $r$ = Remainder (the amount left over).

The remainder must satisfy:

$$
0\leq r<b
$$

This means that the remainder is always non-negative and smaller than the divisor.

### Example

Divide $17$ by $5$.

$$
17=5\times3+2
$$

Therefore:

- Dividend: $17$
- Divisor: $5$
- Quotient: $3$
- Remainder: $2$

We can express this as:

$$
17\bmod5=2
$$

## 2. The Modulo Operation

The **modulo operation** calculates the remainder of an integer division.

It is represented by the symbol $\bmod$.

$$
a\bmod b=r
$$

Where $r$ is the remainder when $a$ is divided by $b$.

### Examples

$$
17\bmod5=2
$$

$$
20\bmod6=2
$$

$$
24\bmod6=0
$$

$$
29\bmod10=9
$$

When the modulo result is zero, the dividend is perfectly divisible by the divisor.

### Important Properties

For positive integers $a$ and $b$:

**1. Modulo with a smaller number**

If $0\leq a<b$, then:

$$
a\bmod b=a
$$

Example:

$$
3\bmod7=3
$$

**2. Modulo with equal numbers**

$$
a\bmod a=0
$$

Example:

$$
8\bmod8=0
$$

**3. Modulo with zero**

$$
0\bmod b=0
$$

For any positive integer $b$.

**4. Modulo with multiples**

If $a$ is divisible by $b$, then:

$$
a\bmod b=0
$$

Example:

$$
36\bmod9=0
$$

## 3. Remainders and Negative Numbers

The Division Algorithm also works with negative integers.

We still require:

$$
0\leq r<b
$$

For example:

$$
-7=(-3)\times4+5
$$

Therefore, using the non-negative remainder convention:

$$
-7\bmod4=1
$$

This is important because programming languages can implement remainder and modulo operations differently for negative numbers.

## 4. Applications of Remainders

### Base Conversion

When converting decimal integers into another base, we repeatedly divide by the target base and collect the remainders.

Example:

$$
13\bmod2=1
$$

These remainders help construct the binary representation.

See [[Base Conversion]].

### Checking Divisibility

A number is divisible by another number if its remainder is zero.

$$
a\bmod b=0
$$

Example:

$$
42\bmod7=0
$$

Therefore, $42$ is divisible by $7$.

See [[Divisibility]].

### Clock Arithmetic

A 12-hour clock is an example of arithmetic involving remainders.

If it is 10 o'clock and 5 hours pass:

$$
(10+5)\bmod12=3
$$

The resulting time is 3 o'clock.

See [[Modular Arithmetic]].

## 5. Related Concepts

- [[Number Theory]]
- [[Division Algorithm]]
- [[Modulo Operation]]
- [[Modular Arithmetic]]
- [[Congruence]]
- [[Divisibility]]
- [[Base Conversion]]

## Summary

A remainder is the amount left after integer division.

The Division Algorithm expresses this relationship as:

$$
a=bq+r
$$

With the condition:

$$
0\leq r<b
$$

The modulo operation calculates this remainder:

$$
a\bmod b=r
$$

Remainders are fundamental to modular arithmetic and congruence.