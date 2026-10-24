---
title: Lecture notes, weeks 1 to 3
tags: [lecture]
status: known
---
# Lecture notes, weeks 1 to 3

Notation: vectors are bold, $\mathbb{R}^n$ is the set of all lists of $n$ real numbers.

## Week 1: vectors and combinations

A [vector](card-vector.md) in $\mathbb{R}^n$ is an ordered list $\mathbf{v} = (v_1, \dots, v_n)$. We can add two vectors and scale one by a number $c$:

$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1, \dots, u_n + v_n), \qquad c\,\mathbf{v} = (c v_1, \dots, c v_n).
$$

A *linear combination* of $\mathbf{v}_1, \dots, \mathbf{v}_k$ is any vector $c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k$. The set of all of them is the [span](card-span.md).

## Week 2: independence and bases

The vectors are [linearly independent](card-independence.md) when

$$
c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k = \mathbf{0} \implies c_1 = \dots = c_k = 0.
$$

A [basis](card-basis.md) is an independent list that spans the space. Every basis of $\mathbb{R}^n$ has exactly $n$ vectors, so $\dim \mathbb{R}^n = n$.

## Week 3: linear maps and eigenvectors

A function $T$ is a [linear map](card-linear-map.md) when $T(a\mathbf{u} + b\mathbf{v}) = aT(\mathbf{u}) + bT(\mathbf{v})$. In coordinates it is multiplication by a matrix $A$, whose columns are the images of the basis vectors.

For a square matrix $A$, a nonzero $\mathbf{v}$ with $A\mathbf{v} = \lambda\mathbf{v}$ is an [eigenvector](card-eigenvalue.md), and $\lambda$ is its eigenvalue. We find them by solving

$$
\det(A - \lambda I) = 0.
$$

## Worked example

For $A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$ we get $\det(A - \lambda I) = (2-\lambda)^2 - 1 = (\lambda - 1)(\lambda - 3)$, so the eigenvalues are $1$ and $3$, with eigenvectors $(1,-1)$ and $(1,1)$.

The same polynomial as a picture: the eigenvalues are where the curve crosses zero.

::::line{title="The characteristic polynomial of A" subtitle="det(A − λI) = (2 − λ)² − 1" ticks="0,1,2,3,4" note="The horizontal axis is λ."}
:::series{title="det(A − λI)" highlight}
- 0｜3
- 0.5｜1.25
- 1｜0｜λ = 1
- 1.5｜-0.75
- 2｜-1
- 2.5｜-0.75
- 3｜0｜λ = 3
- 3.5｜1.25
- 4｜3
:::
::::
