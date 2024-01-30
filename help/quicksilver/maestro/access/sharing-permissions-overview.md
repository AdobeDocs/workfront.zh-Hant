---
title: 在Adobe Maestro中共用許可權概觀
description: 您可以共用或移除Adobe大師工作區或檢視的許可權。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 72d044541f8e061c51c4483672a89ce20e4f30d9
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# 在Adobe Maestro中共用許可權概觀

{{maestro-important-intro}}

您可以共用或移除Adobe大師工作區或檢視的許可權。

本文說明Maestro物件的許可權層級。

如需有關如何共用工作區或檢視的資訊，請參閱下列文章：

* [共用工作區](/help/quicksilver/maestro/access/share-workspaces.md)

* [共用檢視](/help/quicksilver/maestro/access/share-views.md)

## 您可以在Adobe大師中共用的物件

您可以在Maestro中共用下列物件：

* 工作區

  當您共用工作區時，也會共用與工作區相關聯的所有記錄型別、記錄和欄位。 檢視不會共用。

* 檢視

## 在Maestro中共用物件的考量事項

* 您必須擁有下列授權才能在Maestro中建立工作區：

   * 新的定價模式：標準授權
   * 目前的訂價模式：計畫授權。

  如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* 系統管理員可以管理和共用其他使用者建立的工作區。
* 如果您不是系統管理員，且其他人建立的工作區已共用給您，您就可以為其貢獻內容。
* 您無法大量共用工作區。
* 您可以與下列實體共用工作區：
   * 使用者
   * 群組
* 其他使用者（包括系統管理員）只能存取他們已建立或已與他們共用的檢視。
* 您可以與其他人共用工作區的連結，或從記錄型別頁面共用檢視。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取所選檢視中顯示的工作區或記錄型別頁面。

## 共用Maestro物件的許可權

以下各節中的表格說明在共用Maestro工作區或檢視時可以選取的許可權層級，以及每個層級允許的功能。

### 工作區許可權

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 編輯 | ✓ (A) |            |       |
| 共用 | ✓ (A) |            |       |
| 刪除 | ✓ (A) |            |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |

### 記錄型別許可權

當您授予工作區許可權時，會繼承記錄型別許可權。

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ (A) |            |       |
| 刪除 | ✓ (A) |            |       |
| 編輯 | ✓ (A) |            |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |

### 記錄許可權

當您授予工作區許可權時，會繼承記錄許可權。

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ (A) |            |       |
| 刪除 | ✓ (A) | ✓ (A) |       |
| 編輯 | ✓ (A) | ✓ (A) |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |

### 欄位許可權

當您授與工作區許可權時，會繼承欄位許可權。
以下許可權是指欄位本身，而不是與每個欄位關聯的值。 若要編輯欄位值，您必須擁有編輯記錄的許可權。

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ (A) |            |       |
| 刪除 | ✓ (A) |            |       |
| 編輯 | ✓ (A) |            |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |


### 檢視許可權

您必須授予個別許可權才能記錄檢視。 授予工作區許可權不會授予工作區中記錄檢視的許可權。

|        | 管理 | 檢視 |
|--------|--------|-------|
| 編輯 | ✓ (A) |       |
| 刪除 | ✓ (A) |       |
| 檢視 | ✓ (A) | ✓ (A) |
| 套用 | ✓ (A) | ✓ (A) |






