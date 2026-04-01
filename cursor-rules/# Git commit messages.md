---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Git認可訊息

一律套用此規則。 當您草稿或產生Git認可訊息時（例如在Source的「控制項」認可方塊中，或在Agent聊天中詢問時），請遵循此格式。

## 主旨列（僅第一行）

- 大約&#x200B;**50個字元或更少**。
- 總結&#x200B;**命令式情境**&#x200B;中的變更（例如「新增……」、「修正……」、「重構……」）。

## 空白行

在主旨後面於內文前保留一行&#x200B;**空白行**。

## 內文（詳細說明）

- 以大約&#x200B;**72個字元**&#x200B;換行（包括專案符號首碼和空格）。
- 使用&#x200B;**專案符號行**&#x200B;來取得說明。 每個專案符號都必須以下列任一專案開頭：
   - **📖** — 當變更&#x200B;**新增**&#x200B;新內容時使用：新檔案、新區段、新功能、新標題、全新行或其他新欄位內容。
   - **✏️** — 當變更&#x200B;**修改**&#x200B;現有工作時使用：編輯現有行、更新現有區段、重構現有程式碼，或變更目前內容。

將&#x200B;**📖**&#x200B;或&#x200B;**✏️**&#x200B;套用至每個內文專案符號，以清楚顯示匯入的內容與變更的內容。

## 範本

填入預留位置（請勿在最終訊息中保留角括弧）：

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## 範例

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
