---
title: 生成空間
tags: [卡片, linear-algebra]
status: 複習中
---
# 生成空間

$\operatorname{span}\{\mathbf{v}_1, \dots, \mathbf{v}_k\}$ 是什麼意思？

---

這些向量所有**線性組合**的集合：

$$
\operatorname{span}\{\mathbf{v}_1, \dots, \mathbf{v}_k\} = \{\, c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k : c_i \in \mathbb{R} \,\}.
$$

例：$\operatorname{span}\{(1,0),(0,1)\} = \mathbb{R}^2$，但 $\operatorname{span}\{(1,1)\}$ 只是直線 $y = x$。

依據[向量](card-vector.md)。「有沒有向量是多餘的？」這個問題通往[線性獨立](card-independence.md)。
