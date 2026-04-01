---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# 提取請求(PR)

起草或檢閱提取要求標題或說明時（例如在GitHub/GitLab中，或在Agent聊天中詢問時），請遵循下列慣例。

## 衍生Jira問題

- **真實的Source：**&#x200B;從&#x200B;**目前的Git分支名稱**&#x200B;衍生Jira問題ID （例如符合專案金鑰模式的區段，例如`FFENT-8796`）。
- **如果分支名稱包含Jira ID：**&#x200B;請在PR標題中使用該ID （請參閱下文），並在`# Context`→`## Jira`中將其連結。
- **如果分支名稱不包含Jira ID：**&#x200B;請將PR視為與票證無關。 **省略** PR標題中的Jira金鑰（不要發明票證）。 仍包含`# Context`→`## Jira`，內容剛好是： `No ticket` （無連結）。

## PR標題

**當分支名稱包含Jira問題識別碼**&#x200B;時，包含&#x200B;**both**：

1. **Jira問題識別碼** （例如`FFENT-8001`）。
2. **認可型別** （請參閱下列清單），使用此模式：

`{type}/{JIRA-ID}- {short task description}`

範例：

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

在ID後面使用簡潔的命令式描述。 比對顯示的間距模式：文字、斜線、Jira鍵與尾端連字型大小、空格，然後是說明。

**當分支名稱不包含Jira問題ID**&#x200B;時，請從標題中省略票證並使用：

`{type}- {short task description}`

範例：

`docs- Refresh Object Composite API changelog`

### 可接受的認可型別（在`/`之前剛好使用這些標籤）

- **feat** — 新增一項功能。 當加入新的TOC專案或JIRA連線到另一個`feat` — 標示為Jira時。
- **修正** — 修正錯誤
- **重新調整** — 重新寫入/重新建構程式碼而不變更行為
- **perf** — 改善效能（特殊重構）
- **style** — 僅格式設定/空白字元；無意義。 僅編輯
- **測試** — 新增或修正測試
- **檔案** — 已新增內容。 僅檔案
- **組建** — 組建工具、CI、相依性、專案版本等。
- **ops** — 基礎架構、部署、備份、復原等。
- **雜項** — 雜項（例如`.gitignore`）

## PR內文 — 必要區段

請一律使用&#x200B;**這些最上層區段** （Markdown標題）：

### 1. `# Summary`

**變更內容**&#x200B;和&#x200B;**原因**&#x200B;的簡短概觀（商業或技術意圖）。

### 2. `# Changes`

依&#x200B;**檔案**&#x200B;組織。 對於每個接觸的檔案，使用帶有反引號中路徑的層級2標題，然後使用描述編輯的專案符號。

格式：

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

一律在&#x200B;**下包含** Jira`# Context`子區段。

**當分支名稱包含Jira ID時：**&#x200B;使用問題的可點按連結（從分支名稱衍生索引鍵）。

格式：

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

將金鑰和URL取代為實際票證。 如果套用多個票證，請在相同子區段中將其逐行列出。

**當分支名稱不包含Jira ID時：**&#x200B;保留`## Jira`並完全使用：

```markdown
# Context

## Jira
No ticket
```

## 範例（完整PR說明）

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## 範例（完整PR說明，不含Jira ID的分支）

**標題：** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
