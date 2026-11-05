---
description: Adobe Workfront發行說明（概觀、產品區域、計畫和外觀頁面）的格式化和驗證規則。
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# 發行說明格式化程式

這些檔案是&#x200B;**發行說明**，而非作法文章。 請&#x200B;**不**套用
一般撰寫品質標準。 編輯之前，請先閱讀以下專案的完整來源：
truth，其中包含範本和發行行事曆：

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## 重要規則 — 先決定檔案季度

> [!IMPORTANT]
> 絕對不要在其上使用calendar-quarter math將功能指派給doc-quarter
> 預覽或生產日期。 Doc-quarter是以哪個&#x200B;**月發行為準**
> 根據Workfront的內部發行 — 行事曆分組，此功能出貨於
> 是從日曆季度位移。 例如，具有生產環境的功能
> 2026年8月13日的日期屬於doc-quarter `26-q4`，而非`26-q3`。 永遠
> 仔細檢查之前參考檔案中的2026年發行行事曆表格
> 建立或編輯任何檔案。 如果生產日期在該表格之外，
> 要求更新行事曆，而非猜測。

## 主要結構規則

- **Frontmatter**： `feature`必須剛好`Product Announcements`；
  `recommendations`必須剛好`noDisplay, noCatalog`。 絕不發明
  `exl-id` — 僅在其已存在時才包含它。
- **最新功能在前**：最新的發行說明是之後的第一個H2
介紹（產品區域頁面）和每個功能表格的頂列（概觀）
頁面)。
- **總覽連結**：產品區域頁面必須連結至&#x200B;**自己的季度**
概述檔案 — 常見錯誤為連結至上一季。
- **日期圖說文字**：每個功能H2後面都有一個`>[!NOTE]`區塊，其中
預覽/生產快速發佈/生產適用於每個日期，符合
概觀表格列。 將日期格式設為`Month Day, Year`；若不明，請使用`TBD`。
- 以H1代字元&#x200B;**撰寫季度名稱**：「第一季」、「第二季」、「第三季」
季」、「第四季」。

## 新增頁面時所需的隨附更新

- **新頁面（任何）**：在同一變更中將它新增到`help/quicksilver/TOC.md`
（概覽優先，產品區域頁面按字母順序排列，其他增強功能優先）。
- **新季的概觀頁面**：同時更新`help/quicksilver/home.md` —
重新整理「最新版本」索引標籤連結和Planning活動連結，然後新增
「本年度版本」標籤的新季度。

如需完整的範本，請參閱上述SKILL.md和reference.md檔案，
檔案命名慣例、連結格式及完整發行行事曆。
