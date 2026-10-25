---
title: 特徵值
tags: [卡片, linear-algebra]
status: 新卡片
---
# 特徵值

$A\mathbf{v} = \lambda\mathbf{v}$ 和 $\det(A - \lambda I) = 0$ 在說什麼？

---

非零向量 $\mathbf{v}$ 若使 $A\mathbf{v}$ 與 $\mathbf{v}$ 共線，即 $A\mathbf{v} = \lambda\mathbf{v}$，$\mathbf{v}$ 就是 $A$ 的**特徵向量**，$\lambda$ 是**特徵值**。

有非零解，當且僅當 $A - \lambda I$ 不可逆：

$$
\det(A - \lambda I) = 0.
$$

---

## 例子

$A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$ 的特徵值是 $3$（特徵向量 $(1,1)$）和 $1$（特徵向量 $(1,-1)$）。

特徵向量是[線性映射](card-linear-map.md)不會轉動的那些方向，只會被拉長、縮短或反向。回到起點：[向量](card-vector.md)。
