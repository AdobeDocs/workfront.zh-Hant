---
title: 存取層級與權限如何搭配運作
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，權限
navigation-topic: access-levels
description: Adobe Workfront管理員會決定每個使用者應具有的存取層級。 該訪問級別定義了用戶可以查看和處理系統中的對象類型和區域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# 舊版存取層級和權限如何搭配運作

Adobe Workfront管理員會決定每個使用者應具有的存取層級。 該訪問級別定義了用戶可以查看和處理系統中的對象類型和區域。

此外，當其他用戶共用並授予這些對象的特定權限時，用戶可以訪問各個對象。

因此，使用者可以對物件執行的活動是由其存取層級與針對該專案授予其權限的組合所定義。

![](assets/security-model-hierachy.png)

例如，如果您的存取層級指出您可以建立工作，但您在特定專案上獲得的權限不允許您新增工作，則即使您可以在Workfront中的其他位置建立工作，也無法新增專案上的工作。

本文說明此組合的運作方式。

## 舊版存取層級

登入Workfront需要Workfront管理員指派給每位使用者的存取層級。

預設的舊版存取層級為：

* 系統管理員（附於計畫許可證）
* 計畫員（附於計畫許可證）
* 工作人員（附於工作許可證）
* 審閱者（附於審閱許可證）
* 請求者（附加至請求授權）
* 外部用戶（附加到外部電子郵件許可）

每個預設存取層級的Workfront授權會決定哪些是可在存取層級中使用和設定。 如需Workfront授權的相關資訊，請參閱 [Adobe Workfront授權概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

對於指派給此物件的使用者，存取層級會定義他們可以查看的項目，以及如何處理Workfront中的下列物件類型和區域：

* 專案
* 任務
* 問題
* 專案組合
* 報表、控制面板和日曆
* 篩選器、檢視和群組
* 文件
* 其他使用者
* 範本
* 財務資料
* 資源管理
* 案例規劃工具
* Workfront 目標

在自定義訪問級別中，您可以配置這些對象和區域的設定，以更改用戶對這些對象和區域的訪問量。 根據與訪問級別相關聯的許可以及對象或區域的類型，您可以配置訪問級別以允許不訪問、查看訪問或編輯對對象或區域的訪問。

>[!IMPORTANT]
>
>強烈建議您將內建存取層級維持不變，以便在設定使用者後參照這些層級。 要自定義訪問級別，請複製預設訪問級別並修改副本。 （除了「系統管理員」和「外部用戶」之外，您可以對每個訪問級別執行此操作。）

有關每個預設訪問級別的詳細說明，請參見 [Adobe Workfront中的內建存取層級](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

有關為用戶分配訪問級別的說明，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 權限

與系統中的某人共用物件時，使用者可向收件者授予該物件下列任何權限。

* **檢視**:此權限層級可讓收件者透過下列其中一種方式共用物件：

   * 系統範圍，以便所有用戶都能看到它（不適用於所有對象）
   * 沒有Workfront授權的外部使用者（不適用於所有物件）
   * 具有電子郵件地址（僅適用於文檔）

* **Contribute**:（不適用於所有對象）
* **管理**:當某人共用對象時，收件人對對象的權限由收件人的訪問級別和共用人授予的對象權限的組合確定。 該組合中可用的最低訪問程度決定了接收方可以對對象執行什麼操作。

   >[!INFO]
   >
   >**範例：** 如果收件者的存取層級不允許編輯專案，即使共用者已授予管理專案的權限，該人員仍無法編輯或刪除專案。
   >
   >或者，如果收件者的存取層級允許編輯專案，但共用者授予專案的僅限檢視權限，則使用者無法編輯或刪除專案。

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

>[!NOTE]
>
>* 如果用戶與某個對象共用某個對象，並且該對象下面有任何子對象，則收件者將繼承這些子對象的相同權限。
>* 如果訪問級別限制用戶刪除某些對象，則這不會阻止用戶刪除這些對象中包含的子對象。
>


## 更多範例案例

當Olivia與Tony分享一個Workfront專案時，Tony的存取權取決於兩件事的組合：

* Tony的存取層級，由Workfront管理員指派
* Olivia指定的Tony對項目的權限

托尼在項目上的行動可以在項目上受到進一步限制，但除了他的訪問級別允許的以外，這些行動不能不受限制：

* 如果Tony的訪問級別不允許他建立任務，則他無法向項目添加任務，即使Olivia授予他添加任務的權限。
* 如果Tony的訪問級別允許他建立任務，但Olivia沒有授予向項目添加任務的權限，則他無法向該項目添加任務，但他可以將任務添加到已授予其權限的其他項目。
