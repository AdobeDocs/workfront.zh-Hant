---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 手動生成工時單
description: 要啟用對工時單配置檔案所做的更改以反映在當前工時單中，必須先刪除現有工時單，然後手動生成新工時單。 您可以按照本文所述，從「時間表」(Timesheets)區域或「設定」(Setup)中的「診斷」(Diagnostics)區域手動生成時間表。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 手動生成工時單

要啟用對工時單配置檔案所做的更改以反映在當前工時單中，必須先刪除現有工時單，然後手動生成新工時單。 您可以按照本文所述，從「時間表」(Timesheets)區域或「設定」(Setup)中的「診斷」(Diagnostics)區域手動生成時間表。

有關刪除工時單的說明，請參閱 [刪除Adobe Workfront中的工時單](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是Workfront管理員，或者，如果您正在處理組的時間表配置檔案，則必須是組管理員(或Workfront管理員)。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>.</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於手動生成工時單的注意事項

手動生成工時單時：

* 它們根據與用戶關聯的時間表配置檔案生成。 沒有與其關聯的時間表配置檔案的用戶不會收到時間表。 
* 只生成當前時間表和後續時間表。 Workfront不會為同一期間產生兩個工作表。 如果您已有特定時間範圍的時間表，則使用手動流程生成時間表時，將不會生成另一個時間表。

## 從「工時單和工時」區域手動生成工時單

您可以從「設定」中的「工時單和小時」區域手動生成系統級或組級工時單。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 如果要生成整個系統使用的工時單，請按一下 **工時單和小時數。**

   或

   如果要生成特定組使用的工時單，請按一下 **群組**，然後按一下群組的名稱。

1. 按一下 **時間表配置檔案**.
1. 按一下 **更多**，然後 **生成工時單**.

   為與時間表配置檔案關聯的用戶建立最多兩個時間期的新時間表。

## 從診斷區手動生成系統級時間表

您可以從「設定」中的「診斷」區域手動生成系統級時間表。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **系統**，然後按一下 **診斷**.

1. 按一下 **進行診斷**. 
1. 按一下 **生成工時單**.
