---
title: 課堂筆記：第 1 到 3 週
tags: [課堂]
status: 已熟悉
---
# 課堂筆記：第 1 到 3 週

符號：向量用粗體，$\mathbb{R}^n$ 是所有由 $n$ 個實數排成的數列所成的集合。

## 第 1 週：向量與線性組合

$\mathbb{R}^n$ 裡的[向量](card-vector.md)是一串有順序的數 $\mathbf{v} = (v_1, \dots, v_n)$。兩個向量可以相加，也可以乘上一個數 $c$：

$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1, \dots, u_n + v_n), \qquad c\,\mathbf{v} = (c v_1, \dots, c v_n).
$$

$\mathbf{v}_1, \dots, \mathbf{v}_k$ 的*線性組合*，就是任何形如 $c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k$ 的向量。所有線性組合的集合叫[生成空間](card-span.md)。

## 第 2 週：獨立與基底

當下面這個條件成立時，這些向量[線性獨立](card-independence.md)：

$$
c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k = \mathbf{0} \implies c_1 = \dots = c_k = 0.
$$

[基底](card-basis.md)是一組線性獨立、又能生成整個空間的向量。$\mathbb{R}^n$ 的每組基底都剛好有 $n$ 個向量，所以 $\dim \mathbb{R}^n = n$。

## 第 3 週：線性映射與特徵向量

函數 $T$ 滿足 $T(a\mathbf{u} + b\mathbf{v}) = aT(\mathbf{u}) + bT(\mathbf{v})$，就是[線性映射](card-linear-map.md)。取定座標後，它就是乘上一個矩陣 $A$，矩陣的各行是基底向量被映射之後的結果。

對方陣 $A$，若有非零向量 $\mathbf{v}$ 使 $A\mathbf{v} = \lambda\mathbf{v}$，$\mathbf{v}$ 就是[特徵向量](card-eigenvalue.md)，$\lambda$ 是對應的特徵值。解下面這個方程式就能找到它們：

$$
\det(A - \lambda I) = 0.
$$

## 例題

取 $A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$，得到 $\det(A - \lambda I) = (2-\lambda)^2 - 1 = (\lambda - 1)(\lambda - 3)$，所以特徵值是 $1$ 和 $3$，對應的特徵向量是 $(1,-1)$ 和 $(1,1)$。

同一個多項式畫成圖：曲線穿過 0 的地方，就是特徵值。

::::line{title="A 的特徵多項式" subtitle="det(A − λI) = (2 − λ)² − 1" ticks="0,1,2,3,4" note="橫軸是 λ。"}
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

*這是 [MyGitNotes](https://mygitnotes.com/zh-tw) 的範例筆記本。[這個範例在示範什麼](https://mygitnotes.com/zh-tw/use-cases/study)。*
