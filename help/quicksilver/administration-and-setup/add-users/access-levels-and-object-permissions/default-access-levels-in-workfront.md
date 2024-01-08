---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，許可權
navigation-topic: access-levels
title: 內建存取層級
description: 目前內建的六個存取層級中的每一個層級都是為特定型別的使用者設計的，包括系統管理員、供需規劃員、工作者、檢閱者、請求者和外部使用者。 這些存取層級可讓您控制哪些使用者可以在系統中編輯和檢視。 如果您需要自訂存取層級，可以複製內建存取層級，並根據您想要它允許各種Workfront物件型別的存取量進行修改。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 5%

---

# 內建存取層級

<!--Audited: 01/2024-->

>[!NOTE]
>
>本文說明Adobe Workfront中目前的內建存取層級。 如需新的內建存取層級的詳細資訊，請參閱 [新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


目前內建的六個存取層級，每個層級都是針對特定型別的使用者而設計。 這些存取層級可讓您控制哪些使用者可以在系統中編輯和檢視。

六個內建存取層級分別針對下列使用者型別而設計：

* 系統管理員
* 規劃工具
* 工作者
* 檢閱者
* 請求者
* 外部使用者

根據存取層級，大多數Workfront物件型別最多可使用3個設定：

<table style="table-layout:auto">
    <tr>
        <td>編輯</td>
        <td>使用者可以建立、編輯、刪除和共用Workfront物件</td>
    </tr>
    <tr>
        <td>檢視</td>
        <td>使用者可以檢閱和共用Workfront物件</td>
    </tr>
    <tr>
        <td>無存取權限</td>
        <td>使用者無法存取Workfront物件</td>
    </tr>
</table>

如果您需要自訂供需規劃員、員工、請求者或檢閱者存取層級，您可以複製內建存取層級，並決定允許各種Workfront物件型別的存取量。

>[!TIP]
>
>您無法修改系統管理員或外部使用者存取層級。

如需有關建立自訂存取層級或修改其中一個內建存取層級的資訊，請參閱 [建立和修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。

如需這些存取層級的一般資訊，請參閱 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## 系統管理員存取層級

內建的「系統管理員」存取層級附加至「計畫」授權，專為負責管理Adobe Workfront系統的使用者所設計。 您無法修改此內建存取層級。

具有系統管理員存取層級的使用者可以在Workfront中執行所有操作。 他們可以檢視及編輯所有其他使用者在Workfront中輸入的所有Workfront物件和資訊。

使用者也可完整存取「設定」區域，在此變更系統層級的任何設定。 而且他們可以存取主功能表中的所有區域 ![](assets/main-menu-icon.png) 或主要功能表 ![](assets/lines-main-menu.png)，如果有的話。

如需詳細資訊，請參閱 [授予使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## 規劃工具存取層級

同樣附加於計畫授權的「供需規劃員」存取層級專為：

* 群組、團隊、專案和資源的管理員
* 任何負責計畫、建立和管理任務、專案、投資組合和計畫的人
* 負責將工作（任務和問題）指派給其他使用者的任何人
* 建立報告及核準時程表、工作專案和檔案的使用者
* 需要存取主功能表中所有區域的使用者 ![](assets/main-menu-icon.png) 或主要功能表 ![](assets/lines-main-menu.png)，若有

您可以建立Planner內建存取層級的自訂版本，並決定其允許各種Workfront物件型別的存取量。 如需詳細資訊，請參閱 [建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

以下是「供需規劃員」存取層級中物件可用的最高存取設定：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 |   |   | ✓ (A) |
| 任務 |   |   | ✓ (A) |
| 問題 |   |   | ✓ (A) |
| 專案組合 |   |   | ✓ (A) |
| 計劃 |   |   | ✓ (A) |
| 報告、儀表板和行事曆 |   |   | ✓ (A) |
| 篩選器、檢視和群組 |   |   | ✓ (A) |
| 文件 |   |   | ✓ (A) |
| 使用者 |   |   | ✓ (A) |
| 團隊 |   |   | ✓ (A) |
| 範本 |   |   | ✓ (A) |
| 財務資料 |   |   | ✓ (A) |
| 資源管理 |   |   | ✓ (A) |
| 情境規劃工具 |   |   | ✓ （預設設定為「無存取權」。） |
| Workfront Goals |   |   | ✓ （預設設定為「無存取權」。） |

{style="table-layout:auto"}

## 工作者存取層級

「背景工作」存取層級附加至「工作」授權，專為在Workfront中執行工作的使用者設計。 他們不會計畫工作，而會完成工作。

具有此存取層級的使用者：

* 會指派給可以貢獻並記錄時間的工作專案
* 可以核准工作和檔案，但不能核準時程表
* 可存取和共用報告
* 可以與系統中的其他使用者通訊
* 無法存取主功能表中的所有區域 ![](assets/main-menu-icon.png) 或主要功能表 ![](assets/lines-main-menu.png)，如果有，則其「使用者」區域將命名為團隊。 在「專案團隊」區域中，具有此存取層級的使用者只能檢視他們所屬的專案團隊，以及指派給這些專案團隊的工作。
* 建立物件的能力有限 — 他們無法建立專案、投資組合、計畫或報告。

您可以建立Worker內建存取層級的自訂版本，並決定其允許各種Workfront物件型別的存取量。 如需詳細資訊，請參閱 [建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

以下是「背景工作」存取層級中物件的最高存取設定：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 |   |   | ✓ （有限：使用者只能共用專案、在專案中建立任務和問題，以及在已附加至專案的自訂表單中編輯資料。） |
| 任務 |   |   | ✓ (A) |
| 問題 |   |   | ✓ (A) |
| 專案組合 |   | ✓ （預設設定為「無存取權」。） |   |
| 計劃 |   | ✓ （預設設定為「無存取權」。） |   |
| 報告、儀表板和行事曆 |   | ✓ (A) |   |
| 篩選器、檢視和群組 |   |   | ✓ (A) |
| 文件 |   |   | ✓ (A) |
| 使用者 |   |   | ✓ (A) |
| 團隊 |   |   | ✓有限存取 |
| 範本 | ✓ (A) |   |   |
| 財務資料 |   | ✓ (預設設定為「無存取權」。 檢視設定可讓使用者僅檢視專案詳細資訊中的財務區域。) |   |
| 資源管理 |   | ✓ (A) |   |
| 情境規劃工具 |   |   | ✓ （預設設定為「無存取權」。） |
| Workfront Goals |   |   | ✓ （預設設定為「無存取權」。） |

{style="table-layout:auto"}

## 檢閱者存取層級

「檢閱者」存取層級附加至「檢閱」授權，專為請求其他使用者工作以及檢閱和核准工作的主管所設計。 他們不是專案所有者或團隊成員，但他們需要存取Workfront以檢視他們監督的工作專案。

例如，具有此存取層級的利害關係人可以登入Workfront以參與行銷資料的持續稽核，檢視工作更新並稽核檔案、核准、報告和行事曆。

具有檢閱者存取層級的使用者：

* 無法指派工作專案或核準時程表
* 可以存取主功能表中的「請求與檔案」區域 ![](assets/main-menu-icon.png) 或主要功能表 ![](assets/lines-main-menu.png)，若有
* 建立物件的能力有限 — 他們無法建立專案、投資組合、計畫或報告。

您可以建立Reviewer內建存取層級的自訂版本，並決定其允許各種Workfront物件型別的存取量。 如需詳細資訊，請參閱 [建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

專案與任務的限制比「背景工作」存取層級更有限，以下是「稽核者」存取層級中物件可用的最高存取設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront物件型別</th> 
   <th>無存取權</th> 
   <th>檢視存取權</th> 
   <th>編輯存取權</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>專案</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td> </td> 
   <td>✓ （預設設定為「無存取權」。）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計劃</td> 
   <td> </td> 
   <td>✓ （預設設定為「無存取權」。）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>報告、儀表板、行事曆</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>篩選器、檢視和群組</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
<tr> 
   <td>團隊</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr>

<tr> 
   <td>範本</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>財務資料</td> 
   <td> </td> 
   <td> <p>✓ (預設設定為「無存取權」。 檢視設定可讓使用者僅檢視專案詳細資訊中的財務區域。)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源管理</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>情境規劃工具 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ （預設設定為「無存取權」。）</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ （預設設定為「無存取權」。）</td> 
  </tr> 
 </tbody> 
</table>

## 要求者存取層級

請求者存取層級附加於請求授權，專為在Workfront中提出及接收簡單工作請求的使用者而設計。 依預設，這些區域限制在請求區域。

例如，使用者可以將問題記錄到您組織的服務檯請求佇列。

具有此存取層級的使用者：

* 可以提出要求並更新這些要求
* 可以上傳和核准檔案
* 可以檢閱他們已提交問題的狀態
* 無法指派給工作專案
* 只能從主功能表的請求區域存取請求 ![](assets/main-menu-icon.png) 或主要功能表 ![](assets/lines-main-menu.png)，如果有的話。 如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您可以建立請求者內建存取層級的自訂版本，並決定其允許各種Workfront物件型別的存取量。 如需詳細資訊，請參閱 [建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

以下是「請求者」存取層級中物件可用的最高存取設定：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 |   | ✓ （僅限專案詳細資訊頁面） |   |
| 任務 |   | ✓ （僅限任務詳細資訊頁面） |   |
| 問題 |   |   | ✓ (A) |
| 專案組合 | ✓ (A) |   |   |
| 計劃 | ✓ (A) |   |   |
| 報告、儀表板和行事曆 |   | ✓ (A) |   |
| 篩選器、視圖和分組 |   |   | ✓ (A) |
| 文件 |   |   | ✓ (A) |
| 使用者 |   | ✓ (A) |   |
| 團隊 |   | ✓ (A) |   |
| 範本 | ✓ (A) |   |   |
| 財務資料 | ✓ (A) |   |   |
| 資源管理 | ✓ (A) |   |   |
| 情境規劃工具 | ✓ (A) |   |   |
| Workfront Goals |   |   | ✓ （預設設定為「無存取權」。） |

{style="table-layout:auto"}

## 外部使用者存取層級

外部使用者存取層級未附加至付費Workfront授權。 這是限制最嚴格的存取層級，主要是為未登入Workfront但偶爾需要檢閱、下載或檢視檔案的外部顧問等共同作業人員所設計。

即使外部使用者無法登入系統，Workfront使用者仍可以將任務指派給外部使用者。 但是，我們不建議將任務和問題指派給外部使用者，因為那項工作在系統中將維持未解決。

具有外部使用者存取層級的使用者：

* 只能檢視與其共用的檔案和行事曆報告
* 可檢視與他們共用檔案和行事曆報表的使用者
* 可以核准與其共用的檔案

您無法修改此存取層級。

>[!IMPORTANT]
>
>只有在「設定」的「系統偏好設定」區域中啟用「透過電子郵件地址與沒有Workfront帳戶的人合作」選項時，外部使用者才可用。 如需詳細資訊，請參閱 [設定系統安全性偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

雖然這些設定不會顯示在外部使用者存取層級的存取層級區域中，但具有此存取許可權的使用者對Workfront物件型別具有下列最高存取許可權：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 | ✓ (A) |   |   |
| 任務 | ✓ (A) | |   |
| 問題 | ✓ (A) |   |   |
| 專案組合 | ✓ (A) |   |   |
| 計劃 | ✓ (A) |   |   |
| 報告、儀表板和行事曆 |   | ✓ （僅適用於行事曆報表；無法共用報表） |   |
| 篩選器、檢視和群組 | ✓ (A) |   |   |
| 文件 |   | ✓ （無法共用檔案） |   |
| 使用者 |   | ✓ (A) |   |
| 團隊 |   | ✓ (A) |   |
| 範本 | ✓ (A) |   |   |
| 財務資料 | ✓ (A) |   |   |
| 資源管理 | ✓ (A) |   |   |
| 情境規劃工具 | ✓ (A) |   |   |
| Workfront Goals | ✓ (A) |   |   |
