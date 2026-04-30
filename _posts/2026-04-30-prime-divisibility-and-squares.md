---

layout: post
title: "Prime Divisibility and Squares"
date: 2026-04-30 00:00:00 +0000
tags: [number-theory, primes, proofs, mathematics]
---

## Theorem

If ( p ) is prime and

[
p \mid n^2,
]

then

[
p \mid n.
]

---

## Proof

Assume ( p \mid n^2 ). Since

[
n^2 = n \cdot n,
]

we have

[
p \mid n \cdot n.
]

By the prime divisibility rule:

[
p \mid ab \implies p \mid a \text{ or } p \mid b.
]

Apply this with ( a = n ) and ( b = n ). Then

[
p \mid n \quad \text{or} \quad p \mid n.
]

So simply,

[
p \mid n.
]

---

## Conclusion

[
p \mid n^2 \implies p \mid n
]

for every prime ( p ).

---

## Intuition

A prime factor cannot appear “halfway” inside a square.

If ( p ) divides ( n^2 ), then ( p ) must already divide ( n ).

For example:

[
3 \mid 12^2 = 144,
]

and indeed,

[
3 \mid 12.
]

This fact is a key ingredient in many irrationality proofs, including proofs that ( \sqrt{p} ) is irrational for prime ( p ).
