---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

**workfront.en**存放庫的代理程式指引（Adobe Workfront英文）
檔案)。 此檔案指向規範指示，因此任何代理程式 — 
無論讀取哪個慣例檔案，都會遵循相同的規則。

## 標準指令檔案

- **全存放庫規則**： [.github/copilot-instructions.md](.github/copilot-instructions.md)
 — 候選文章搜尋、在編輯前建議、認可訊息和PR格式
和「聰明地填補空白」。
- **寫入標準** （自動套用至`help/**/*.md`）：
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md)，
提供完整詳細資訊，請參見
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md)。
- **發行說明** （自動套用至`product-announcements/product-releases/**`）：
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md)。
- **預覽反白清除** （隨選工作流程）：
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md)。

## 不可協商的行為

1. **建立新文章之前先尋找候選文章。** 當新內容出現時
在中，搜尋`help/`並顯示可能適合的現有文章的排名清單，
然後在起草之前詢問其所屬位置。
2. 在編輯任何說明`.md`文章之前，**提出變更。** 顯示提議的
比較並等待明確核准。 唯一的例外是我說「只要修復」
或是「不要詢問，只要編輯」。 唯讀研究與聊天中
工程圖永遠都可以。
3. **以智慧方式填滿空隙。** 當目的明確時，提交至
最佳實務解答並比對相關文章的標題，
術語和結構而非簡報選項功能表。
4. **在每`help/`次編輯時主動套用寫入標準** — 不要等待
以提醒您。

## 認可和PR慣例

如需完整資訊，請參閱[.github/copilot-instructions.md](.github/copilot-instructions.md)
認可訊息格式(必要主旨≤~50個字元；新增為📖，新增為✏️
修改)和PR結構(來自分支名稱的Jira ID；`# Summary`，
`# Changes`依檔案，`# Context` → `## Jira`)。
