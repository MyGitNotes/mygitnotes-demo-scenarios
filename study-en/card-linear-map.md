---
title: Linear maps
tags: [card, linear-algebra]
status: new
---
# Linear maps

What makes a function $T$ a linear map, and how do we write it as a matrix?

---

$T$ is linear when $T(a\mathbf{u} + b\mathbf{v}) = aT(\mathbf{u}) + bT(\mathbf{v})$ for all vectors and numbers.

Once we fix a [basis](card-basis.md), $T$ is multiplication by a matrix $A$. **The columns of $A$ are the images of the basis vectors.**

---

## Example

Rotating the plane by 90° anticlockwise: $T(1,0) = (0,1)$ and $T(0,1) = (-1,0)$, so

$$
A = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}.
$$

This rotation turns every nonzero vector. Many other maps leave some directions alone and only stretch them: those vectors are eigenvectors, and the stretch factors are [Eigenvalues](card-eigenvalue.md).

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/study).*
