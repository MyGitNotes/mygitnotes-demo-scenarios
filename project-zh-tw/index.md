---
title: 歡迎：產品規格
tags: [導覽]
status: 已上線
---
# 貨架小幫手：產品規格

「貨架小幫手」是給社區雜貨店用的 App。店家常替街坊代收包裹，這個程式讓老闆登記一個包裹，通知收件的鄰居，再用一組取件碼把包裹交出去。這裡的內容都是虛構的範例。

## 可以試試

1. **從規格檢視開始。** 筆記本一打開就是「規格檢視」這個 Focus：[產品概述](product-overview.md)旁邊是[取件流程](spec-pickup-flow.md)的流程圖，[資料模型](data-model.md)和[通知](spec-notifications.md)在同一格的分頁。「筆記」頁工具列的 Focus 選單可以切回一般清單。
2. **切到看板檢視。** 筆記是四欄裡的卡片：*待排*、*規格中*、*開發中*、*已上線*。把卡片拖到另一欄，或用圓點改狀態，檔案裡的狀態也跟著改。
3. **看圖表。** [取件流程](spec-pickup-flow.md)、[通知](spec-notifications.md)和[資料模型](data-model.md)各有一張用文字寫成的圖。用原始碼模式打開，改一行就會看到圖重畫。
4. **請助理改筆記。** [和 AI 助理一起工作](ai-assistant.md)說明助理怎麼直接讀、改這些筆記，改完你會看到什麼。
5. **掃一眼狀態板。** 在「筆記對照」下面，`status-board` 把筆記按進度分組，每一項都連到它的筆記。
6. **隨便改。** 這是示範用的副本，你的修改只留在這個瀏覽器 24 小時，不會影響任何人。

## 筆記對照

::::status-board{title="每篇筆記進行到哪"}
:::group{status="done" title="已上線"}
- [產品概述](product-overview.md)｜問題、想法和第一版做了什麼
- [和 AI 助理一起工作](ai-assistant.md)｜助理怎麼直接改這些筆記
:::
:::group{status="partial" title="開發中"}
- [通知](spec-notifications.md)｜四項驗收條件，完成兩項
:::
:::group{status="partial" title="規格中"}
- [取件流程](spec-pickup-flow.md)｜還有三個待釐清的問題
- [資料模型](data-model.md)｜要存的四樣東西
:::
:::group{status="none" title="待排"}
- [條碼掃描](spec-barcode-scan.md)｜開始規格前要先回答的問題
- [退貨](spec-returns.md)｜開始規格前要先回答的問題
:::
::::

*這是 [MyGitNotes](https://mygitnotes.com/zh-tw) 的範例筆記本。[這個範例在示範什麼](https://mygitnotes.com/zh-tw/use-cases/project)。*
