---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，權限
navigation-topic: access-levels
title: Adobe Workfront中的內建存取層級
description: 六個內置訪問級別中的每個級別都針對特定類型的用戶而設計，包括系統管理員、計畫員、工作人員、審核者、請求者和外部用戶。 這些存取層級可讓您控制使用者可在系統中編輯和檢視的項目。 如果您需要自訂存取層級，您可以複製e內建存取層級，並決定要其允許的存取量，以用於各種Workfront物件類型。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 5%

---

# Adobe Workfront中的內建存取層級

6個內置訪問級別中的每個級別都是針對特定類型的用戶而設計的：

* 系統管理員
* 計劃者
* 工作者
* 檢閱者
* 要求者
* 外部使用者

根據存取層級，大部分的Workfront物件類型最多可使用3個設定：

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

如果您需要自定義的計畫員、工作人員、請求者或審核者訪問級別，則可以複製內置訪問級別並確定希望它允許各種Workfront對象類型的訪問量。 有關建立自定義訪問級別或修改其中一個內置訪問級別的資訊，請參見 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>強烈建議您將內建存取層級維持不變，以便在設定使用者後參照這些層級。

有關這些訪問級別的一般資訊，請參見 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## 系統管理員訪問級別

此內建存取層級附加至「計畫」授權，專為負責管理Adobe Workfront系統的使用者而設計。 您無法修改此內置訪問級別。

具有系統管理員存取層級的使用者可在Workfront中執行所有作業。 他們可以檢視和編輯所有其他使用者在Workfront中輸入的Workfront物件和資訊。

他們還可以訪問完整的「設定」區域，在該區域可以更改系統級別的任何設定。 他們可以訪問主菜單中的所有區域 ![](assets/main-menu-icon.png).

如需詳細資訊，請參閱 [授予使用者完整的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## 計畫員訪問層

此訪問級別還附於計畫許可證，其設計目的是：

* 群組、團隊、專案和資源的經理
* 負責規劃、建立和管理任務、項目、產品組合和計畫的任何人
* 負責指派工作（任務和問題）給其他使用者的任何人
* 生成報告以及批准工時單、工作項和文檔的用戶
* 需要存取主功能表中所有區域的使用者 ![](assets/main-menu-icon.png)

您可以建立Planner內置訪問級別的自定義版本，並確定它允許的訪問量以用於各種Workfront對象類型。 如需詳細資訊，請參閱 [Adobe Workfront中的內建存取層級](#Customiz) 這篇文章。

以下是「計畫員」訪問級別中對象可用的最高訪問設定：

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
| Workfront 目標 |   |   | ✓（預設設定為「無權存取」）。 |

{style="table-layout:auto"}

## 工作人員訪問級別

此存取層級附加至工作授權，專為在Workfront中執行工作的使用者而設計。 他們沒有規劃工作；他們完成了。

具有此訪問級別的用戶：

* 會指派給可以貢獻和記錄時間的工作項目
* 可以批准工作和文檔，但不能批准時間表
* 可存取和共用報表
* 可以與系統中的其他用戶通信
* 可以訪問主菜單中的所有區域 ![](assets/main-menu-icon.png)，但其「使用者」區域名為「團隊」。 在「團隊」區域中，具有此訪問級別的用戶只能查看他們所屬的團隊以及分配給這些團隊的工作。
* 建立對象的能力有限 — 他們不能建立項目、產品組合、方案或報告。

您可以建立Worker內置訪問級別的自定義版本，並確定它允許的各種Workfront對象類型的訪問量。 如需詳細資訊，請參閱 [Adobe Workfront中的內建存取層級](#Customiz) 這篇文章。

以下是工作器訪問級別中對象可用的最高訪問設定：

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 |   |   | ✓(有限：使用者只能共用專案、建立工作和問題，以及以已附加至專案的自訂表單編輯資料。) |
| 任務 |   |   | ✓ |
| 問題 |   |   | ✓ |
| 專案組合 |   | ✓（預設設定為「無權存取」）。 |   |
| 計劃 |   | ✓（預設設定為「無權存取」）。 |   |
| 報表（包括控制面板和日曆報表） |   | ✓ |   |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   |   | ✓ |
| 範本 | ✓ |   |   |
| 財務資料 |   | ✓(預設設定為「無權存取」。 「查看」設定允許用戶僅查看「項目詳細資訊」中的「財務」區域。) |   |
| 資源管理 |   | ✓ |   |
| 案例規劃工具 |   |   | ✓（預設設定為「無權存取」）。 |
| Workfront 目標 |   |   | ✓（預設設定為「無權存取」）。 |

{style="table-layout:auto"}

## 審核者訪問級別

此訪問級別附加於「審閱」許可證，面向向其他用戶請求工作以及審閱和批准工作的執行官。 這些人員不是專案擁有者或團隊成員，但需要存取Workfront，才能查看其監控的工作項目。

例如，具有此存取層級的利害關係人可登入Workfront，參與持續審核行銷資料、查看工作更新，以及檢閱檔案、核准、報表和日曆。

具有審核者訪問級別的用戶：

* 無法分配工作項或批准時間表
* 可以訪問主菜單中的請求和文檔 ![](assets/main-menu-icon.png).
* 建立對象的能力有限 — 他們不能建立項目、產品組合、方案或報告。

您可以建立Reviewer內建存取層級的自訂版本，並決定各種Workfront物件類型可允許的存取量。 如需詳細資訊，請參閱 [Adobe Workfront中的內建存取層級](#Customiz) 這篇文章。

與「工作人員」訪問級別相比，對項目和任務的限制更大，以下是「審核者」訪問級別中對象可用的最高訪問設定：

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
   <td>✓</td> 
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
   <td>範本</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>財務資料</td> 
   <td> </td> 
   <td> <p>✓(預設設定為「無權存取」。 「查看」設定允許用戶僅查看「項目詳細資訊」中的「財務」區域。)</p> </td> 
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
   <td>Workfront 目標 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓（預設設定為「無權存取」）。</td> 
  </tr> 
 </tbody> 
</table>

## 請求者存取層級

此存取層級附加至「請求」授權，專為在Workfront中提出和接收簡單工作請求的使用者而設計。 依預設，它們會限制在「請求」區域。

例如，使用者可將問題記錄到貴組織的服務台請求佇列。

具有此訪問級別的用戶：

* 可以提出請求並更新這些請求
* 可以上傳和核准檔案
* 可以查看已提交問題的狀態
* 無法分配給工作項
* 只能從主功能表存取請求 ![](assets/main-menu-icon.png). 如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您可以建立Requester內建存取層級的自訂版本，並決定其允許的存取量以用於各種Workfront物件類型。 如需詳細資訊，請參閱 [Adobe Workfront中的內建存取層級](#Customiz) 這篇文章。

以下是「請求者」訪問級別中對象可用的最高訪問設定：

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 |   | ✓（僅限「項目詳細資訊」頁） |   |
| 任務 |   | ✓（僅「詳細資訊」頁） |   |
| 問題 |   |   | ✓ |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報表（包括控制面板和日曆報表） |   | ✓（僅限「詳細資訊」頁面） |   |
| 篩選器、檢視和群組 |   |   | ✓ |
| 文件 |   |   | ✓ |
| 使用者 |   | ✓ |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| Workfront 目標 |   |   | ✓（預設設定為「無權存取」）。 |

{style="table-layout:auto"}

## 外部用戶訪問級別

此存取層級未附加至付費Workfront授權。 這是限制最嚴格的存取層級，主要針對未登入Workfront、但偶爾需要檢閱、下載或檢視檔案的外部顧問等共同作業人員。

Workfront使用者可指派工作給外部使用者，即使外部使用者無法登入系統亦然。 但我們建議不要這樣做，因為這一工作在系統中仍未解決。

具有外部用戶訪問級別的用戶：

* 只能查看與它們共用的文檔和日曆報告
* 查看與他們共用文檔和日曆報告的用戶
* 核准與其共用的檔案

您無法修改此訪問級別。

>[!IMPORTANT]
>
>只有在「設定」的「系統偏好設定」區域中啟用「透過未使用Workfront帳戶之人員的電子郵件地址與其共同作業」選項時，「外部使用者」才可供使用。 如需詳細資訊，請參閱 [配置系統安全首選項](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

以下是「外部用戶」訪問級別中對象可用的最高訪問設定。

| Workfront物件類型 | 無權存取 | 檢視存取 | 編輯存取 |
|---|---|---|---|
| 專案 | ✓ |   |   |
| 任務 | ✓ | ✓ |   |
| 問題 | ✓ |   |   |
| 專案組合 | ✓ |   |   |
| 計劃 | ✓ |   |   |
| 報表（包括控制面板和日曆報表） |   | ✓(僅用於日曆報告；無法共用報表) |   |
| 篩選器、檢視和群組 | ✓ |   |   |
| 文件 |   | ✓（不能共用檔案） |   |
| 使用者 |   | ✓ |   |
| 範本 | ✓ |   |   |
| 財務資料 | ✓ |   |   |
| 資源管理 | ✓ |   |   |
| 案例規劃工具 | ✓ |   |   |
| Workfront 目標 | ✓ |   |   |
