# Bits and Bytes

**Bits and bytes** are fundamental units of digital information. They are used to measure data storage, memory, and data transfer in computer systems.

Computers represent information using binary digits, making bits and bytes closely connected to the [[Binary]] number system.

## 1. Bit

A **bit** (binary digit) is the smallest basic unit of digital information.

A bit can have only two possible values:

$$
0\quad\text{or}\quad1
$$

These values represent two possible states, such as OFF and ON.

For example:

$$
1011
$$

This sequence contains four bits.

## 2. Byte

A **byte** is a group of 8 bits.

$$
1\text{ Byte}=8\text{ bits}
$$

Example:

$$
10110101
$$

This binary sequence contains exactly one byte.

A byte can represent:

$$
2^8=256
$$

different possible combinations, ranging from:

$$
00000000_2=0
$$

to:

$$
11111111_2=255
$$

## 3. Larger Units of Data

Common data storage units include:

| Unit          |        Size |
| ------------- | ----------: |
| Bit           |       1 bit |
| Byte          |      8 bits |
| Kilobyte (KB) | 1,000 bytes |
| Megabyte (MB) |    1,000 KB |
| Gigabyte (GB) |    1,000 MB |
| Terabyte (TB) |    1,000 GB |

In computing, binary-based units are also used:

| Unit           |           Size |
| -------------- | -------------: |
| Kibibyte (KiB) | $2^{10}$ bytes |
| Mebibyte (MiB) | $2^{20}$ bytes |
| Gibibyte (GiB) | $2^{30}$ bytes |
| Tebibyte (TiB) | $2^{40}$ bytes |

**Important:** KB and KiB are not identical. KB uses 1,000 bytes, while KiB uses 1,024 bytes.

## 4. Bits vs. Bytes

The distinction between bits and bytes is important when discussing computer hardware and network speeds.

- Lowercase `b` usually represents bits.
- Uppercase `B` usually represents bytes.

For example:

$$
1\text{ MB}=8\text{ Mb}
$$

A network connection advertised as 100 Mbps means 100 megabits per second, not 100 megabytes per second.

Ignoring overhead and other limitations:

$$
100\text{ Mbps}\div8=12.5\text{ MB/s}
$$

## 5. Binary and Hexadecimal Representation

Bytes are often displayed in hexadecimal because hexadecimal is more compact than binary.

One byte contains 8 bits, which can be divided into two groups of 4 bits.

Example:

$$
10101111_2
$$

Divide into groups:

$$
1010\quad1111
$$

Convert each group into hexadecimal:

$$
A\quad F
$$

Therefore:

$$
10101111_2=AF_{16}
$$

One byte can therefore be represented using exactly two hexadecimal digits.

## 6. Applications

- Measuring computer memory and storage.
- Representing digital information.
- Measuring network transfer speeds.
- Representing characters and encoded data.
- Working with binary and hexadecimal values.

## 7. Related Concepts

- [[Binary]]
- [[Hexadecimal]]
- [[Number Systems]]
- [[Base Conversion]]
## Summary

A bit is a binary digit that can hold either $0$ or $1$.

A byte consists of 8 bits and can represent 256 different combinations.

Bits and bytes are the fundamental units used to represent and measure digital information.