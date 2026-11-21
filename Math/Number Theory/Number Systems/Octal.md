**Octal** is a positional numeral system with base $8$. It uses eight digits, from $0$ to $7$.

Octal is useful in computing because it provides a shorter representation of binary numbers. Every octal digit corresponds to exactly three binary bits.

## 1. Digits and Base

Octal uses:

$$
\{0,1,2,3,4,5,6,7\}
$$

Each position represents a power of $8$.

For example:

$$
157_8
$$

Its decimal value is:

$$
1\times8^2+5\times8^1+7\times8^0
$$

$$
=64+40+7=111
$$

Therefore:

$$
157_8=111_{10}
$$

## 2. Octal Place Values

| Position | Power | Value |
|---|---|---:|
| 4th | $8^3$ | 512 |
| 3rd | $8^2$ | 64 |
| 2nd | $8^1$ | 8 |
| 1st | $8^0$ | 1 |

## 3. Relationship with Binary

Since:

$$
8=2^3
$$

Each octal digit corresponds to exactly three binary digits.

| Octal | Binary |
|---|---|
| 0 | 000 |
| 1 | 001 |
| 2 | 010 |
| 3 | 011 |
| 4 | 100 |
| 5 | 101 |
| 6 | 110 |
| 7 | 111 |

Example:

$$
157_8=001\ 101\ 111_2
$$

Removing unnecessary leading zeros:

$$
157_8=1101111_2
$$

## 4. Applications

- Compact representation of binary numbers.
- Unix and Linux file permission notation, such as `755`.
- Some legacy computing systems and programming environments.

## 5. Related Concepts

- [[Number Systems]]
- [[Base Conversion]]
- [[Binary]]
- [[Decimal]]
- [[Hexadecimal]]
- [[Bits and Bytes]]

## Summary

Octal is the base-8 numeral system, using digits from $0$ to $7$. Its main advantage in computing is its direct relationship with binary, where one octal digit represents three bits.