---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 建立排程
description: 您可以使用排程來定義使用者的工作周。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Workfront] 計算時間表和用戶可用性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 建立排程

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

作為 [!DNL Adobe Workfront] 管理員，您可以使用排程來定義工作周。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Workfront] 計算時間表和用戶可用性。

當您的使用者在不同時區工作時，請在每個時區中建立排程，並將其與這些使用者建立關聯，以確保其工作記錄在 [!DNL Workfront] 即時性，而且其可用性始終根據其工作時間而準確。

如需將排程與使用者和專案相關聯的詳細資訊，請參閱下列文章：

* [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)

群組管理員也可以建立與其管理之群組相關聯的排程。 如需詳細資訊，請參閱 [建立和修改群組的排程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

有關使用計畫幫助用戶協作的資訊 [!DNL Workfront] 跨時區，請參閱 [跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立排程

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 按一下 **[!UICONTROL 排程]**.
1. 按一下 **[!UICONTROL 新排程]**.
1. 指定排程的名稱。
1. （選用）選取 **[!UICONTROL 預設排程]** 以將此排程識別為預設。

   您可以在 [!DNL Workfront]，但您只能有一個預設排程。

   您至少必須有一個 [!DNL Workfront]. 如果您只有一個，則會指定為預設排程。

   >[!NOTE]
   >
   >如果您是組管理員，則不能將某個計畫指定為預設計畫。 僅a [!DNL Workfront] 管理員可以將某個計畫指定為系統的預設計畫。

   ![](assets/new-schedule.png)

1. 在 **[!UICONTROL 排程]** 頁簽，將藍色大綱拖曳到各個小時區塊以反白顯示，以選擇每日計畫。

   建議您在9小時內選取8個1小時的區塊。 這可供午餐或其他休息時間使用。

   ![](assets/new-schedule-with-exceptions.png)

1. 在 **[!UICONTROL 詳細資料]** 頁簽，指定以下資訊：

   <table style="table-layout:auto">
    <tr>
     <td>[！具有管理訪問權限的UICONTROL組]</td>
     <td><p>指定其管理員有權編輯此排程的群組。</p>
     <p><b>重要</b>:</p>
      <ul>
       <li>
       <p>如果您是建立排程的群組管理員，此欄位為必填欄位。</p>
       <p>作為組管理員，僅當為指定為管理員的組或子組指定調度時，才可建立調度。</p>
       <p>如果您只管理一個群組，依預設會在此欄位中選取該群組。</p>
       <p>如果您管理多個群組，必須在此欄位中選取群組，才能儲存排程。</p></li>
       <li>如果您是 [!DNL Workfront] 管理員建立排程時，此欄位為選填欄位。 在建立調度而未將其與組關聯時，該調度將另存為系統級調度，並且不能由任何組的組管理員管理。
       <p>分配給帳戶或項目的計畫對所有可以編輯這些對象的用戶都可見。 系統層級和群組層級排程均是如此。</p>
       </li>
       <p>為排程指定具有管理存取權的群組時，不會將排程指派給群組中的使用者；它只允許群組中的群組管理員編輯、刪除和複製排程。</p>
       <p>組管理員無法編輯、刪除或複製系統級計畫。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL具有視圖訪問的組]</td>
     <td><p>選擇具有[!UICONTROL視圖]訪問權限的組，此計畫對其可見。</p>
     <p>當指定給使用者或專案時，只有在此指定的群組中的使用者才能在下拉式功能表中找到排程。</p></tr>
    <tr>
     <td>[!UICONTROL時區]</td>
     <td><p>選取排程的時區。</p>
     <p>如果將調度與用戶關聯，我們建議調度的時區與用戶的時區匹配。有關用戶時區的資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔。
     </td>
    </tr>
   </table>


1. 在 **[!UICONTROL 例外]** 頁簽，指定排程的例外。

   例外是需要從排程中排除的全天或半天，例如假日或公司事件。

   >[!NOTE]
   >
   >如果您已知道重複計畫例外是什麼，則可以定義未來許多年的計畫例外。

   可以從工作排程中排除完整或部分天數。 按一下日期以選取例外，然後選取 **[!UICONTROL 全天]** 欄位，指出例外是否為一整天。

   ![](assets/schedule-adding-an-all-day-exception.png)

1. 指定部分日例外的開始和結束時間。

   ![partial-day-exception-on-schedules.png](assets/partial-day-exception-on-schedules.png)

1. 按一下 **[!UICONTROL 儲存]**，然後按一下 **[!UICONTROL 儲存] 變更**.

1. （選用）將排程與使用者關聯。

   如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. （選用）將排程與專案關聯。

   如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).
