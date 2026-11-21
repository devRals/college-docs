**Hexadecimal** is a positional numeral system with base $16$. It uses sixteen symbols: the digits $0$–$9$ and the letters $A$–$F$.

It is widely used in computer science because it provides a compact and readable representation of binary data.

## 1. Digits and Base

Hexadecimal uses:

$$
\{0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F\}
$$

Letters represent values greater than 9:

| Symbol | Decimal Value |
|---|---:|
| A | 10 |
| B | 11 |
| C | 12 |
| D | 13 |
| E | 14 |
| F | 15 |

Each position represents a power of $16$.

Example:

$$
2A_{16}
$$

Its decimal value is:

$$
2\times16^1+10\times16^0
$$

$$
=32+10=42
$$

Therefore:

$$
2A_{16}=42_{10}
$$

## 2. Hexadecimal Place Values

| Position | Power | Value |
|---|---|---:|
| 4th | $16^3$ | 4096 |
| 3rd | $16^2$ | 256 |
| 2nd | $16^1$ | 16 |
| 1st | $16^0$ | 1 |

## 3. Relationship with Binary

Since:

$$
16=2^4
$$

Each hexadecimal digit corresponds to exactly four binary bits.

| Hexadecimal | Binary |
|---|---|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |
| A | 1010 |
| B | 1011 |
| C | 1100 |
| D | 1101 |
| E | 1110 |
| F | 1111 |

Example:

$$
10101111_2=AF_{16}
$$

## 4. Applications

- Representing memory addresses.
- HTML and CSS color codes, such as `#FF0000`.
- Representing machine code and binary data.
- Debugging and examining computer memory.
- Representing individual bytes in a readable format.

## 5. Related Concepts

- [[Number Systems]]
- [[Base Conversion]]
- [[Binary]]
- [[Octal]]
- [[Decimal]]
- [[Bits and Bytes]]

## Summary

Hexadecimal is the base-16 numeral system. It uses digits $0$–$9$ and letters $A$–$F$. Because each hexadecimal digit represents four binary bits, it is especially useful for representing computer data compactly.