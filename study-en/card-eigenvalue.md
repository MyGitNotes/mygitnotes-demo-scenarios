---
title: Eigenvalues
tags: [card, linear-algebra]
status: new
---
# Eigenvalues

What do $A\mathbf{v} = \lambda\mathbf{v}$ and $\det(A - \lambda I) = 0$ say?

---

A nonzero $\mathbf{v}$ is an **eigenvector** of $A$ when $A\mathbf{v}$ lies on the line through $\mathbf{v}$: $A\mathbf{v} = \lambda\mathbf{v}$. The number $\lambda$ is the **eigenvalue**.

Nonzero solutions exist exactly when $A - \lambda I$ is not invertible:

$$
\det(A - \lambda I) = 0.
$$

---

## Example

$A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$ has eigenvalues $3$ (eigenvector $(1,1)$) and $1$ (eigenvector $(1,-1)$).

Eigenvectors are the directions a [linear map](card-linear-map.md) does not turn (it may stretch or flip them). Back to the start: [Vectors](card-vector.md).
