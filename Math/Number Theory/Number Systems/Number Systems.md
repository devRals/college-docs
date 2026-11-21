---
tags:
  - MOCs
---
A **number system** is a method of representing numbers using a collection of symbols (digits) and mathematical rules.

Different number systems use different bases (radixes), which determine how many unique digits are available and how the positional value of each digit is calculated.

Number systems are fundamental to mathematics and computer science. Computers, for example, use binary internally, while humans commonly use decimal.

## 1. What is a Base?

A **base** (or radix) determines the number of unique digits used in a positional number system.

For a base `b`, the available digits range from `0` to `b - 1`.

Examples:

- Base 2: `0, 1`
- Base 8: `0, 1, 2, 3, 4, 5, 6, 7`
- Base 10: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9`
- Base 16: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F`

In hexadecimal, letters represent values greater than 9:

| Symbol | Decimal Value |
| ------ | ------------: |
| A      |            10 |
| B      |            11 |
| C      |            12 |
| D      |            13 |
| E      |            14 |
| F      |            15 |

## 2. Common Number Systems

### Binary (Base 2)

Binary uses only two digits: `0` and `1`.

It is the fundamental number system used by digital computers because electronic circuits can represent two states, commonly interpreted as OFF and ON.

Example:

`1011₂ = 11₁₀`

Each position represents a power of 2.

### Octal (Base 8)

Octal uses eight digits, from `0` to `7`.

It is sometimes used in computing as a more compact representation of binary numbers.

Example:

`13₈ = 11₁₀`

One octal digit corresponds to exactly three binary digits.

### Decimal (Base 10)

Decimal is the number system most commonly used in everyday life.

It uses ten digits, from `0` to `9`.

Example:

`253₁₀`

Decimal is based on powers of 10.

### Hexadecimal (Base 16)

Hexadecimal uses sixteen symbols: `0–9` and `A–F`.

It is widely used in computing because it provides a compact way to represent binary data.

Example:

`B₁₆ = 11₁₀`

One hexadecimal digit corresponds to exactly four binary digits.

## 3. Positional Notation

The value of a digit depends on both the digit itself and its position.

For example, consider the decimal number:

`253₁₀`

Its expanded representation is:

`2 × 10² + 5 × 10¹ + 3 × 10⁰`

`= 200 + 50 + 3`

The same principle applies to every positional number system.

General formula:

`(aₙ...a₂a₁a₀)ᵦ = aₙ × bⁿ + ... + a₂ × b² + a₁ × b¹ + a₀ × b⁰`

Where:
- `b` is the base.
- `a` represents a digit.
- The position determines the exponent.

See [[Positional Notation]] for a more detailed explanation.

## 4. Base Conversion

**Base conversion** is the process of representing the same numerical value in a different number system.

For example:

`1011₂ = 13₈ = 11₁₀ = B₁₆`

The numerical value stays the same; only its representation changes.

Common conversion methods include:

- Converting another base to decimal using positional notation.
- Converting decimal to another base using repeated division.
- Converting binary to octal by grouping binary digits in groups of three.
- Converting binary to hexadecimal by grouping binary digits in groups of four.

See [[Base Conversion]] for conversion algorithms, examples, and calculations.

## 5. Relationship Between Binary, Octal and Hexadecimal

Octal and hexadecimal are particularly useful because they make long binary numbers shorter and easier to read.

| Binary | Octal | Decimal | Hexadecimal |
| ------ | ----: | ------: | ----------: |
| 0000   |     0 |       0 |           0 |
| 0001   |     1 |       1 |           1 |
| 0010   |     2 |       2 |           2 |
| 0011   |     3 |       3 |           3 |
| 0100   |     4 |       4 |           4 |
| 0101   |     5 |       5 |           5 |
| 0110   |     6 |       6 |           6 |
| 0111   |     7 |       7 |           7 |
| 1000   |    10 |       8 |           8 |
| 1001   |    11 |       9 |           9 |
| 1010   |    12 |      10 |           A |
| 1011   |    13 |      11 |           B |
| 1100   |    14 |      12 |           C |
| 1101   |    15 |      13 |           D |
| 1110   |    16 |      14 |           E |
| 1111   |    17 |      15 |           F |

Note: The binary column shows four-bit representations, with leading zeros where necessary.

Important relationships:

- 1 octal digit = 3 binary bits.
- 1 hexadecimal digit = 4 binary bits.
- 1 hexadecimal digit = 4 binary bits = 16 possible values.

## 6. Number Systems and Modular Arithmetic

Number systems are closely related to division and remainders.

When converting decimal numbers into another base, repeated division and remainder calculations are commonly used.

For example, converting `13₁₀` to binary:

| Division | Quotient | Remainder |
| -------- | -------: | --------: |
| 13 ÷ 2   |        6 |         1 |
| 6 ÷ 2    |        3 |         0 |
| 3 ÷ 2    |        1 |         1 |
| 1 ÷ 2    |        0 |         1 |

Reading the remainders from bottom to top gives:

`13₁₀ = 1101₂`

The remainder is also the result of a modulo operation.

For example:

`13 mod 2 = 1`

This connects number-base conversion to [[Modular Arithmetic]].

## 7. Related Concepts

- [[Base Conversion]] — How to convert numbers between different bases.
- [[Boolean Algebra|Binary Arithmetic]] — Addition, subtraction, multiplication and division in binary.
- [[Modular Arithmetic]] — Arithmetic based on remainders.
- [[Divisibility]] — Understanding when one integer divides another.
- [[Bits and Bytes]] — Basic units of digital information.

## Summary

Number systems provide different ways of representing numerical values.

The most common systems in computing and mathematics are:

| Number System | Base | Digits   |
| ------------- | ---: | -------- |
| Binary        |    2 | 0–1      |
| Octal         |    8 | 0–7      |
| Decimal       |   10 | 0–9      |
| Hexadecimal   |   16 | 0–9, A–F |

Understanding bases, positional notation, and base conversion provides a foundation for studying computer architecture, digital electronics, and number theory.