---

layout: post
title: "Infinitely Many Prime Numbers"
date: 2026-04-18 00:00:00 +0003
tags: [mathematics, number-theory, primes, proofs]
---

## Theorem

There are infinitely many prime numbers.

---

## Definitions

A **prime number** is an integer greater than 1 whose only positive divisors are 1 and itself.

---

## Proof

We will again use **contradiction**.

Assume there are only finitely many primes. List them all:

$$
p_1, p_2, p_3, \ldots, p_n
$$

Now form the number:

$$
N = p_1 p_2 p_3 \cdots p_n + 1
$$

So $N$ is one more than the product of all supposed prime numbers.

Now ask: is $N$ divisible by any of the primes in our list?

Take any $p_i$. Since $p_i$ divides the product

$$
p_1 p_2 \cdots p_n,
$$

if $p_i$ also divided $N$, then $p_i$ would divide the difference:

$$
N - p_1 p_2 \cdots p_n = 1
$$

But no prime divides 1.

So **none** of the primes $p_1, \ldots, p_n$ divides $N$.

That means one of two things must happen:

* either $N$ itself is prime, or
* $N$ is composite, in which case it has a prime factor.

In either case, there exists a prime dividing $N$. But that prime is **not** in our list, since none of $p_1, \ldots, p_n$ divides $N$.

This contradicts the assumption that $p_1, \ldots, p_n$ were all the primes.

---

## Conclusion

Therefore, there are **infinitely many prime numbers**.
