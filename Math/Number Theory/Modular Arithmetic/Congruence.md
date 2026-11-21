**Congruence** is a mathematical relationship between two integers that have the same remainder when divided by a particular positive integer.

It is one of the fundamental concepts of [[Modular Arithmetic]] and [[Number Theory]].

## 1. Definition of Congruence

Two integers $a$ and $b$ are said to be congruent modulo $n$ if they have the same remainder when divided by $n$.

The notation is:

$$
a\equiv b\pmod n
$$

This is read as:

"$a$ is congruent to $b$ modulo $n$."

### Example

Consider the numbers $17$ and $5$.

Divide both by $12$:

$$
17\bmod12=5
$$

$$
5\bmod12=5
$$

Both numbers have the same remainder.

Therefore:

$$
17\equiv5\pmod{12}
$$

## 2. Mathematical Definition

Two integers $a$ and $b$ are congruent modulo $n$ if and only if $n$ divides their difference.

$$
a\equiv b\pmod n
$$

If and only if:

$$
n\mid(a-b)
$$

The symbol $\mid$ means "divides."

This means that there exists an integer $k$ such that:

$$
a-b=kn
$$

### Example

Determine whether $23$ and $8$ are congruent modulo $5$.

Calculate their difference:

$$
23-8=15
$$

Since:

$$
15=3\times5
$$

The difference is divisible by $5$.

Therefore:

$$
23\equiv8\pmod5
$$

## 3. Congruence and Remainders

Congruence is directly related to the [[Modulo Operation]].

The following statements are equivalent:

$$
a\equiv b\pmod n
$$

$$
a\bmod n=b\bmod n
$$

$$
n\mid(a-b)
$$

All three express the same mathematical relationship.

### Example

Consider:

$$
26\equiv11\pmod5
$$

Check the remainders:

$$
26\bmod5=1
$$

$$
11\bmod5=1
$$

Both remainders are equal, so the numbers are congruent.

## 4. Properties of Congruence

Congruence modulo $n$ has several important properties.

### 4.1 Reflexive Property

Every integer is congruent to itself.

$$
a\equiv a\pmod n
$$

Example:

$$
7\equiv7\pmod3
$$

### 4.2 Symmetric Property

If $a$ is congruent to $b$, then $b$ is also congruent to $a$.

$$
a\equiv b\pmod n
$$

Implies:

$$
b\equiv a\pmod n
$$

Example:

$$
17\equiv5\pmod{12}
$$

Therefore:

$$
5\equiv17\pmod{12}
$$

### 4.3 Transitive Property

If $a$ is congruent to $b$, and $b$ is congruent to $c$, then $a$ is congruent to $c$.

$$
a\equiv b\pmod n
$$

$$
b\equiv c\pmod n
$$

Therefore:

$$
a\equiv c\pmod n
$$

### 4.4 Addition Property

If two congruences have the same modulus, they can be added.

If:

$$
a\equiv b\pmod n
$$

And:

$$
c\equiv d\pmod n
$$

Then:

$$
a+c\equiv b+d\pmod n
$$

### Example

$$
8\equiv3\pmod5
$$

$$
7\equiv2\pmod5
$$

Adding both sides:

$$
8+7\equiv3+2\pmod5
$$

$$
15\equiv5\pmod5
$$

### 4.5 Subtraction Property

Congruences can also be subtracted.

$$
a-c\equiv b-d\pmod n
$$

### 4.6 Multiplication Property

Congruences can be multiplied.

If:

$$
a\equiv b\pmod n
$$

And:

$$
c\equiv d\pmod n
$$

Then:

$$
ac\equiv bd\pmod n
$$

### Example

$$
7\equiv2\pmod5
$$

Multiply both sides by themselves:

$$
7^2\equiv2^2\pmod5
$$

$$
49\equiv4\pmod5
$$

This works because:

$$
49\bmod5=4
$$

## 5. Congruence Classes

All integers that have the same remainder when divided by $n$ belong to the same congruence class modulo $n$.

For example, modulo $5$, the integers can be grouped into five classes:

- Remainder 0: $\{\ldots,-10,-5,0,5,10,15,\ldots\}$
- Remainder 1: $\{\ldots,-9,-4,1,6,11,16,\ldots\}$
- Remainder 2: $\{\ldots,-8,-3,2,7,12,17,\ldots\}$
- Remainder 3: $\{\ldots,-7,-2,3,8,13,18,\ldots\}$
- Remainder 4: $\{\ldots,-6,-1,4,9,14,19,\ldots\}$

These are called residue classes modulo $5$.

The set of all residue classes modulo $n$ is commonly denoted by:

$$
\mathbb{Z}/n\mathbb{Z}
$$

This is also called the integers modulo $n$.

## 6. Applications of Congruence

### Clock Arithmetic

A 12-hour clock operates using congruence modulo $12$.

For example, 15 hours and 3 hours correspond to the same clock position:

$$
15\equiv3\pmod{12}
$$

### Modular Arithmetic

Congruence allows us to simplify calculations by replacing numbers with other numbers from the same congruence class.

For example:

$$
27+18\equiv2+3\pmod5
$$

$$
45\equiv5\pmod5
$$

### Divisibility

Two integers are congruent modulo $n$ when their difference is divisible by $n$.

This makes congruence useful for studying divisibility patterns.

See [[Divisibility]].

## 7. Important Distinction

Congruence and equality are not the same thing.

For example:

$$
17\equiv5\pmod{12}
$$

This does not mean:

$$
17=5
$$

It means that both numbers belong to the same congruence class modulo $12$.

Their numerical values are different, but their remainders are equal.

## 8. Related Concepts

- [[Number Theory]]
- [[Remainders]]
- [[Modular Arithmetic]]
- [[Divisibility]]
- [[Greatest Common Divisor]]

## Summary

Congruence describes a relationship between integers that have the same remainder when divided by a positive integer.

Its notation is:

$$
a\equiv b\pmod n
$$

Its equivalent divisibility condition is:

$$
n\mid(a-b)
$$

Congruence is fundamental to modular arithmetic and provides useful rules for simplifying mathematical calculations.