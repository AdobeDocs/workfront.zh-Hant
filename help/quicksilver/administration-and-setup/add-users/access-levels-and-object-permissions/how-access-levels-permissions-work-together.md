---
title: 存取層級和許可權如何搭配運作
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，許可權
navigation-topic: access-levels
description: Adobe Workfront管理員會決定每個使用者應該具有的存取層級。 該存取層級會定義使用者能夠檢視的物件型別以及系統中區域的動作。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 2%

---

# 存取層級和許可權如何搭配運作

Adobe Workfront管理員會決定每個使用者應該具有的存取層級。 該存取層級會定義使用者能夠檢視的物件型別以及系統中區域的動作。

當其他使用者共用並授予這些物件的特定許可權時，使用者也可存取個別物件。


![](assets/security-model-hierachy.png)

例如，如果您的存取層級顯示您可以建立任務，但您收到的特定專案許可權不允許您新增任務，則即使您可以在Workfront的其他位置建立任務，您仍無法在專案上新增任務。

本文說明此組合的運作方式。

## 存取層級

登入Workfront時，需要Workfront管理員指派給每位使用者的存取層級。

預設的存取層級為：

* 系統管理員（附加到計畫授權）
* 計畫者（附加至計畫授權）
* 工作者（附加到工作授權）
* 檢閱者（附加至檢閱授權）
* 請求者（附加到請求授權）
* 外部使用者（附加至外部電子郵件授權）

每個預設存取層級的Workfront授權會決定在存取層級中可用和可設定的專案。 如需Workfront授權的相關資訊，請參閱[Adobe Workfront授權概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

對於指派給該許可權的使用者，存取層級會定義他們在Workfront中可以看見及處理以下物件型別和區域的內容：

* 專案
* 任務
* 問題
* 專案組合
* 報告、儀表板和行事曆
* 篩選器、檢視和群組
* 文件
* 其他使用者
* 範本
* 財務資料
* 資源管理
* 情境規劃工具
* Workfront Goals

在自訂存取層級中，您可以設定這些物件和區域的設定，以變更使用者對它們的存取許可權。 根據與存取層級相關聯的授權以及物件或區域的型別，您可以將存取層級設定為不允許存取、檢視存取或編輯物件或區域的存取權。

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。 若要自訂存取層級，請複製預設存取層級並修改副本。 （除了系統管理員和外部使用者之外，您可以對每個存取層級執行此動作。）

如需每個預設存取層級的詳細說明，請參閱[內建存取層級](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md)。

如需指派存取層級給使用者的指示，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 權限

與系統中的某人共用物件時，使用者可以將下列任何許可權授予收件者給該物件。

* **檢視**：此許可權層級允許收件者以下列其中一種方式共用物件：

   * 系統範圍，讓所有使用者都能看見（不適用於所有物件）
   * 針對沒有Workfront授權的外部使用者（不適用於所有物件）
   * 含電子郵件地址（僅適用於檔案）

* **Contribute**： （不適用於所有物件）
* **管理**：當某人共用物件時，收件者對該物件的許可權是由收件者的存取層級與共用者所授予之物件許可權的組合所決定。 該組合中可用的最低存取度決定了收件者可以對物件執行的操作。

  >[!INFO]
  >
  >**範例：**&#x200B;如果收件者的存取層級不允許編輯專案，即使共用者授予管理專案的許可權，該人員也無法編輯或刪除專案。
  >
  >或者，如果收件者的存取層級允許編輯專案，但共用者授予專案的僅限檢視許可權，則使用者無法編輯或刪除專案。

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
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>由共用物件層級物件的使用者授予</td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>繼承自較高等級的共用物件 
   </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果使用者以特定許可權共用物件，而該物件底下有任何子物件，則收件者會繼承這些子物件的相同許可權。
>* 如果存取層級限制使用者無法刪除某些物件，這不會阻止他們刪除這些物件中包含的子物件。
>

## 更多範例情境

當Olivia與Tony共用Workfront專案時，Tony的存取權取決於兩個因素：

* 由Workfront管理員指派的Tony存取層級
* Tony對專案的許可權，由Olivia指定

Tony在專案上的動作可以在專案上進一步限制，但是不能超出其存取層級所允許的限制：

* 如果Tony的存取層級不允許他建立任務，他無法將任務新增到專案，即使Olivia授予他許可權將任務新增到專案。
* 如果Tony的存取層級允許他建立任務，但Olivia沒有授予將任務新增到專案的許可權，他無法將任務新增到專案，但他可以將任務新增到他已被授予許可權的其他專案。
