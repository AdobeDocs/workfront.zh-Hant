---
title: 在Adobe Workfront Planning中共用許可權的概觀
description: 您可以共用或移除Adobe Workfront Planning工作區或檢視的許可權。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# 在Adobe Workfront Planning中共用許可權的概觀

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中共用或移除工作區或檢視的許可權。

本文說明Workfront Planning物件的許可權層級。

如需有關如何共用工作區或檢視的資訊，請參閱下列文章：

* [共用工作區](/help/quicksilver/maestro/access/share-workspaces.md)

* [共用檢視](/help/quicksilver/maestro/access/share-views.md)

## 可在Adobe Workfront Planning中共用的物件

您可以共用下列物件：

* 工作區

  當您共用工作區時，也會共用與工作區相關聯的所有記錄型別、記錄和欄位。 檢視不會共用。

* 檢視

## 在Adobe Workfront Planning中共用物件的相關考量事項

* 您的Adobe Workfront授權型別可與Workfront Planning許可權搭配使用，讓您在使用Workfront Planning時能夠檢視、貢獻或管理物件。

  如需有關授權型別如何影響Workfront Planning許可權等級的資訊，請參閱 [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/maestro/access/license-type-overview.md).
* 系統管理員可以管理和共用其他使用者建立的工作區。
* 如果您不是系統管理員，且其他人建立的工作區已共用給您，您就可以為其貢獻內容。
* 您無法大量共用工作區或檢視。
* 您可以與下列實體共用工作區或檢視：
   * 使用者
   * 群組
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* 其他使用者（包括系統管理員）只能存取他們已建立或已與他們共用的檢視。 系統管理員只能獲得管理檢視的許可權。
* 您可以與其他人共用工作區連結或從記錄型別頁面檢視連結。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取所選檢視中顯示的工作區或記錄型別頁面。

## 共用Adobe Workfront Planning物件的許可權

以下各節中的表格說明了共用工作區或檢視時您可以選取的許可權層級，以及每個層級允許的功能。

>[!IMPORTANT]
>
>並非所有使用者都可擁有下述許可權層級。 使用者的個別授權會決定他們可以針對Workfront Planning物件接收的許可權層級。
>
>如需詳細資訊，請參閱 [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/maestro/access/license-type-overview.md).


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

<!--You can share views internally or publicly. -->

|        | 管理 | 檢視 |
|--------|--------|-------|
| 編輯 | ✓ (A) |       |
| 刪除 | ✓ (A) |       |
| 共用 | ✓ (A) |       |
| 檢視 | ✓ (A) | ✓ (A) |
| 套用 | ✓ (A) | ✓ (A) |

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |
| Delete | ✓      |       |
| Share  | ✓       |       |
| View   | ✓      | ✓     |
| Apply  | ✓      | ✓     |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->