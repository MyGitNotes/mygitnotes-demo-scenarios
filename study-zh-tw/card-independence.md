---
title: 線性獨立
tags: [卡片, linear-algebra]
status: 學習中
---
# 線性獨立

$\mathbf{v}_1, \dots, \mathbf{v}_k$ 什麼時候線性獨立？

---

當把 $\mathbf{0}$ 寫成線性組合的方法只有全部係數為零這一種時：

$$
c_1\mathbf{v}_1 + \dots + c_k\mathbf{v}_k = \mathbf{0} \implies c_1 = \dots = c_k = 0.
$$

也就是說，這串向量裡沒有任何一個落在其他向量的[生成空間](card-span.md)裡。

---

## 例子

$(1,0)$、$(0,1)$ 線性獨立；$(1,1)$、$(2,2)$ 不獨立，因為 $2\cdot(1,1) - (2,2) = \mathbf{0}$。

又獨立、又能生成整個空間的向量，就是[基底](card-basis.md)。

*這是 [MyGitNotes](https://mygitnotes.com/zh-tw) 的範例筆記本。[這個範例在示範什麼](https://mygitnotes.com/zh-tw/use-cases/study)。*
