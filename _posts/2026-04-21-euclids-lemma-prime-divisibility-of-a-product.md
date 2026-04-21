---

layout: post
title: "Euclid's Lemma: Prime Divisibility of a Product"
date: 2026-04-21 00:00:00 +0000
tags: [number-theory, primes, divisibility, proofs, mathematics]
---

# Theorem

If a prime number *p* divides a product *ab*, then *p* divides *a* or *p* divides *b*.

In symbols:

$$
p \mid ab \Longrightarrow p \mid a \text{ or } p \mid b.
$$

This is one of the basic facts that makes primes so important.

---

# Definitions

* $p \mid n$ means “$p$ divides $n$,” i.e. $n = pk$ for some integer $k$.
* A **prime** is an integer greater than 1 whose only positive divisors are 1 and itself.

---

# Proof

Assume

$$
p \mid ab.
$$

We want to prove that $p \mid a$ or $p \mid b$.

Now suppose $p \nmid a$. We will show that this forces $p \mid b$.

Since $p$ is prime, the only positive common divisors of $p$ and $a$ can be 1 or $p$. But $p \nmid a$, so they cannot share the divisor $p$. Therefore,

$$
\gcd(p, a) = 1.
$$

So $p$ and $a$ are coprime.

A standard fact says that if $\gcd(p, a) = 1$, then there exist integers $x, y$ such that

$$
px + ay = 1.
$$

This is Bézout's identity.

Now multiply both sides by $b$:

$$
pbx + aby = b.
$$

Look at the two terms on the left:

* $pbx$ is divisible by $p$.
* $aby$ is divisible by $p$ because $p \mid ab$.

So the sum

$$
pbx + aby
$$

is divisible by $p$.

But this sum equals $b$. Hence

$$
p \mid b.
$$

So if $p \nmid a$, then $p \mid b$. Therefore,

$$
p \mid a \text{ or } p \mid b.
$$

---

# Conclusion

$$
p \mid ab \Longrightarrow p \mid a \text{ or } p \mid b
$$

whenever $p$ is prime.

---

# Intuition

A prime cannot “hide” across two factors.

If a composite number divides a product, it might be built partly from one factor and partly from the other. For example,

$$
6 \mid (2 \cdot 3),
$$

but $6 \nmid 2$ and $6 \nmid 3$.

Primes are different: they are indivisible in a strong enough way that if they appear in a product, they must already appear in at least one factor.
