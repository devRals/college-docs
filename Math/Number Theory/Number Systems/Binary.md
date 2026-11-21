**Binary** is a positional numeral system with base $2$. It uses only two digits: $0$ and $1$.

Binary is the fundamental number system used by computers and digital electronics because electronic circuits can represent two states, commonly interpreted as ON and OFF.

## 1. Digits and Base

Binary uses:

$$
\{0,1\}
$$

Each position represents a power of $2$.

For example:

$$
1011_2
$$

Its decimal value is:

$$
1\times2^3+0\times2^2+1\times2^1+1\times2^0
$$

$$
=8+0+2+1=11
$$

Therefore:

$$
1011_2=11_{10}
$$

## 2. Binary Place Values

| Position | Power | Value |
| -------- | ----- | ----: |
| 4th      | $2^3$ |     8 |
| 3rd      | $2^2$ |     4 |
| 2nd      | $2^1$ |     2 |
| 1st      | $2^0$ |     1 |

Each position from right to left represents an increasing power of 2.

## 3. Binary Arithmetic

Binary supports the same basic arithmetic operations as decimal.

Basic addition rules:

| Operation | Result |
| --------- | ------ |
| $0+0$     | 0      |
| $0+1$     | 1      |
| $1+0$     | 1      |
| $1+1$     | 10     |

In binary, $1+1=10$ because the result is two in decimal, which requires carrying to the next position.

Example:

$$
\begin{array}{r}
  101\\
+ 011\\
\hline
 1000
\end{array}
$$

## 4. Applications

- Internal representation of data in computers.
- Digital logic circuits and processors.
- Representing numbers using bits.
- Encoding text, images, and other information.

## 5. Related Concepts

- [[Number Systems]]
- [[Base Conversion]]
- [[Octal]]
- [[Decimal]]
- [[Hexadecimal]]
- [[Bits and Bytes]]
- [[Boolean Algebra|Binary Arithmetic]]

## Summary

Binary is the base-2 numeral system and uses only $0$ and $1$. It is the foundation of digital computing and data representation.