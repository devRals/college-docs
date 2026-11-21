**Base conversion** is the process of converting a number from one numeral system to another without changing its actual numerical value.

Different number systems use different bases (radixes), such as:

- [[Binary]] — Base 2
- [[Octal]] — Base 8
- [[Decimal]] — Base 10
- [[Hexadecimal]] — Base 16

For example, all of the following represent the same numerical value:

$$
1011_2 = 13_8 = 11_{10} = B_{16}
$$

Only the representation changes, not the value.

---

## 1. Converting Any Base to Decimal

To convert a number from another base into decimal, use **positional notation**.

Each digit is multiplied by its corresponding power of the original base.

### General Formula

For a number with base $b$:

$$
(a_na_{n-1}\ldots a_1a_0)_b
$$

Its decimal value is:

$$
\sum_{i=0}^{n} a_i \times b^i
$$

Where:

- $a_i$ is the digit at position $i$.
- $b$ is the original base.
- $i$ is the position, starting from the right at zero.

### Example: Binary to Decimal

Convert $(1011)_2$to decimal.

Expand the number using powers of 2:

$$
1011_2 =
1\times2^3 +
0\times2^2 +
1\times2^1 +
1\times2^0
$$

Calculate:

$$
=8+0+2+1
$$

$$
\boxed{1011_2=11_{10}}
$$

### Example: Octal to Decimal

Convert $(157)_8$ to decimal.

$$
157_8 =
1\times8^2 +
5\times8^1 +
7\times8^0
$$

$$
=64+40+7
$$

$$
\boxed{157_8=111_{10}}
$$

### Example: Hexadecimal to Decimal

Convert $(2A)_{16}$ to decimal.

Remember that $A=10$.

$$
(2A)_{16} =
2\times16^1 +
10\times16^0
$$

$$
=32+10
$$

$$
\boxed{(2A)_{16}=42_{10}}
$$

---

## 2. Converting Decimal to Another Base

To convert a positive integer from decimal into another base, repeatedly divide the number by the target base and record the remainders.

The final result is obtained by reading the remainders **from bottom to top**.

### General Algorithm

Given a decimal integer $N$ and target base $b$:

1. Divide $N$ by $b$.
2. Record the remainder.
3. Replac $N$ with the quotient.
4. Repeat until the quotient becomes zero.
5. Read the remainders in reverse order.

The [[Remainders|remainder]] is calculated using:

$$
r=N\bmod b
$$

The quotient is:

$$
q=\left\lfloor\frac{N}{b}\right\rfloor
$$

### Example: Decimal to Binary

Convert $13$ to binary.

Divide repeatedly by 2:

| Division  | Quotient | Remainder |
| --------- | -------: | --------: |
| $13\div2$ |        6 |         1 |
| $6\div2$  |        3 |         0 |
| $3\div2$  |        1 |         1 |
| $1\div2$  |        0 |         1 |

Read the remainders from bottom to top:

$$
\boxed{13=(1101)_2}
$$

### Example: Decimal to Octal

Convert $83$ to octal.

| Division  | Quotient | Remainder |
| --------- | -------: | --------: |
| $83\div8$ |       10 |         3 |
| $10\div8$ |        1 |         2 |
| $1\div8$  |        0 |         1 |

Read from bottom to top:

$$
\boxed{(83)_{10}=123_8}
$$

### Example: Decimal to Hexadecimal

Convert $254$ to hexadecimal.

| Division    | Quotient | Remainder |
| ----------- | -------: | --------: |
| $254\div16$ |       15 |        14 |
| $15\div16$  |        0 |        15 |

Convert the remainders into hexadecimal symbols:

- $14=E_{16}$
- $15=F_{16}$

Read from bottom to top:

$$
\boxed{254=(FE)_{16}}
$$

---

## 3. Binary to Octal Conversion

Binary and octal have a special relationship:

$$
2^3=8
$$

This means that **every octal digit corresponds to exactly three binary digits**.

Instead of converting binary to decimal first, we can group binary digits directly.

### Conversion Algorithm

1. Start grouping binary digits from the right.
2. Create groups of three digits.
3. Add leading zeros to the left if necessary.
4. Convert each group into its corresponding octal digit.

### Example

Convert $(1101011)_2$ to octal.

First, group the digits from right to left:

$$
001\quad101\quad011
$$

Convert each group:

| Binary | Octal |
| ------ | ----: |
| $001$  |     1 |
| $101$  |     5 |
| $011$  |     3 |

Therefore:

$$
\boxed{(1101011)_2=153_8}
$$

---

## 4. Octal to Binary Conversion

This is the reverse of binary-to-octal conversion.

Each octal digit is replaced with its corresponding three-bit binary representation.

### Example

Convert $(157)_8$ to binary.

| Octal | Binary |
| ----- | ------ |
| 1     | 001    |
| 5     | 101    |
| 7     | 111    |

Combine the groups:

$$
001\quad101\quad111
$$

Remove unnecessary leading zeros:

$$
\boxed{157_8=1101111_2}
$$

---

## 5. Binary to Hexadecimal Conversion

Binary and hexadecimal also have a special relationship:

$$
2^4=16
$$

Therefore, every hexadecimal digit corresponds to exactly four binary digits.

### Conversion Algorithm

1. Start grouping binary digits from the right.
2. Create groups of four digits.
3. Add leading zeros to the left if necessary.
4. Convert each group into its corresponding hexadecimal digit.

### Example

Convert $(110101101)_2$ to hexadecimal.

Group the digits:

$$
0001\quad1010\quad1101
$$

Convert each group:

| Binary | Hexadecimal |
| ------ | ----------- |
| 0001   | 1           |
| 1010   | A           |
| 1101   | D           |

Therefore:

$$
\boxed{110101101_2=1AD_{16}}
$$

---

## 6. Hexadecimal to Binary Conversion

This is the reverse of binary-to-hexadecimal conversion.

Each hexadecimal digit is replaced with its corresponding four-bit binary representation.

### Example

Convert $(3B)_{16}$ to binary.

Remember that $B=11$.

| Hexadecimal | Binary |
| ----------- | ------ |
| 3           | 0011   |
| B           | 1011   |

Combine the groups:

$$
0011\quad1011
$$

Therefore:

$$
\boxed{3B_{16}=00111011_2}
$$

---

## 7. Converting Between Any Two Bases

What if we need to convert between two bases that don't have a direct conversion method?

A simple general approach is to use decimal as an intermediate system.

For example, to convert octal to hexadecimal:

$$
\text{Octal}
\rightarrow
\text{Decimal}
\rightarrow
\text{Hexadecimal}
$$

### Example: Octal to Hexadecimal

Convert $(157)_8$ to hexadecimal.

**Step 1: Convert octal to decimal.**

$$
157_8 =
1\times8^2+
5\times8^1+
7\times8^0
$$

$$
=64+40+7=111_{10}
$$

**Step 2: Convert decimal to hexadecimal.**

$$
111\div16=6\text{ remainder }15
$$

The remainder 15 corresponds to $F$.

$$
\boxed{157_8=6F_{16}}
$$

This method works for conversions between any valid positional bases.

---

## 8. Converting Fractional Numbers

The methods above focus on integers. Numbers containing fractional parts require a slightly different approach.

To convert a decimal fraction into another base, repeatedly multiply the fractional part by the target base and record the integer parts.

### General Algorithm

1. Multiply the fractional part by the target base.
2. Record the integer part of the result.
3. Keep the remaining fractional part.
4. Repeat until the fractional part becomes zero or the desired precision is reached.
5. Read the recorded integer parts from top to bottom.

### Example: Decimal Fraction to Binary

Convert $(0.625)_{10}$ to binary.

| Multiplication      | Integer Part | New Fraction |
| ------------------- | -----------: | -----------: |
| $0.625\times2=1.25$ |            1 |         0.25 |
| $0.25\times2=0.5$   |            0 |          0.5 |
| $0.5\times2=1.0$    |            1 |            0 |

Read the integer parts from top to bottom:

$$
\boxed{0.625_{10}=0.101_2}
$$

### General Positional Representation of Fractions

Digits after the radix point represent negative powers of the base.

For example:

$$
0.101_2 =
1\times2^{-1}
+
0\times2^{-2}
+
1\times2^{-3}
$$

$$
=0.5+0+0.125
$$

$$
=0.625_{10}
$$

---

## 9. Quick Reference Table

| Conversion                      | Method                         |
| ------------------------------- | ------------------------------ |
| Any base → Decimal              | Positional notation            |
| Decimal → Any base              | Repeated division              |
| Binary → Octal                  | Group into 3 bits              |
| Octal → Binary                  | Replace each digit with 3 bits |
| Binary → Hexadecimal            | Group into 4 bits              |
| Hexadecimal → Binary            | Replace each digit with 4 bits |
| Any base → Another base         | Convert through decimal        |
| Decimal fraction → Another base | Repeated multiplication        |

## 10. Common Mistakes

- Forgetting to read remainders from bottom to top when converting decimal integers.
- Grouping binary digits from the left instead of the right when converting to octal or hexadecimal.
- Forgetting to add leading zeros when creating complete binary groups.
- Using digits that are invalid for the selected base.
- Forgetting that hexadecimal letters represent values from 10 to 15.
- Confusing the numerical value with its representation in a particular base.

## Related Concepts

- [[Number Systems]]
- [[Positional Notation]]
- [[Binary]]
- [[Octal]]
- [[Decimal]]
- [[Hexadecimal]]
- [[Boolean Algebra|Binary Arithmetic]]
- [[Modular Arithmetic]]

## Summary

Base conversion allows us to represent the same numerical value in different numeral systems.

The most important techniques are:

1. Use positional notation to convert numbers into decimal.
2. Use repeated division to convert decimal integers into another base.
3. Use repeated multiplication to convert decimal fractions into another base.
4. Use bit grouping to convert directly between binary, octal, and hexadecimal.