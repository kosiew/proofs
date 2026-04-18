---

layout: post
title: "Proof that √2 is Irrational"
date: 2026-04-17 10:00:01 +0000
tags: [mathematics, number-theory, proofs, irrational-numbers]
---

## Theorem

$\sqrt{2}$ is irrational (i.e., it cannot be written as a ratio of two integers).

---

## Proof

We proceed by **contradiction**.

Assume $\sqrt{2}$ is rational. Then we can write it as a reduced fraction:

$$
\sqrt{2} = \frac{a}{b}
$$

where $a, b$ are integers with no common factors (the fraction is in lowest terms), and $b \ne 0$.

Now square both sides:

$$
2 = \frac{a^2}{b^2}
$$

Multiply by $b^2$:

$$
2b^2 = a^2
$$

So $a^2$ is even, which implies $a$ is even (since only even numbers have even squares).

Let $a = 2k$ for some integer $k$. Substitute:

$$
2b^2 = (2k)^2 = 4k^2
$$

Divide by 2:

$$
b^2 = 2k^2
$$

This shows $b^2$ is even, so $b$ is also even.

---

## Contradiction

We’ve shown:

* $a$ is even
* $b$ is even

So both share a factor of 2 — contradicting our assumption that $\frac{a}{b}$ was in lowest terms.

---

## Conclusion

Our assumption must be false. Therefore,

$$
\sqrt{2} \text{ is irrational.}
$$
