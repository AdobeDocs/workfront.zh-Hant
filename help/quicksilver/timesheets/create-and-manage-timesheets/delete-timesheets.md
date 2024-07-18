---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 刪除Adobe Workfront中的時間表
description: 您對時程表設定檔進行的變更對目前現有時程表而言立即無效，如建立、編輯和指派時程表設定檔中所述。 若要讓變更顯示在現有的時程表中，您必須刪除已產生的時程表並產生新時程表。 這僅適用於將時間表設定檔與使用者建立關聯所產生的時程表。
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 刪除Adobe Workfront中的時間表

您對時程表設定檔進行的變更對目前現有時程表而言立即無效，如[建立、編輯和指派時程表設定檔](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中所述。 若要讓變更顯示在現有的時程表中，您必須刪除已產生的時程表並產生新時程表。 這僅適用於將時間表設定檔與使用者建立關聯所產生的時程表。

>[!NOTE]
>
>無法透過重新產生時程表來重新建立手動建立的時程表，除非使用者在時程表手動建立後已與時程表設定檔相關聯。 刪除手動建立的時程表可能會導致資料遺失。 如需建立單一時程表的詳細資訊，請參閱[建立單一使用時程表](../../timesheets/create-and-manage-timesheets/create-tmshts.md)。

Adobe Workfront管理員或群組管理員可以為系統中的每個人產生時程表。 如需手動產生時程表的詳細資訊，請參閱：

* [手動產生時間表](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [建立和管理群組的時程表設定檔](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 您無法復原已刪除的時程表。
>* 我們建議您不要刪除過去的時程表，因為這些時程表不會根據時程表設定檔自動產生。 如果您希望時程表設定檔的變更立即顯示在新時程表中，可以刪除目前和未來的時程表，並手動產生它們。
>* 當您刪除時程表時，不會刪除針對任務、問題和專案記錄的小時。 只有一般時數會隨時程表一起刪除。 在獨立的文字編輯器中，寫下與時程表關聯的一般時數。 刪除時程表後，您就可以將它們記錄在新時程表中。
>

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
   <td> <p>您必須擁有時程表的管理存取權。 </p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>。</p> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 刪除清單中的時程表

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**時程表**。 依預設會選取&#x200B;**全部**&#x200B;篩選器，且篩選器會顯示您有權檢視的所有時程表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下「篩選」圖示![](assets/filter-nwepng.png)以套用不同的篩選，或建立新的篩選。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （選擇性）按一下&#x200B;**檢視** ![](assets/view-icon.png)或&#x200B;**群組** ![](assets/grouping.png)圖示以套用不同的檢視或群組或建立新的檢視或群組。

   如需有關建立篩選器、檢視或群組的資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取一或多個您要刪除的時程表，然後按一下時程表清單頂端的&#x200B;**刪除** ![](assets/delete.png)圖示。

1. 按一下&#x200B;**刪除**。

   所選的時程表已刪除且無法復原。

   若要產生新時程表，請確保使用者與時程表設定檔相關聯，並要求Workfront管理員或群組管理員產生新時程表。

   如需詳細資訊，請參閱下列內容：

   * [建立、編輯和指派週期性時程表](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [手動產生時程表](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [建立和管理群組的時程表設定檔](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## 從時程表頁面刪除時程表

1. 按一下Adobe Workfront右上角的&#x200B;[!UICONTROL **主要功能表**]&#x200B;圖示![](assets/main-menu-icon.png)。
1. 按一下您要刪除的時程表以開啟它。
1. 按一下時程表名稱右側的&#x200B;[!UICONTROL **更多**]&#x200B;圖示![](assets/more-icon.png)，然後按一下&#x200B;**刪除**。

   ![從時程表頁面](assets/delete-timesheet-from-timesheet-page.png)刪除時程表
1. 按一下&#x200B;[!UICONTROL **刪除**]&#x200B;確認。

   時程表已刪除且無法復原。
