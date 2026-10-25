---
title: 資料模型
tags: [規格, 資料]
status: 規格中
---
# 資料模型

要存四樣東西：店家、鄰居、包裹，以及為包裹發出的訊息。

```mermaid
erDiagram
    SHOP ||--o{ PARCEL : 收存
    NEIGHBOUR |o--o{ PARCEL : 收件人
    PARCEL ||--o{ MESSAGE : 觸發
    PARCEL {
        string id
        string recipient_name
        string shelf
        string pickup_code
        string status
        datetime arrived_at
        datetime collected_at
    }
    NEIGHBOUR {
        string id
        string name
        string contact
    }
    MESSAGE {
        string id
        string channel
        datetime sent_at
    }
```

## 欄位說明

- `status` 是 *waiting*、*collected* 或 *returned* 其中一種。
- `pickup_code` 是六位數字，在同一家店的等待中包裹裡不重複。
- 鄰居是選填。老闆可以替一個沒人註冊過的名字登記包裹。

這些欄位怎麼變化，見[取件流程](spec-pickup-flow.md)。

*這是 [MyGitNotes](https://mygitnotes.com/zh-tw) 的範例筆記本。[這個範例在示範什麼](https://mygitnotes.com/zh-tw/use-cases/project)。*
