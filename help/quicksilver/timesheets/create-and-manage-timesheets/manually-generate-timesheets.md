---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 手動產生時間表
description: 若要啟用您對時程表設定檔所做的變更以反映在目前的時程表中，您必須先刪除現有的時程表，然後手動產生新時程表。 您可以從時程表區域或設定中的診斷區域手動產生時程表，如本文所述。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 手動產生時間表

若要啟用您對時程表設定檔所做的變更以反映在目前的時程表中，您必須先刪除現有的時程表，然後手動產生新時程表。 您可以從時程表區域或設定中的診斷區域手動產生時程表，如本文所述。

如需刪除時程表的指示，請參閱[刪除Adobe Workfront中的時程表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是Workfront管理員，或者，如果您正在處理群組的時程表設定檔，您必須是群組管理員(或Workfront管理員)。 如需詳細資訊，請參閱<a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>。</p> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 關於手動產生時程表的考量事項

當您手動產生時程表時：

* 會根據與使用者相關聯的時程表設定檔來產生。 沒有相關時間表設定檔的使用者不會收到時間表。 
* 系統只會產生目前的時程表及要追蹤的時程表。 Workfront不會為同一期間產生兩個時程表。 如果您已經有特定時間範圍的時程表，則當您使用手動程式來產生時程表時，將不會產生另一個時程表。

## 從時程表和時數區域手動產生時程表

您可以從設定的時程表和時數區域手動產生系統或群組層級時程表。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 如果您產生的時程表正在整個系統中使用，請按一下&#x200B;**時程表和時數。**

   或

   如果您正在產生特定群組使用的時程表，請按一下&#x200B;**群組**，然後按一下群組的名稱。

1. 按一下&#x200B;**週期性時程表**。
1. 按一下&#x200B;**更多**，然後&#x200B;**產生時程表**。

   新時程表最多可為與時程表設定檔相關聯的使用者建立兩個時段。

## 從診斷區域手動產生系統層級時間表

您可以從「設定」的「診斷」區域手動產生系統層級時間表。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 展開&#x200B;**系統**，然後按一下&#x200B;**診斷**。

1. 按一下&#x200B;**執行診斷**。 
1. 按一下&#x200B;**產生時程表**。
