---
title: 新訪問級別概述
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 訪問，級別，系統，管理員，標準，輕量，貢獻者
navigation-topic: access-levels
description: 每個使用者都必須有存取層級才能登入並在Workfront中運作。 您可以使用存取層級來控制使用者可以看到哪些內容，以及如何處理特定Workfront物件和區域。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 26da544bb8cd833d37dd6a484687495fde5060b1
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 4%

---

# 新訪問級別概述

身為Adobe Workfront管理員，您可為使用者指派存取層級，目的有2種：

* 每個使用者都必須有存取層級才能登入並在Workfront中運作。
* 您可以使用存取層級來控制使用者可以看到哪些內容，以及如何處理特定Workfront物件和區域。

## Adobe Workfront中新的內建存取層級 {#built-in-access}

Workfront有5個新的內建存取層級：

* 系統管理員
* 標準
* 輕度
* 投稿人
* 外部

視存取層級而定，大部分的Workfront物件類型最多可使用3個權限：

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

如果您需要自訂存取層級，則可複製內建存取層級，並調整您要其允許的存取量，以用於各種Workfront物件類型。 如需建立自訂存取層級的資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>強烈建議您將內建存取層級維持不變，以便在設定使用者後參照這些層級。

### 系統管理員訪問級別

此內建存取層級附加至標準授權，專為負責管理Adobe Workfront系統的使用者而設計。 您無法修改此內置訪問級別。

具有系統管理員存取層級的使用者可在Workfront中執行所有作業。 他們可以檢視和編輯所有其他使用者在Workfront中輸入的Workfront物件和資訊。

他們還可以訪問完整的「設定」區域，在此可以更改系統級別的任何設定，也可以訪問主菜單中的所有區域。

如需詳細資訊，請參閱 [授予使用者完整的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### 標準訪問級別

此存取層級也附加至標準授權，適用於下列情況的使用者：

* 在一個位置規劃、建立和追蹤所有專案
* 自動執行例行程式
* 管理資源
* 追蹤及協作請求
* 跟蹤和報告項目財務
* 啟動入站工作請求
* 針對專案、任務和問題進行協作

>[!NOTE]
>
>您可以建立標準內建存取層級的自訂版本，並調整其允許的存取量以用於各種Workfront物件類型。 如需建立自訂存取層級的資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資訊**

以下是標準訪問級別中對象可用的最高訪問設定：

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 |   |   | ✓ |
| 任務 |   |   | ✓ |
| 問題 |   |   | ✓ |
| 專案組合 |   |   | ✓ |
| 計劃 |   |   | ✓ |
| 報表（包括控制面板和日曆報表） |   |   | ✓ |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   |   | ✓ |
| 範本 |   |   | ✓ |
| 財務資料 |   |   | ✓ |
| 資源管理 |   |   | ✓ |
| 案例規劃工具 |   |   | ✓（預設設定為「無權存取」）。 |
| 展示板 |   |   | ✓ |
| 首頁 |   |   | ✓ |
| 目標 |   |   | ✓ |

{style="table-layout:auto"}

### 輕量級

此訪問級別附加至Light許可證，面向以下用戶：

* 查看與工作關聯的所有項目和更新
* 核准專案、工作和問題
* 檢視控制面板和報表
* 追蹤時間
* 建立和管理問題
* 更新工作

具有輕量級訪問級別的用戶：

* 無法分配工作項或批准工時單
* 可以訪問主菜單中的請求和文檔。
* 建立對象的能力有限 — 他們不能建立項目、產品組合、方案或報告。

>[!NOTE]
>
>您可以建立Light內建存取層級的自訂版本，並調整其允許的存取量，以用於各種Workfront物件類型。 如需建立自訂存取層級的資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資訊**

以下是「淺色」訪問級別中對象可用的最高訪問設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront物件類型</th> 
   <th>無權存取</th> 
   <th>檢視存取</th> 
   <th>編輯存取</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>專案</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td> </td> 
   <td>✓（預設設定為「無權存取」）。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計劃</td> 
   <td> </td> 
   <td>✓（預設設定為「無權存取」）。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>報表（包括控制面板和日曆報表）</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>篩選器、檢視和群組</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
    <tr> 
   <td>團隊</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>
  <tr> 
   <td>範本</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>財務資料</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源管理</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>案例規劃工具 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓（預設設定為「無權存取」）。</td> 
  </tr> 
  <tr> 
   <td>展示板 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>首頁 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>目標 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### 貢獻者存取層級

此存取層級已附加至貢獻者授權，專為下列使用者而設計：

* 提交請求
* 追蹤請求
* 更新和審核請求。

具有此內置訪問級別的用戶：

* 可以提出請求並更新這些請求
* 可以上傳和核准檔案
* 可以查看已提交問題的狀態
* 無法分配給工作項
* 只能從主功能表存取請求。 如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>您可以建立貢獻者內建存取層級的自訂版本，並調整貢獻者內建各種Workfront物件類型的存取量。 如需建立自訂存取層級的資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資訊**

以下是「貢獻者」存取層級中物件可用的最高存取設定：

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 |   | ✓（僅限「項目詳細資訊」頁） |   |
| 任務 |   | ✓（僅「詳細資訊」頁） |   |
| 問題 |   |   | ✓ |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報表（包括控制面板和日曆報表） |   | ✓（僅限「詳細資訊」頁簽） |   |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   | ✓ |   |
| 團隊 |   | ✓ |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| 展示板 |   |   | ✓（簡單卡） |
| 首頁 |   | ✓（我的更新） |   |
| 目標 |   |   | ✓ |

{style="table-layout:auto"}

### 外部用戶訪問級別

此存取層級未附加至付費Workfront授權。 這是限制最嚴格的存取層級，主要針對未登入Workfront、但偶爾需要檢閱、下載或檢視檔案的外部顧問等共同作業人員。

Workfront使用者可指派工作給外部使用者，即使外部使用者無法登入系統亦然。 但我們建議不要這樣做，因為這一工作在系統中仍未解決。

具有外部用戶訪問級別的用戶：

* 只能查看與它們共用的文檔和日曆報告
* 查看與其共用文檔和日曆報告的用戶
* 核准與其共用的檔案

您無法修改此訪問級別。

>[!IMPORTANT]
>
>只有在「設定」的「系統偏好設定」區域中啟用「透過未使用Workfront帳戶之人員的電子郵件地址與其共同作業」選項時，「外部使用者」才可供使用。 如需詳細資訊，請參閱 [配置系統安全首選項](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **存取詳細資訊**

以下是「外部用戶」訪問級別中對象可用的最高訪問設定。

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 | ✓ |   |   |
| 任務 | ✓ |   |   |
| 問題 | ✓ |   |   |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報表（包括控制面板和日曆報表） |   | ✓(僅用於日曆報告；無法共用報表) |   |
| 篩選器、檢視和群組 | ✓ |   |   |
| 文件 |   | ✓（無法共用檔案） |   |
| 使用者 |   | ✓ |   |
| 團隊 | ✓ |   |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| 展示板 | ✓ |   |   |
| 首頁 | ✓ |   |   |
| 目標 | ✓ |   |   |


## 存取層級與權限如何搭配運作

訪問級別定義了用戶可以查看和處理系統中的一般對象類型和區域（如項目、任務和問題）的內容。 權限會定義您對系統中其他人員建立的特定物件（例如為執行行銷活動而建立的專案）的存取權。

下表將用戶對對象的一般訪問（由用戶的訪問級別定義）與特定共用對象的權限進行比較：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>存取層級 </th> 
   <th>權限 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>由Workfront管理員授與使用者的存取層級</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>由在對象級別共用對象的用戶授予</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>繼承自排名較高的共用物件 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

使用者可以對物件執行的活動，是透過其存取層級與授予對象的權限組合而定義。

![](assets/security-model-hierachy-copy.png)

### 透過共用物件授予權限

當其他用戶共用這些對象並授予這些對象的特定權限時，用戶可以訪問這些對象。

>[!NOTE]
>
>* 如果用戶與某個對象共用某個對象，並且該對象下面有任何子對象，則收件者將繼承這些子對象的相同權限。
>* 如果訪問級別限制用戶刪除某些對象，則這不會阻止用戶刪除這些對象中包含的子對象。


使用者可將下列任何權限授予個別物件：

* **檢視**:此權限層級可讓收件者透過下列其中一種方式共用物件：

   * 系統範圍，以便所有用戶都能看到它（不適用於所有對象）
   * 沒有Workfront授權的外部使用者（不適用於所有物件）
   * 具有電子郵件地址（僅適用於文檔和日曆）

* **Contribute**:（不適用於所有對象）
* **管理**:當某人共用對象時，收件人對對象的權限由收件人的訪問級別和共用人授予的對象權限的組合確定。 該組合中可用的最低訪問程度決定了接收方可以對對象執行什麼操作。

### 範例案例

#### **方案1**

如果收件者的存取層級不允許編輯專案，即使共用者已授予管理專案的權限，該人員仍無法編輯或刪除專案。

或者，如果收件者的存取層級允許編輯專案，但共用者授予專案的僅限檢視權限，則使用者無法編輯或刪除專案。

#### **方案2**

當Olivia與Tony分享一個Workfront專案時，Tony的存取權取決於兩件事的組合：

* Tony的存取層級，由Workfront管理員指派
* Olivia指定的Tony對項目的權限

托尼在項目上的行動可以在項目上受到進一步限制，但除了他的訪問級別允許的以外，這些行動不能不受限制：

* 如果Tony的訪問級別不允許他建立任務，則他無法向項目添加任務，即使Olivia授予他添加任務的權限。
* 如果Tony的訪問級別允許他建立任務，但Olivia沒有授予向項目添加任務的權限，則他無法向該項目添加任務，但他可以將任務添加到已授予其權限的其他項目。
