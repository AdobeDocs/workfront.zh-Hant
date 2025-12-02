---
title: 在Adobe Workfront Planning中共用許可權概觀
description: 並非組織中的所有使用者都有相同的存取權和許可權來使用Adobe Workfront Planning。 本文會說明共用或移除Adobe Workfront Planning工作區或檢視之許可權的一般資訊。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# 在Adobe Workfront Planning中共用許可權的概觀

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

您可以共用或移除Adobe Workfront Planning工作區、記錄型別或檢視的許可權。

您也可以共用Planning請求表單。 如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。

本文說明Workfront Planning工作區、記錄型別、記錄、欄位及檢視的許可權層級。

## 可在Adobe Workfront Planning中共用的物件

您可以手動共用某些Workfront Planning物件，而其他物件會繼承其他物件的這些許可權。

您可以在Workfront Planning中手動共用下列物件：

* 工作區

   * 您可以和組織內部人員共用工作區。
   * 當您共用工作區時，也會共用與工作區相關聯的所有記錄型別、記錄和欄位。
   * 當您共用工作區時，檢視不會共用。 檢視會個別共用。

  如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)

* 記錄類型

   * 您可以和組織內部人員共用記錄型別。
   * 授予工作區的許可權層級會顯示為記錄型別的繼承許可權。
   * 您無法以高於使用者在工作區上的許可權層級來共用記錄型別。

  如需詳細資訊，請參閱[共用記錄型別](/help/quicksilver/planning/access/share-record-types.md)。


* 檢視

   * 您必須授予使用者（包括系統管理員）存取檢視的許可權，而不授予其存取工作區的許可權。
   * 當您共用檢視時，會共用所有檢視元素，包括篩選、分組、排序或設定。
   * 當您共用檢視時，檢視中顯示的記錄不會共用。 記錄必須透過共用工作區來共用。
   * 當您產生檢視的公開連結時，您可以與組織外部的人員公開共用檢視。透過公開連結存取記錄頁面的人員可以檢視所有記錄及其欄位，包括連線的記錄和欄位。

  如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。

## 在Adobe Workfront Planning中共用物件的相關考量事項

* 您的Adobe Workfront授權型別與Workfront Planning許可權搭配使用，可讓您檢視、貢獻或管理工作區及其物件。

  如需授權型別如何影響Workfront Planning許可權等級的資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。
* 系統管理員可以管理系統中的所有工作區，包括他們未建立的工作區。
* 其他使用者（包括系統管理員）只能存取他們已建立或已與他們共用的檢視。 系統管理員只能獲得管理檢視的許可權。

* 當您與他人共用工作區和記錄型別時，記錄型別的許可權層級會自動繼承到與其關聯的記錄和欄位。

  >[!IMPORTANT]
  >
  >如果您組織的Workfront例項已上線至Adobe統一體驗，則您想要與其共用Planning物件的使用者必須新增至Adobe Admin Console。 您無法與尚未新增至Adobe Admin Console的Workfront使用者共用Planning物件。

* 您可以透過下列方式共用Planning物件：

   * 在內部，您可以與下列Workfront實體共用工作區、檢視或記錄型別：

      * 使用者
      * 群組
      * 團隊
      * 公司
      * 職務角色

     您可以與每個物件最多100個實體共用Planning物件。

   * 在內部，透過與其他Planning使用者共用工作區或檢視的連結。 存在下列情況：

      * 收到工作區連結的使用者必須是作用中使用者，並登入Workfront才能存取工作區。
      * 收到檢視的內部共用連結的使用者必須是作用中使用者，並且登入Workfront才能存取檢視。
   * 從外部來說，透過與沒有Workfront帳戶的外部使用者共用檢視的公開共用連結。

## 共用Adobe Workfront Planning物件的許可權

以下各節中的表格說明了共用工作區或檢視時您可以選取的許可權層級，以及每個層級允許的功能。

>[!IMPORTANT]
>
>並非所有使用者都可擁有下述許可權層級。 使用者的個別授權會決定他們可以針對Workfront Planning物件接收的許可權層級。
>
>只有標準（或計畫）授權使用者才能擁有工作區的「貢獻」或「管理」許可權，以及檢視的「管理」許可權。
> 
>具有所有其他授權型別的使用者可以擁有對工作區和檢視的檢視許可權。
>
>如需詳細資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。


### 工作區的許可權

您必須授予使用者對工作區的許可權，才能允許他們存取下列實體：

* 工作區
* 記錄類型
* 記錄
* 欄位

以下是工作區的許可權層級：

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 編輯 | ✓ |            |       |
| 共用 | ✓ |            |       |
| 刪除 | ✓ |            |       |
| 檢視 | ✓ | ✓ | ✓ |

### 記錄型別的許可權

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

當您授予工作區許可權時，會一律繼承記錄型別許可權。

您可以移除從工作區接收的記錄型別繼承許可權。

您可以授予使用者比他們在工作區中擁有更低的記錄型別許可權。

但是，您不能執行下列動作：

* 授予記錄型別比使用者在工作區上更高的許可權。
* 為工作區管理員提供記錄型別的較低許可權。
* 從記錄型別許可權中移除使用者，以移除記錄型別或工作區的檢視許可權。

存在下列情況：

| Workspace許可權 | 記錄型別的自動繼承許可權 | 已關閉繼承許可權時可能的記錄型別許可權（手動授予） |
|--------|--------|-------------|
| 管理 | 管理 | 管理，移除許可權* |
| 參與 | 參與 | 參與、檢視、移除許可權* |
| 檢視 | 檢視 | 檢視，移除許可權* |

>[!NOTE]
>
>當您從記錄型別中移除許可權時，使用者仍然保留對工作區和所有記錄型別的檢視許可權，除非您從工作區中移除其許可權。

### 記錄的許可權

當您將許可權授予工作區和記錄型別時，記錄許可權是從記錄型別繼承的。

以下是記錄的許可權層級：


|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ | ✓ |       |
| 刪除 | ✓ | ✓ |       |
| 編輯 | ✓ | ✓ |       |
| 檢視 | ✓ | ✓ | ✓ |

### 記錄欄位的許可權

當您授與許可權給工作區和記錄型別時，欄位許可權是從記錄型別繼承的。

以下許可權是指欄位本身，而不是與每個欄位關聯的值。 若要編輯欄位值，您必須擁有編輯記錄的許可權。

|        | 管理 | 參與 | 檢視 |
|--------|--------|------------|-------|
| 建立 | ✓ |            |       |
| 刪除 | ✓ |            |       |
| 編輯 | ✓ |            |       |
| 檢視 | ✓ | ✓ | ✓ |


### 檢視的許可權

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
| 編輯 | ✓ |       |                            |
| 刪除 | ✓ |       |                            |
| 共用 | ✓ |       |                           |
| 檢視 | ✓ | ✓ | ✓ |
| 套用 | ✓ | ✓ | ✓ |

| 公開共用 | 檢視 |
|--------|-------|
| 檢視 | ✓ |
| 套用 | ✓ |

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
