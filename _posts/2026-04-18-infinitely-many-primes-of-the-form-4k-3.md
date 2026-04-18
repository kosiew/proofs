---

layout: post
title: "Infinitely Many Primes of the Form 4k + 3"
date: 2026-04-18 10:00:00 +0002
tags: [number-theory, primes, modular-arithmetic, proofs]
---

## Theorem

There are infinitely many primes of the form

$$
4k + 3
$$

that is, primes congruent to $3 \pmod{4}$.

---

## What this means

A number is of the form $4k + 3$ if it leaves remainder 3 when divided by 4:

$$
3, 7, 11, 15, 19, \ldots
$$

Among these, the primes include:

$$
3, 7, 11, 19, 23, 31, \ldots
$$

We will prove there are infinitely many such primes.

---

## Proof

We again use **contradiction**.

Assume there are only finitely many primes congruent to $3 \pmod{4}$. List them:

$$
p_1, p_2, \ldots, p_n
$$

where each $p_i \equiv 3 \pmod{4}$.

Now build the number:

$$
N = 4p_1 p_2 \cdots p_n - 1
$$

We will show this leads to a contradiction.

---

### Step 1: $N \equiv 3 \pmod{4}$

Since $4p_1 p_2 \cdots p_n$ is divisible by 4,

$$
4p_1 p_2 \cdots p_n \equiv 0 \pmod{4}
$$

So

$$
N = 4p_1 p_2 \cdots p_n - 1 \equiv -1 \equiv 3 \pmod{4}
$$

So $N$ is itself of the form $4k + 3$.

---

### Step 2: None of the listed primes divides $N$

Each $p_i$ divides the product $4p_1 p_2 \cdots p_n$. If some $p_i$ also divided $N$, then it would divide the difference

$$
(4p_1 p_2 \cdots p_n) - N = 1
$$

But no prime divides 1.

Therefore, none of

$$
p_1, p_2, \ldots, p_n
$$

divides $N$.

---

### Step 3: $N$ must have a prime factor congruent to $3 \pmod{4}$

Since $N > 1$, it has at least one prime divisor; call one of them $q$.

Now we claim:

$$
q \equiv 3 \pmod{4}
$$

for at least one prime divisor $q$ of $N$.

Why must this be true?

Suppose instead that every prime divisor of $N$ were congruent to $1 \pmod{4}$ (we can ignore 2, since $N$ is odd). Then their product would also be congruent to $1 \pmod{4}$, because

$$
1 \cdot 1 \equiv 1 \pmod{4}
$$

So $N$ would be congruent to $1 \pmod{4}$.

But from Step 1, we know

$$
N \equiv 3 \pmod{4}
$$

Contradiction.

So at least one prime factor $q$ of $N$ satisfies

$$
q \equiv 3 \pmod{4}
$$

---

### Step 4: This gives a new $4k + 3$ prime

This prime $q$ divides $N$, but none of the primes

$$
p_1, \ldots, p_n
$$

divides $N$.

So $q$ is not in our list.

But $q$ is another prime congruent to $3 \pmod{4}$, contradicting the assumption that our list contained all such primes.

---

## Conclusion

Therefore, there are infinitely many primes of the form

$$
4k + 3
$$

> There are infinitely many primes $p$ with $p \equiv 3 \pmod{4}$.

---

## Intuition

This is Euclid’s proof with a twist.

For ordinary primes, we multiply all known primes and add 1.

Here, we want specifically primes of the form $4k + 3$, so we build

$$
4p_1 p_2 \cdots p_n - 1
$$

That guarantees the new number is $3 \pmod{4}$, and any prime factorization of such a number must include at least one prime that is also $3 \pmod{4}$.

So a new prime of the desired type is forced to appear.
