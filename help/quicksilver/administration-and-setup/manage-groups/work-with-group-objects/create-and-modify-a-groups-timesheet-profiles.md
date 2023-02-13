---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和管理組的時間表配置檔案
description: 在「組」區域中查看管理的組時，可以查看並使用該組的管理員或其子組具有管理訪問權限的時間表配置檔案。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 建立和管理組的時間表配置檔案

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

在「組」區域中查看管理的組時，可以查看並使用該組的管理員或其子組具有管理訪問權限的時間表配置檔案。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是群組的群組管理員。</p>  <p>您還必須具有對工時單的管理訪問權限。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用戶對特定區域的管理訪問權限</a>.</p>  <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立和編輯組級時間表配置檔案

您可以建立和編輯工時單配置檔案以用於您管理的組中。 如需指示，請參閱 [建立、編輯和分配工時單配置檔案](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 刪除組級時間表配置檔案

您可以刪除管理的組正在使用的時間表配置檔案。 如需指示，請參閱 [刪除工時單配置檔案](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## 手動生成組工時單

要啟用對組時間表配置檔案所做的更改以反映在當前組時間表中，必須先刪除現有時間表，然後手動生成新時間表。 如需指示，請參閱 [從「工時單和工時」區域手動生成工時單](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [手動生成工時單](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

有關刪除組時間表的資訊，請參閱 [刪除Adobe Workfront中的工時單](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 導出組級時間表配置檔案

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 按一下 **群組**.

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 按一下組的名稱，並包含要導出的時間表配置檔案。
1. 按一下 **時間表配置檔案**.
1. 按一下 **匯出** 導出組的時間表配置檔案清單。
