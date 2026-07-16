---
title: Adobe Workfront Planning作為獨立產品所需的存取
description: 本文說明Adobe Workfront Planning作為獨立產品的授權、存取層級和使用者功能。
last-update: 2026-04-01T18:02:40Z
git-commit-file: 8cc175490a6aa1db68b238edbdf9da9da7fbb258
source-git-commit: b186900d58f6a422c787cef881a4d06d6cd7feed
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 2%

---

<!--

Update metadata with this at release:
---
title: Access Required for Planning Standalone
description: This article describes how you can benefit from using the standalone version of Adobe Workfront Planning.
feature: Workfront Planning (******************ask Bob for a new feature???***********)
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

# Adobe Workfront Planning作為獨立產品所需的存取權

>[!IMPORTANT]
>
>本文資訊是指Adobe Workfront Planning （購買獨立產品時）。 當您的公司購買僅Adobe Workfront Planning套件，但未購買Workfront Workflow套件時，請參閱本文。
>
>如需搭配Adobe Workfront Workflow套件一起購買時的Workfront Planning相關資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

本文說明Adobe Workfront Planning作為獨立產品的授權、存取層級和使用者功能。

## Workfront計畫套件

您的組織可以購買下列其中一個獨立的Workfront Planning套件：

* Prime
* 選擇
* Ultimate

下表說明每個封裝包含的內容：

| 規劃功能 | 選擇 | Prime | Ultimate |
|---|---|---|---|
| 規劃、協調、行銷活動管理 | ✓ | ✓ | ✓ |
| Unlimited工作區 | ✓ | ✓ | ✓ |
| 每個工作區的記錄數 | 25,000 | 500,000 | 1,000,000 |
| 記錄總數（所有工作區） | 500,000 | 2,000,000 | 無限制 |
| 全域記錄型別和跨工作區連線 | — | ✓ | ✓ |
| 在發行時存取未來功能 | 部分 | 部分 | 最多 |

## Workfront Planning套件可用性

<!--
the bullets repeat in the "Planning overview" article
-->

當您的組織購買下列其中一個Workfront套件時，即可存取Workfront計畫：

* Workfront Workflow和Workfront Planning一起購買。 組織中的每個使用者都有「工作流程」和「計畫」授權。 這可讓所有使用者完整存取這兩個模組的所有Workfront功能。

* 適用於組織中每個人的Workfront工作流程以及僅適用於組織中某些使用者的Workfront Planning。 這可讓使用者完整存取所有Workflow的功能，並為已指派Planning授權的使用者提供對Planning功能的更有限存取權。

* Workfront Planning可作為獨立產品，供貴組織使用者使用。 這讓使用者無法存取任何Workfront Workflow功能，也無法存取Planning功能。

如需以獨立產品形式包含在Planning中的功能相關資訊，請參閱文章[以獨立產品形式開始使用Workfront Planning ](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)中的「Adobe Workfront Planning中包含的功能」一節。

## 使用者授權和存取層級

<!-- should this be moved to the Manage users in Planning article??-->

Planning授權是指派給使用者的存取層級的一部分。

對於Planning作為獨立產品，您無法指派授權給存取層級 — 這些授權已硬式編碼為包含在指派給使用者的存取層級中。

視貴組織購買的Workfront Planning套件組合而定，您的使用者可能會有以下其中一個存取層級：

* **計畫管理員**：可用於Workfront計畫套件。 將使用者新增至Admin Console時，會自動指派Planning管理員。
* **規劃標準**：適用於所有Workfront規劃套件。 建立使用者時，您可以將此存取層級指派給使用者。

<!--
this is not available for Planning STA: 
* **Planning Contributor**: Available for the following customers: 

    * Customers that purchase equal amounts of Workflow and Planning packages together. In this case, Planning Contributors have limited access to Planning objects.
    * Customer that purchase unequal amounts of Workflow and Planning packages. In this case, Planning Contributors have read-only access to Planning objects.

-->

每個獨立Planning授權都會對應至系統中的角色，並控制可存取的產品區域。

下表說明Workfront Planning中每個Planning授權型別及其功能（若以獨立產品形式購買）：

| 功能/授權型別 | 規劃管理員 | 規劃標準 |
|---|---|---|
| 存取層級說明 | 完整系統存取 | 可以管理工作區和內容 |
| 主功能表中的Planning區域 | ✔ | ✔ |
| 主功能表中的「使用者」區域 | ✔ | 僅限檢視 |
| 主要功能表中的請求區域 | ✔ | ✔ |
| 主要功能表的設定區域 | ✔ |   |
| 管理工作區及其內容 | ✔ | ✔ |
| 與團隊共用Planning資料 | ✔ | ✔ |
| 提交請求 | ✔ | ✔ |
| 建立或編輯使用者 | ✔ |   |
| 檢視使用者清單 | ✔ | 僅限檢視 |
| 設定>團隊 | ✔ |   |
| 設定>登入身份 | ✔ |   |
| 設定>自訂季度 | ✔ |   |
| 設定>系統>客戶資訊 | ✔ |   |
| 設定>系統>偏好設定 | ✔ |   |

如需有關指派使用者存取層級的資訊，請參閱[在Adobe Workfront Planning中將使用者管理為獨立產品](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)。

## 導覽區域和存取層級相依性

根據Planning授權，使用者在其全域導覽中可能有不同的可用區域。

<!--
>[!NOTE]
>
>Workfront-specific toolbar actions (Search, Recents, Favorites, Notifications) are not available in the Workfront header for any Standalone user.
-->

### Planning管理員導覽概觀

<!--
Managing your Adobe Workfront Planning instance is similar to managing an Adobe Workfront with Planning instance, but there are some differences.
-->

具有「Planning管理員」存取層級的使用者具有下列權能：

* 擁有系統的完整管理存取權。
* 可以建立和編輯使用者、管理團隊、設定自訂季度，以及存取所有「設定」子頁面。

  如需詳細資訊，請參閱：

   * [在Adobe Workfront Planning中作為獨立產品管理使用者](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)
   * [以獨立產品形式管理Adobe Workfront Planning中的團隊](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)
* 可以提交及管理請求。

  如需詳細資訊，請參閱[Adobe Workfront規劃要求：文章索引](/help/quicksilver/planning/requests/requests-article-index.md)。
* 在主要功能表中有下列區域：

   * **Planning**：具有完整功能，可讓Planning物件建立、刪除、共用及連線物件。
   * **使用者**：您可以新增使用者並編輯其設定檔。
   * **請求**
   * **設定**
* 在「設定」區域中有下列區段：

   * **團隊**：您可以新增、移除或編輯團隊。 編輯僅限於專案團隊名稱、說明和成員；沒有可用的篩選、檢視、分組或匯出控制項。
   * **以**&#x200B;身分登入：模擬其他使用者以進行疑難排解。
   * **自訂季度**：設定出現在Planning時間表檢視中的自訂會計季度。
   * 系統

* 在「系統」區域中有下列區段：

   * **客戶資訊**：檢視客戶與組織詳細資料。
   * **偏好設定**：檢閱並設定系統層級的偏好設定。

### Planning Standard導覽概觀

具有Planning標準存取層級的使用者具有下列功能：

* 可以管理工作區及其內容。
* 可以提交及管理請求。

  如需詳細資訊，請參閱[Adobe Workfront規劃要求：文章索引](/help/quicksilver/planning/requests/requests-article-index.md)。
* Planning Standard使用者可在主功能表中存取下列區域：

   * **規劃**
   * **使用者**：他們擁有使用者的僅限檢視存取權。 他們無法建立或編輯使用者。<!--not sure if this is still true-->
   * **請求**

* 無法存取「設定」或其任何區段。

## 將Planning的存取層級設定為獨立產品

當您購買Planning作為獨立產品時，存取層級是內建的，而且您無法為Planning使用者設定它們。

若要將存取層級指派給使用者，請以Planning管理員的身分：

* 在Adobe Console中建立使用者。

  存在下列情況：

   * 新增至Adobe Console作為管理員的使用者，可在Workfront Planning中獲得Planning管理員存取層級。
   * 新增至Adobe Console的使用者（作為使用者）可以在Workfront Planning中指派為Planning標準存取層級。 這是唯一可指派給Workfront Planning中新使用者作為獨立產品的存取權。

如需詳細資訊，請參閱[管理使用者](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)。

## 在Workfront Planning中作為獨立產品授予許可權

您可以在Workfront Planning中作為獨立產品共用下列物件：

* 工作區
* 記錄類型
* 記錄
* 檢視

以獨立產品形式共用Planning中的物件，等同於與Workflow套件一起購買時在Planning中共用物件。

如需詳細資訊，請參閱[Adobe Workfront Planning存取資訊：文章索引](/help/quicksilver/planning/access/access-information.md)。

<!--

I took this out because there is NO Contributor for true STA: 

### Planning Contributor user experience

>[!IMPORTANT]
>
>Planning Contributor access level is only available for customers that purchase both Workfront Planning and a Workfront Workflow package together. 
>
>If they purchase unequal numbers of packages for the two modules, the Planning Contributor license is read-only. 

When standalone Workfront Planning users purchase a Workflow package, they receive a read-only Planning Contributor license by default. 

For more information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

A user with a Planning Standard access level has the following capabilities: 

* View-only access to Planning data, equivalent to the Contributor license in Workfront.
* Can access the following areas in the Main menu:
    * **Planning**
    * **Requests**
* Can submit requests.
* No access to the Users list.
* No access to Setup or any of its sub-pages.

-->

<!-- 
this was moved from the STA general article - some information is already above - take out here what is not needed or add above: 

## Package overview

The following packages are available for Workfront Planning as a standalone product:

* Select
* Prime
* Ultimate

The following table describes what is included in each package:  

| Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Licensing overview

Consider the following about Workfront Planning licenses:

* Your organization can purchase Workfront Planning licenses without requiring Workfront or Workflow licenses.
* You can add users to Workfront Planning using the Adobe Experience Platform.

    For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 
* Workfront Planning users are limited to Planning-only capabilities and do not receive access to any Workfront areas or capabilities.

The following access levels are hard-coded in Workfront Planning and cannot be modified: 

* Planning Administrator
* Planning Standard 

>[!IMPORTANT]
>
>In a Workfront Planning context, a user must hold a **Planning Standard** license to access the product. 

For more information, see [Access needed for Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md). 

## How licensing works for customers with a Planning and Workfront combined package

Consider the following if you have both the Workfront Workflow and Planning packages:

* A Planning Contributor read-only license is available for users in Planning. 
* Any Workfront access level (including Light or Contributor) can be paired with either a Planning Standard or Planning Contributor access level, regardless of the Workfront Workflow license type.

    For example, a user with a Workfront Contributor license can still hold a Planning Standard license and have full Planning management capabilities.

### Mixed License access matrix

When a customer has both Planning and Workfront packages, access levels are determined by the combination below:

| Access Type | Planning License | Workflow License | License Origin |
|---|---|---|---|
| Default | Read Only | Workfront Light | Workfront |
| Default | Read Only | Workfront Standard | Workfront |
| Default | Read Only | Workfront Contributor | Workfront |
| Default | Read Only | Workfront External | Workfront |
| Default | Planning Standard | Workfront Contributor | Planning |
| — | Planning Standard | Workfront Light | Either Planning or Workfront |
| — | Planning Standard | Workfront Standard | Either Planning or Workfront |

Consider the following if your organization has purchased Workfront with Planning:

* Adding a new user to Planning or Workfront automatically creates default (read-only) access in the other product.
* You can upgrade the access in the opposite product. For more information, contact your account representative.

### Upgrading from standalone Planning to a Planning with a Workflow package

#### Workfront Planning with a Workfront Workflow package

When you add a Workfront Planning Standalone package to an existing Workflow license, the following changes take effect automatically:

* Planning Administrators are promoted to System Administrators.
* Non-admin Planning users (Standard and Contributor) receive Workflow Contributor licenses.
* All existing Planning data is preserved.
* All newly provisioned Workfront users are auto-assigned Planning Contributor (read-only) licenses.

#### License mapping when you upgrade to a Planning with Workflow package

| Before (Planning Standalone) | After (Workfront + Planning) |
|---|---|
| Planning Administrator | System Administrator |
| Planning Standard | Workflow Contributor |
| Planning Contributor | Workflow Contributor |

Planning and Workflow licenses remain separate after the upgrade. A Planning Standard user can hold a Workflow Contributor license, and a Planning Contributor user can hold a Workflow Standard license — these are assigned independently based on need.

All users receive an email notification when they gain access to the additional Workflow capabilities in Workfront.

-->

<!--
I took out the last column on this table and added above:

| Feature / Access | Planning Administrator | Planning Standard | Planning Contributor |
|---|---|---|---|
| Access level description | Full system access | Can manage workspaces and content | View-only access to Planning data when Planning packages are in unequal numbers to Workflow licenses. This license is not available for Planning as a standalone product.|
| Planning area in the Main Menu | ✔ | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |   |
| Requests area in the Main Menu | ✔ | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |   |
| Manage Workspaces and their content | ✔ | ✔ |   |
| Submit requests | ✔ | ✔ | ✔ |
| Create or edit users | ✔ |   |   |
| View users list | ✔ | View only |   |
| Setup > Teams | ✔ |   |   |
| Setup > Log In As | ✔ |   |   |
| Setup > Custom Quarters | ✔ |   |   |
| Setup > System > Customer info | ✔ |   |   |
| Setup > System > Preferences | ✔ |   |   |

-->