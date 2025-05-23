---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 建立排程
description: 您可以使用排程定義使用者的工作週。 您可以將排程與使用者或專案建立關聯。 這可讓 [!DNL Workfront] 計算時間表和使用者可用性。
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 建立排程

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

作為[!DNL Adobe Workfront]管理員，您可以使用排程定義您的工作週。 您可以將排程與使用者或專案建立關聯。 這可讓[!DNL Workfront]計算時間表和使用者可用性。

如果您的使用者在不同時區工作，在每個時區建立排程並將其與這些使用者建立關聯，可以確保他們的工作會即時記錄在[!DNL Workfront]中，而且他們的可用性始終根據其工作時間準確無誤。

如需將排程與使用者和專案建立關聯的資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)和[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

群組管理員也可以建立與所管理群組相關聯的排程。 如需詳細資訊，請參閱[建立和修改群組的排程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)。

如需使用排程協助使用者在[!DNL Workfront]中跨時區共同作業的資訊，請參閱[跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

如需有關如何在資源規劃中使用排程的資訊，請參閱[排程總覽](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)和[資源規劃工具總覽](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[!UICONTROL Standard]</p>
       <p>或</p>
       <p>目前： [!UICONTROL 計畫]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>  
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立排程

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 排程]**。
1. 按一下&#x200B;**[!UICONTROL 新增排程]**。
1. 輸入排程的名稱。
1. （選擇性）選取&#x200B;**[!UICONTROL 預設排程]**&#x200B;以識別此排程為您的預設排程。

   您在[!DNL Workfront]中必須至少有一個排程。 如果您只有排程，則會將其指定為預設排程。

   您可以有多個排程，但只能有一個預設排程。

   >[!NOTE]
   >
   >如果您是群組管理員，則無法指定排程作為預設排程。 只有[!DNL Workfront]管理員可以指定排程作為系統的預設值。

   ![新排程](assets/new-schedule.png)

1. 在&#x200B;**[!UICONTROL 排程]**&#x200B;索引標籤上，將藍色外框拖曳到小時區塊以反白顯示，以選取每日排程。

   我們建議您在9小時內選取8個一小時區塊。 這適合午餐或其他休息時間。

   排程上的![個時間區塊](assets/new-schedule-with-exceptions.png)

1. 在&#x200B;**[!UICONTROL 詳細資料]**&#x200B;標籤上，輸入下列資訊：

   <table style="table-layout:auto">
    <tr>
     <td>具有管理存取權的[!UICONTROL 群組]</td>
     <td><p>選取其管理員有權編輯此排程的群組。</p>
     <p><b>重要</b>：</p>
      <ul>
       <li>
       <p>如果您是建立排程的群組管理員，則此欄位為必要欄位。</p>
       <p>作為群組管理員，只有在為指定為管理員的群組或子群組指定排程時，您才能建立排程。</p>
       <p>如果您只管理一個群組，預設會在此欄位中選取該群組。</p>
       <p>如果您管理數個群組，則必須先在此欄位中選取群組，才能儲存排程。</p></li>
       <li>如果您是建立排程的[!DNL Workfront]管理員，此欄位為選擇性欄位。 當您建立排程而不與群組產生關聯時，排程會儲存為系統層級排程，且無法由任何群組的群組管理員管理。
       <p>所有可編輯這些物件的使用者皆可看見指派給帳戶或專案的排程。 系統層級和群組層級排程皆是如此。</p>
       </li>
       <p>為排程指定具有管理存取權的群組不會將排程指派給群組中的使用者；它只允許群組中的群組管理員編輯、刪除和複製排程。</p>
       <p>群組管理員無法編輯、刪除或複製系統層級排程。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>。
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL 群組具有檢視存取權]</td>
     <td><p>選取具有[!UICONTROL 檢視]存取權的群組，讓他們看到此排程。</p>
     <p>只有此處指定之群組中的使用者在將排程指派給使用者或專案時，才可在下拉式選單中找到排程。</p></tr>
    <tr>
     <td>[!UICONTROL 時區]</td>
     <td><p>選取排程的時區。</p>
     <p>如果您將排程與使用者建立關聯，我們建議排程的時區與使用者的時區相符。 如需使用者時區的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者設定檔。
     </td>
    </tr>
   </table>


1. 在&#x200B;**[!UICONTROL 例外]**&#x200B;索引標籤上，指定排程的任何例外。

   例外情況是需要從排程中排除的完整或半天，例如假日或公司活動。

   >[!NOTE]
   >
   >如果您已經知道您的週期性排程例外是什麼，您可以定義未來許多年的排程例外。

   可以從工作排程中排除全部或部分天數。 按一下日期，將其選取為例外，然後選取&#x200B;**[!UICONTROL 全天]**&#x200B;欄位，以指出例外是否為全天。

   ![全天例外狀況](assets/schedule-adding-an-all-day-exception.png)

1. 輸入部分日例外的開始與結束時間。

   ![部分日例外狀況](assets/partial-day-exception-on-schedules.png)

1. 按一下&#x200B;**[!UICONTROL 儲存]**，然後按一下&#x200B;**[!UICONTROL 儲存]變更**。

1. （選用）將排程與使用者建立關聯。

   如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. （選用）將排程與專案建立關聯。

   如需詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。
