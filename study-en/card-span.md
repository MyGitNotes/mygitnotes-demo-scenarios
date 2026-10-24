---
title: Span
tags: [card, linear-algebra]
status: review
---
# Span

What does $\operatorname{span}\{\mathbf{v}_1, \dots, \mathbf{v}_k\}$ mean?

---

The set of every **linear combination** of the vectors:

$$
\operatorname{span}\{\mathbf{v}_1, \dots, \mathbf{v}_k\} = \{\, c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k : c_i \in \mathbb{R} \,\}.
$$

Example: $\operatorname{span}\{(1,0),(0,1)\} = \mathbb{R}^2$, but $\operatorname{span}\{(1,1)\}$ is only the line $y = x$.

Builds on [Vectors](card-vector.md). The question "is anything wasted?" leads to [Independence](card-independence.md).
