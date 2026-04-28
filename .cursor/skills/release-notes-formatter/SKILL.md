---
name: release-notes-formatter
description: 格式化及驗證Workfront發行說明，以取得一致性、正確結構和正確連結。 僅用於產品版本目錄中的版本注意事項檔案，或者當使用者提及版本注意事項、產品版本或季度版本時。 請勿套用至作法文章或一般檔案。
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---


# 發行說明格式化程式

格式化和驗證`help/quicksilver/product-announcements/product-releases/`目錄中的Adobe Workfront發行說明。

## 頁面型別

識別檔案路徑和內容的頁面型別：

| 頁面類型 | 檔案模式 | 範本 |
|-----------|-------------|----------|
| **概觀** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **產品區域** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **規劃** | `planning-release-activity-{YY}-q{N}.md` | 與產品區域相似 |
| **外觀** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## 格式化工作流程

### 步驟1：驗證Frontmatter

所有發行說明頁面的必填欄位：

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

規則：
- `feature`必須剛好`Product Announcements`
- `recommendations`必須剛好`noDisplay, noCatalog`
- 絕不建立`exl-id` — 僅包含已存在的專案
- 請勿將`draft: Probably`新增至實際頁面（僅限範本）

### 步驟2：依頁面型別驗證結構

#### 產品區域頁面

1. **H1**： `{Written Quarter} {Area} enhancements`
   - 範例：`# Second Quarter 2026 Administrator enhancements`
   - 季必須寫成：「第一季」、「第二季」、「第三季」、「第四季」

2. **簡介段落**：說明概觀的區域和連結
   - 必須連結至&#x200B;**正確季的**&#x200B;概觀檔案
   - 常見錯誤：連結至上一季（例如`26-q1`而非`26-q2`）

3. **H2每個功能**：功能標題做為標題
   - **最新功能在前** — 最新的發行說明必須顯示為介紹段落之後的第一個H2
   - 較舊的功能會以反向時間順序遵循

4. 每個H2之後的&#x200B;**日期圖說文字區塊**：

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **內文**：功能說明，然後連結到說明檔案

#### 總覽頁面

1. **H1**： `{Written Quarter} release overview`

2. **將段落**&#x200B;與排定的發行月份一起介紹

3. 使用發行排程表的&#x200B;**`>[!IMPORTANT]`區塊**

4. **H2`Adobe Workfront enhancements`**&#x200B;包含錨點連結的專案符號清單：

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. 每個產品區域&#x200B;**的** H3搭配HTML功能表（請參閱[reference.md](reference.md#overview-feature-table)）
   - 在每個表格中，**最新功能排在前** — 最近的列會顯示在表格頂端（標題列之後）

&#x200B;6. **尾端區段** (H2)：其他區域的發行說明、案頭校訂檢視器更新、公告、API版本、維護更新、訓練更新

### 步驟3：驗證連結

- **產品區域頁面中的總覽連結**：必須指向同一季
   - 正確： `26-q2-release-activity/26-q2-release-overview.md`
   - 錯誤： `26-q1-release-activity/26-q1-release-overview.md`
- 總覽中的&#x200B;**錨點連結**：必須符合H3 ID （小寫、連字型大小）
- 總覽資料表中的&#x200B;**功能連結**：必須使用`class="MCXref xref" xrefformat="{para}"`
- **說明檔案連結**：必須以`/help/quicksilver/`開頭

### 步驟4：驗證日期

- 格式： `{Month} {Day}, {Year}` （例如「2026年3月12日」）
- 將`TBD`用於未知日期
- 產品區域頁面`>[!NOTE]`區塊中的日期必須符合對應的概觀表格列
- 預覽日期應早於生產日期

### 步驟5：常見修正

格式化時套用這些修正：

| 問題 | 修正 |
|-------|-----|
| 錯誤的概觀連結季度 | 更新以符合檔案自己的季度 |
| 缺少`>[!NOTE]`日期區塊 | H2功能標題後新增區塊 |
| 日期格式不一致 | 標準化為`Month Day, Year` |
| `>[!NOTE]`前遺漏空白行 | 新增空白行 |
| 編號說明行中的額外空格 | 修剪尾隨空格 |
| 產品區域頁面中的HTML | 維持為Markdown （HTML僅適用於概觀表格） |
| 遺失`exl-id` | 將其忽略 — 不要產生一個 |

## 檔案命名慣例

| 類型 | 模式 | 範例 |
|------|---------|---------|
| 概觀 | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| 產品區域 | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| 目錄 | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

標準區域概要： `admin-and-setup`、`documents`、`projects`、`reports`、`requests`、`other`

## 季度對應

| 季度 | 書面形式 | 月 |
|---------|-------------|--------|
| Q1 | 第一季 | 3月1日 |
| Q2 | 第二季 | 4月6日 |
| Q3 | 第三季 | 2020年7月 |
| Q4 | 第四季 | 10月至12月 |

每季的製作版本通常會在當季最後一個月的第二個整週的星期四推出。

## 驗證檢查清單

檢閱發行說明檔案時，請確認：

- [ ] Frontmatter的所有必要欄位都具有正確的值
- [ ] H1符合頁面型別格式
- [ ]概觀連結指向正確的季度
- [ ]每個功能都有`>[!NOTE]`個日期區塊（產品區域頁面）
- [ ]日期格式一致(`Month Day, Year`)
- [ 概覽中的]功能表格列符合產品區域頁面內容
- [ ]沒有中斷的內部連結
- [ 總覽中的]個錨點連結符合H3區段ID
- [ ]功能是以最新優先順序排列（產品區域頁面和概觀表格）

## 其他資源

- 如需完整的HTML範本和範例，請參閱[reference.md](reference.md)
