---

layout: post
title: "If n² is Even, Then n is Even"
date: 2026-04-24 00:00:00 +0000
tags: [mathematics, number-theory, proofs, logic]
---

## Theorem

If $n^2$ is even, then $n$ is even.

---

## Why This Is Interesting

This is the **stronger converse** of a previous idea: not only do even numbers square to even numbers, but *only* even numbers can do that.

---

## Proof

We prove this using **contradiction**.

Assume that $n^2$ is even, but $n$ is odd.

Since $n$ is odd, we can write:

$$
n = 2k + 1
$$

for some integer $k$.

Now square $n$:

$$
n^2 = (2k + 1)^2 = 4k^2 + 4k + 1.
$$

Factor:

$$
n^2 = 2(2k^2 + 2k) + 1.
$$

This shows that $n^2$ is **odd**.

---

## Contradiction

We assumed:

* $n^2$ is even
* but we just showed $n^2$ is odd

This is impossible.

---

## Conclusion

Therefore, our assumption was wrong, and $n$ must be even.

$$
n^2 \text{ even} \Rightarrow n \text{ even}
$$

---

## Intuition

Odd numbers “stay odd” when squared. So if a square somehow turns out even, the original number couldn’t have been odd — it must have been even.

---

## Quick Example

* $6^2 = 36$ — even, came from even
* $5^2 = 25$ — odd, never produces even

There’s no way to square an odd number and get an even result.
