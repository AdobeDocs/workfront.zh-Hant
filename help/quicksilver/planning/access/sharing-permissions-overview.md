---
title: 在Adobe Workfront Planning中共用許可權概觀
description: 並非組織中的所有使用者都有相同的存取權和許可權來使用Adobe Workfront Planning。 本文會說明共用或移除Adobe Workfront Planning工作區或檢視之許可權的一般資訊。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 6%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# 在Adobe Workfront Planning中共用許可權的概觀

{{planning-important-intro}}

您可以共用或移除Adobe Workfront Planning工作區或檢視的許可權。

本文說明Workfront Planning物件的許可權層級。

如需有關如何共用工作區或檢視的資訊，請參閱下列文章：

* [共用工作區](/help/quicksilver/planning/access/share-workspaces.md)

* [共用檢視](/help/quicksilver/planning/access/share-views.md)

## 可在Adobe Workfront Planning中共用的物件

您可以共用下列物件：

* 工作區

   * 您可以和組織內部人員共用工作區。
   * 當您共用工作區時，也會共用與工作區相關聯的所有記錄型別、記錄和欄位。

     當您共用工作區時，檢視不會共用。 檢視會個別共用。

* 檢視

   * 您必須授予使用者（包括系統管理員）存取檢視的許可權，而不授予其存取工作區的許可權。
   * 當您共用檢視時，會共用所有檢視元素，包括篩選、分組、排序或設定。

     當您共用檢視時，檢視中顯示的記錄不會共用。 記錄必須透過共用工作區來共用。
   * 當您產生檢視的公開連結時，您可以與組織外部的人員公開共用檢視。透過公開連結存取記錄頁面的人員可以檢視所有記錄及其欄位，包括連線的記錄和欄位。

  如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。

在內部，您可以與下列Workfront實體共用工作區或檢視：

* 使用者
* 群組

## 在Adobe Workfront Planning中共用物件的相關考量事項

* 您的Adobe Workfront授權型別與Workfront Planning許可權搭配使用，可讓您檢視、貢獻或管理工作區及其物件。

  如需授權型別如何影響Workfront Planning許可權等級的資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。
* 系統管理員可以管理系統中的所有工作區，包括他們未建立的工作區。
* 其他使用者（包括系統管理員）只能存取他們已建立或已與他們共用的檢視。 系統管理員只能獲得管理檢視的許可權。
* 您可以與他人共用工作區的連結或檢視。

  存在下列情況：
   * 收到工作區連結的使用者必須是作用中使用者，並登入Workfront才能存取工作區。
   * 使用者收到檢視的連結後，可透過下列方式存取檢視：

      * 如果檢視的連結為內部共用，則必須是作用中使用者並登入Workfront。
      * 可以是Workfront的外部使用者，不需登入Workfront，即可從公開共用的連結存取檢視。

## 共用Adobe Workfront Planning物件的許可權

以下各節中的表格說明了共用工作區或檢視時您可以選取的許可權層級，以及每個層級允許的功能。

>[!IMPORTANT]
>
>並非所有使用者都可擁有下述許可權層級。 使用者的個別授權會決定他們可以針對Workfront Planning物件接收的許可權層級。
>
>只有Standard （或Plan）授權使用者可以擁有Contribute或工作區的「管理」許可權，以及檢視的「管理」許可權。
> 
>具有所有其他授權型別的使用者可以擁有對工作區和檢視的檢視許可權。
>
>如需詳細資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。


### Workspace許可權

您必須授予使用者對工作區的許可權，才能允許他們存取下列實體：

* 工作區
* 記錄類型
* 記錄
* 欄位

以下是工作區的許可權層級：

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 編輯 | ✓ (A) |            |       |
| 共用 | ✓ (A) |            |       |
| 刪除 | ✓ (A) |            |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |

### 記錄型別許可權

當您授予工作區許可權時，會繼承記錄型別許可權。

記錄型別的許可權層級如下：


|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ (A) |            |       |
| 刪除 | ✓ (A) |            |       |
| 編輯 | ✓ (A) |            |       |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |

### 記錄許可權

當您授予工作區許可權時，會繼承記錄許可權。

以下是記錄的許可權層級：


|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ (A) | ✓ (A) |       |
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

您必須授予使用者檢視的許可權，才能讓使用者存取下列檢視元素：

* 篩選器
* 欄位可見性
* 排序
* 分組
* 列高
* 設定

您可以在內部或公開分享檢視。

以下是檢視和檢視元素的許可權層級：

| 內部共用 | 管理（只有受邀者才能存取） | 檢視（只有受邀者才能存取） | 工作區中的所有人都可以檢視* |
|--------|--------|-------|------------------------------|
| 編輯 | ✓ (A) |       |                            |
| 刪除 | ✓ (A) |       |                            |
| 共用 | ✓ (A) |       |                           |
| 檢視 | ✓ (A) | ✓ (A) | ✓ (A) |
| 套用 | ✓ (A) | ✓ (A) | ✓ (A) |

| 公開共用 | 檢視 |
|--------|-------|
| 檢視 | ✓ (A) |
| 套用 | ✓ (A) |

*使用者必須擁有工作區的檢視或更高許可權才能取得此檢視存取權。

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->