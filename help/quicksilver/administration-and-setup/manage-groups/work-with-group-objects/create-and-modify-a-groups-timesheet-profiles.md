---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和管理群組的時程表設定檔
description: 當您檢視您在「群組」區域中管理的群組時，您可以檢視和處理群組或其子群組的管理員具有管理存取權的時程表設定檔。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 建立和管理群組的時程表設定檔

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

當您檢視您在「群組」區域中管理的群組時，您可以檢視和處理群組或其子群組的管理員具有管理存取權的時程表設定檔。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是群組的群組管理員。</p>  <p>您也必須具有時程表的管理存取權。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予使用者對特定區域的管理存取權</a>。</p>  <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 建立和編輯群組層級週期性時程表

您可以建立和編輯週期性時程表，以便在您管理的群組中使用。 如需指示，請參閱[建立、編輯和指派週期性時程表](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

## 刪除群組層級週期性時程表

您可以刪除您管理的群組正在使用的週期性時程表。 如需指示，請參閱[刪除週期性時程表](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)。

## 手動產生群組時間表

若要啟用您對群組時程表設定檔所做的變更以反映在目前的群組時程表中，您必須先刪除現有時程表，然後手動產生新時程表。 如需指示，請參閱[手動產生時間表](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)中的[從時間表和時數區域](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)手動產生時間表。

如需有關刪除群組時程表的資訊，請參閱[刪除Adobe Workfront中的時程表](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

## 匯出群組層級週期性時程表

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含要匯出之時程表設定檔的群組名稱。
1. 按一下&#x200B;**週期性時程表**。
1. 按一下&#x200B;**匯出**&#x200B;以匯出群組的週期性時程表清單。
