---
title: Independence
tags: [card, linear-algebra]
status: learning
---
# Independence

When are $\mathbf{v}_1, \dots, \mathbf{v}_k$ linearly independent?

---

When the only way to write $\mathbf{0}$ as a combination is the trivial one:

$$
c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k = \mathbf{0} \implies c_1 = \dots = c_k = 0.
$$

Equivalently: no vector in the list lies in the [span](card-span.md) of the others.

---

## Example

$(1,0)$, $(0,1)$ are independent. $(1,1)$, $(2,2)$ are not, because $2\cdot(1,1) - (2,2) = \mathbf{0}$.

Independent vectors that also span give a [Basis](card-basis.md).

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/study).*
