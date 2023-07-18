---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 建立排程
description: 您可以使用排程來定義使用者的工作週。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Workfront] 以計算時間表和使用者可用性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# 建立排程

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

作為 [!DNL Adobe Workfront] 管理員，您可以使用排程來定義工作週。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Workfront] 以計算時間表和使用者可用性。

如果您的使用者在不同的時區工作，在每個時區建立排程並將其與這些使用者建立關聯，可以確保他們的工作記錄在 [!DNL Workfront] 即時可用，而且可用性一律會根據其運作時間而準確無誤。

如需將排程與使用者和專案建立關聯的資訊，請參閱下列文章：

* [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)

群組管理員也可以建立與所管理群組相關聯的排程。 如需詳細資訊，請參閱 [建立和修改群組的排程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

有關使用排程協助使用者在中共同作業的資訊 [!DNL Workfront] 跨時區，請參閱 [跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

如需如何在資源計畫中使用排程的相關資訊，請參閱 [排程總覽](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) 和 [資源規劃工具概觀](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>：如果您還是無法存取，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需如何進行 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立排程

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 按一下 **[!UICONTROL 時程表]**.
1. 按一下 **[!UICONTROL 新排程]**.
1. 指定排程的名稱。
1. （選用）選取 **[!UICONTROL 預設排程]** 以識別此排程作為預設值。

   您可以在中擁有多個排程 [!DNL Workfront]，但您只能有一個預設排程。

   您必須至少有一個排程於 [!DNL Workfront]. 如果您只有一個排程，則會指定為預設排程。

   >[!NOTE]
   >
   >如果您是群組管理員，就無法指定排程作為預設排程。 僅a [!DNL Workfront] 管理員可以指定排程作為系統的預設值。

   ![](assets/new-schedule.png)

1. 在 **[!UICONTROL 排程]** 索引標籤上，拖曳藍色外框跨小時區塊以反白顯示它們，藉此選取每日排程。

   建議您在9小時的期間內選取8個一小時區塊。 這適合午餐或其他休息時間。

   ![](assets/new-schedule-with-exceptions.png)

1. 於 **[!UICONTROL 詳細資料]** 索引標籤中，指定下列資訊：

   <table style="table-layout:auto">
    <tr>
     <td>具有管理存取權的[！UICONTROL群組]</td>
     <td><p>指出其管理員有權編輯此排程的群組。</p>
     <p><b>重要</b>：</p>
      <ul>
       <li>
       <p>如果您是建立排程的群組管理員，則必須填寫此欄位。</p>
       <p>作為群組管理員，只有在為指定為管理員的群組或子群組指定排程時，您才能建立排程。</p>
       <p>如果您只管理一個群組，預設會在此欄位中選取該群組。</p>
       <p>如果您管理數個群組，則必須先在此欄位中選取群組，才能儲存排程。</p></li>
       <li>如果您是 [!DNL Workfront] 管理員建立排程，此欄位為選用。 當您建立排程而不與群組相關聯時，排程會儲存為系統層級排程，且無法由任何群組的群組管理員管理。
       <p>所有可以編輯這些物件的使用者都可以看到指派給帳戶或專案的排程。 這適用於系統層級和群組層級排程。</p>
       </li>
       <p>為排程指定具有管理存取權的群組不會將排程指派給群組中的使用者；它只允許群組中的群組管理員編輯、刪除和複製排程。</p>
       <p>群組管理員無法編輯、刪除或複製系統層級排程。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>.
     </td>
    </tr>
    <tr>
     <td>具有檢視存取權的[！UICONTROL群組]</td>
     <td><p>選取可看見此排程且具有[！UICONTROL檢視]存取權的群組。</p>
     <p>只有此處指定群組中的使用者在將排程指派給使用者或專案時，才能在下拉式選單中找到排程。</p></tr>
    <tr>
     <td>[！UICONTROL時區]</td>
     <td><p>選取排程的時區。</p>
     <p>如果您將排程與使用者建立關聯，我們建議排程的時區與使用者的時區相符。如需有關使用者時區的資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔。
     </td>
    </tr>
   </table>


1. 於 **[!UICONTROL 例外]** 頁簽，指定排程的例外。

   例外情況為需要從排程中排除的完整或半天，例如假日或公司活動。

   >[!NOTE]
   >
   >如果您已經知道您的週期性排程例外是什麼，您可以定義未來許多年的排程例外。

   可以從工作排程中排除全部或部分天數。 按一下日期，將其選取為例外，然後選取 **[!UICONTROL 全天]** 表示例外是否為全天的欄位。

   ![](assets/schedule-adding-an-all-day-exception.png)

1. 指定部分日例外的開始和結束時間。

   ![partial-day-exception-on-schedules.png](assets/partial-day-exception-on-schedules.png)

1. 按一下 **[!UICONTROL 儲存]**，然後按一下 **[!UICONTROL 儲存] 變更**.

1. （選用）將排程與使用者建立關聯。

   如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. （選用）將排程與專案建立關聯。

   如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).
