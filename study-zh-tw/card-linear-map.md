---
title: 線性映射
tags: [卡片, linear-algebra]
status: 新卡片
---
# 線性映射

函數 $T$ 要滿足什麼才算線性映射？它怎麼寫成矩陣？

---

對所有向量和數字，都有 $T(a\mathbf{u} + b\mathbf{v}) = aT(\mathbf{u}) + bT(\mathbf{v})$，$T$ 就是線性的。

取定一組[基底](card-basis.md)之後，$T$ 就是乘上一個矩陣 $A$。**$A$ 的各行，就是基底向量經過 $T$ 之後的像。**

---

## 例子

把平面逆時針旋轉 90°：$T(1,0) = (0,1)$，$T(0,1) = (-1,0)$，所以

$$
A = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}.
$$

這個旋轉會轉動每個非零向量。很多別的映射卻有些方向不轉、只被拉長或縮短：那些向量是特徵向量，倍數就是[特徵值](card-eigenvalue.md)。
