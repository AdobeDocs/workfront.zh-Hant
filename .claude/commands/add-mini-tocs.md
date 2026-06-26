---
name: add-mini-tocs
description: ""
source-git-commit: f0ecec8cac6fc0260cb075ab0fd49d079ae5b4c5
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 新增迷你目錄

掃描Markdown檔案，並在每個具有直接副標題的合格標題下插入迷你目錄。

## 工作流程

1. 讀取目標檔案。
2. 識別在`##`層級或更深層級具有至少一個直接子標題（更深層一個`#`層級）的每個標題。
3. 對於每個此類父標題，僅建立其直接子系之連結的專案符號清單。
4. 在第一個子標題的前面，在父標題之後的任何介紹文字之後插入清單。
5. 如果該位置已存在迷你TOC，請將其與該區段中目前的子標題進行比較。 如果清單過期（遺漏專案、額外專案或不正確的連結），請以更新的清單取代。 如果已經相符，則略過。
6. 寫入更新的檔案。

## 範圍

- **從不**&#x200B;在`#`文章標題下建立迷你目錄。 迷你目錄只會新增到`##`個標題下和更深的標題中。
- `##`標題取得其`###`直接子項的清單。
- `###`標題取得其`####`直接子項的清單。
- 如需更深入的瞭解，請參閱以此類推。

## 連結格式

清單中的每個專案都會使用此確切格式：

```
* [Heading text](#anchor)
```

### 錨點產生規則

將標題文字轉換為錨點，如下所示：

1. 小寫所有文字。
2. 移除任何非字母、數字、空格或連字型大小的字元。
3. 以連字型大小取代空格。
4. 移除任何以反引號括住的程式碼格式（保留內有文字）。

範例： `### Create or edit a function` → `#create-or-edit-a-function`

## 巢狀規則

- 每個清單中僅連結&#x200B;**直接子項** （比父項更深一個層級）。
- 請勿在同一個清單中包含孫子或較深的標題。
- 如果這些小標題本身有小標題，他們會在小標題下方插入自己的迷你目錄。

**範例結構：**

```
## Manage a package          ← parent: gets a list of ### headings
### Functions                ← child of ##, parent of ####: gets a list of #### headings
#### Create a function       ← child of ###
#### Delete a function       ← child of ###
### Variables                ← child of ##
### History                  ← child of ##
```

結果位於：

在`## Manage a package`下：

```
* [Functions](#functions)
* [Variables](#variables)
* [History](#history)
```

在`### Functions`下：

```
* [Create a function](#create-a-function)
* [Delete a function](#delete-a-function)
```

## 產品建議放置環境

在第一個子標題的前面插入迷你目錄清單。 如果父標題和第一個子標題之間有介紹性文字，清單會移至該文字之後，第一個子標題的正上方。 在迷你目錄清單前後一定要加上空白行。

## 要略過的專案

- `#`標題（文章標題）：請勿在此新增迷你目錄。
- 只有一個直接子項的父標題：略過 — 單一專案清單不會新增導覽值。
- 沒有子標題的區段：略過。
