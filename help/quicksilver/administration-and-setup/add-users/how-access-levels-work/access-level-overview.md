---
title: 新存取層級概觀
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，層級，系統，管理員，標準，輕量，參與者
navigation-topic: access-levels
description: 每位使用者都必須具備存取層級，才能登入及在Workfront中工作。 您可以使用存取層級來控制使用者可以檢視特定Workfront物件與區域的內容，以及對這些物件與區域執行的動作。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 681d3b74eec1388f3b6cc7edf51422e0019cc318
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 4%

---

# 新存取層級概觀

身為Adobe Workfront管理員，您可以為使用者指派存取層級，目的有二：

* 每位使用者都必須具備存取層級，才能登入及在Workfront中工作。
* 您可以使用存取層級來控制使用者可以檢視特定Workfront物件與區域的內容，以及對這些物件與區域執行的動作。

## Adobe Workfront中新的內建存取層級 {#built-in-access}

Workfront有5個新的內建存取層級：

* 系統管理員
* 標準
* 精簡
* 貢獻者
* 外部

根據存取層級，大多數Workfront物件型別最多可使用3個許可權：

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

如果您需要自訂存取層級，可以複製內建存取層級，並調整您要允許各種Workfront物件型別的存取量。 如需建立自訂存取層級的詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。

### 系統管理員存取層級

此內建存取層級附加至Standard授權，是專為負責管理Adobe Workfront系統的使用者所設計。 您無法修改此內建存取層級。

具有系統管理員存取層級的使用者可以在Workfront中執行所有操作。 他們可以檢視及編輯所有其他使用者在Workfront中輸入的所有Workfront物件和資訊。

使用者也可存取完整的「設定」區域，在此變更系統層級的任何設定，並可存取主功能表中的所有區域。

如需詳細資訊，請參閱 [授予使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### 標準存取層級

此存取層級也隨附於Standard授權，專為具備以下條件的使用者所設計：

* 在一個地方計畫、建立和追蹤所有專案
* 自動化例行程式
* 管理資源
* 追蹤請求並共同作業
* 追蹤及報告專案財務
* 啟動傳入工作請求
* 針對專案、任務和問題共同作業

>[!NOTE]
>
>您可以建立自訂版本的標準內建存取層級，並調整其允許各種Workfront物件型別的存取量。 如需建立自訂存取層級的詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資料**

以下是「標準」存取層級中物件可用的最高存取設定：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 |   |   | ✓ |
| 任務 |   |   | ✓ |
| 問題 |   |   | ✓ |
| 專案組合 |   |   | ✓ |
| 計劃 |   |   | ✓ |
| 報告（包括儀表板和行事曆報告） |   |   | ✓ |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   |   | ✓ |
| 範本 |   |   | ✓ |
| 財務資料 |   |   | ✓ |
| 資源管理 |   |   | ✓ |
| 案例規劃工具 |   |   | ✓ （預設設定為「無存取權」。） |
| 展示板 |   |   | ✓ |
| 首頁 |   |   | ✓ |
| 目標 |   |   | ✓ |

{style="table-layout:auto"}

### 輕度存取層級

此存取層級附加至輕度授權，是專為具備以下條件的使用者所設計：

* 檢視與工作相關聯的所有專案和更新
* 核准專案、任務和問題
* 檢視控制面板和報表
* 追蹤時間並核準時程表
* 建立和管理問題
* 進行工作更新

具有輕度存取層級的使用者：

* 可以指派工作專案，但無法完成它們。
* 可在主功能表中存取請求和檔案。
* 建立物件的能力有限 — 他們無法建立專案、投資組合、計畫或報告。

>[!NOTE]
>
>您可以建立Light內建存取層級的自訂版本，並調整其允許各種Workfront物件型別的存取量。 如需建立自訂存取層級的詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資料**

以下是「淺層存取」等級中物件可用的最高存取設定：

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
   <td>報告（包括儀表板和行事曆報告）</td> 
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
   <td>✓ （預設設定為「無存取權」。）</td> 
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

### 投稿人存取層級

此存取層級附加於貢獻者授權，專為具備以下條件的使用者所設計：

* 提交請求
* 追蹤請求
* 更新及檢閱請求
* 核准請求

具有此內建存取層級的使用者：

* 可以提出要求並更新這些要求
* 可以上傳和核准檔案
* 可以檢閱他們已提交問題的狀態
* 可指派給工作專案，但無法完成它們
* 只能從主功能表存取請求。 如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>您可以建立「貢獻者」內建存取層級的自訂版本，並調整其允許各種Workfront物件型別的存取量。 如需建立自訂存取層級的詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **存取詳細資料**

以下是投稿人存取層級中物件的最高存取設定：

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 |   | ✓ （僅限專案詳細資訊頁面） |   |
| 任務 |   | ✓ （僅限詳細資訊頁面） |   |
| 問題 |   |   | ✓ |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報告（包括儀表板和行事曆報告） |   | ✓ （僅限詳細資訊標籤） |   |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   | ✓ |   |
| 團隊 |   | ✓ |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| 展示板 |   |   | ✓ （簡單卡片） |
| 首頁 |   | ✓ （我的更新） |   |
| 目標 |   |   | ✓ |

{style="table-layout:auto"}

### 外部使用者存取層級

此存取層級未附加至付費Workfront授權。 這是限制最嚴格的存取層級，主要是為未登入Workfront但偶爾需要檢閱、下載或檢視檔案的外部顧問等共同作業人員所設計。

即使外部使用者無法登入系統，Workfront使用者仍可以將任務指派給外部使用者。 但是我們建議不要這麼做，因為那項工作將在系統中仍未解決。

具有外部使用者存取層級的使用者：

* 只能檢視與其共用的檔案和行事曆報告
* 檢視與他們共用檔案和行事曆報表的使用者
* 核准與其共用的檔案

您無法修改此存取層級。

>[!IMPORTANT]
>
>只有在「設定」的「系統偏好設定」區域中啟用「透過電子郵件地址與沒有Workfront帳戶的人合作」選項時，外部使用者才可用。 如需詳細資訊，請參閱 [設定系統安全性偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **存取詳細資料**

以下是「外部使用者」存取層級中物件的最高存取設定。

| Workfront物件型別 | 無存取權 | 檢視存取權 | 編輯存取權 |
|---|---|---|---|
| 專案 | ✓ |   |   |
| 任務 | ✓ |   |   |
| 問題 | ✓ |   |   |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報告（包括儀表板和行事曆報告） |   | ✓ （僅適用於行事曆報表；無法共用報表） |   |
| 篩選器、檢視和群組 | ✓ |   |   |
| 文件 |   | ✓ （無法共用檔案） |   |
| 使用者 |   | ✓ |   |
| 團隊 | ✓ |   |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| 展示板 | ✓ |   |   |
| 首頁 | ✓ |   |   |
| 目標 | ✓ |   |   |


## 存取層級和許可權如何搭配運作

存取層級會定義使用者在系統中一般物件型別和區域（例如專案、任務和問題）中可以檢視和執行的動作。 許可權會定義您對系統中其他人建立的特定物件（例如為執行行銷活動而建立的專案）的存取權。

下表將使用者對物件的一般存取（由使用者的存取層級定義）與特定共用物件的許可權進行比較：

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
   <td>由Workfront管理員授與使用者存取層級</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>由共用物件層級物件的使用者授予</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>繼承自較高等級的共用物件 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

使用者可以對物件執行的活動由其存取層級和授予他們的許可權組合定義。

![](assets/security-model-hierachy-copy.png)

### 透過共用物件授與許可權

當其他使用者共用並授予這些物件的特定許可權時，使用者可存取個別物件。

>[!NOTE]
>
>* 如果使用者以特定許可權共用物件，而該物件底下有任何子物件，則收件者會繼承這些子物件的相同許可權。
>* 如果存取層級限制使用者無法刪除某些物件，這不會阻止他們刪除這些物件中包含的子物件。

使用者可以將下列任一許可權授與收件者給個別物件：

* **檢視**：此許可權層級可讓收件者透過下列其中一種方式共用物件：

   * 系統範圍，讓所有使用者都能看見（不適用於所有物件）
   * 針對沒有Workfront授權的外部使用者（不適用於所有物件）
   * 含電子郵件地址（僅適用於檔案和行事曆）

* **Contribute**：（不適用於所有物件）
* **管理**：當有人共用物件時，收件者對物件的許可權取決於收件者的存取層級與共用者所授予物件的許可權的組合。 該組合中可用的最低存取度決定了收件者可以對物件執行的操作。

### 範例情境

#### **案例1**

如果收件者的存取層級不允許編輯專案，即使共用者授予管理專案的許可權，該人員也無法編輯或刪除專案。

或者，如果收件者的存取層級允許編輯專案，但共用者授予專案的僅限檢視許可權，則使用者無法編輯或刪除專案。

#### **案例2**

當Olivia與Tony共用Workfront專案時，Tony的存取權取決於兩個因素：

* 由Workfront管理員指派的Tony存取層級
* Tony對專案的許可權，由Olivia指定

Tony在專案上的動作可以在專案上進一步限制，但是不能超出其存取層級所允許的限制：

* 如果Tony的存取層級不允許他建立任務，他無法將任務新增到專案，即使Olivia授予他許可權將任務新增到專案。
* 如果Tony的存取層級允許他建立任務，但Olivia沒有授予將任務新增到專案的許可權，他無法將任務新增到專案，但他可以將任務新增到他已被授予許可權的其他專案。
