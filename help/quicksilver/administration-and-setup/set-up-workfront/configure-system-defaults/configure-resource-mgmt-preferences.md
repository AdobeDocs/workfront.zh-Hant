---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置資源管理首選項
description: 作為 [!DNL Adobe Workfront] 管理員可以配置系統的資源管理首選項。 這些資源管理首選項決定了如何計算用戶可用性或容量以及 [!DNL Workfront] 資源調度和規劃工具。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# 設定 [!UICONTROL 資源管理] 偏好設定

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

作為 [!DNL Adobe Workfront] 管理員 [!UICONTROL 資源管理] 系統的首選項。 這些首選項決定如何計算用戶可用性或容量以及 [!DNL Workfront] 資源調度和規劃工具。

有關計畫和計畫資源的資訊，請參閱 [!DNL Workfront]，請參閱 [開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>系統管理員訪問級別</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定 [!UICONTROL 資源管理] 偏好設定

>[!NOTE]
>
>由於這是全局設定，因此此選擇會影響整個系統、所有用戶、所有資源管理工具以及所有資源池的所有計算。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 按一下 **[!UICONTROL 資源管理]**.
1. 選取下列其中一種方法，以計算 [!DNL Workfront]:

   * **預設排程**: [!DNL Workfront] 使用系統的預設計畫和用戶的單個FTE來計算資源管理工具中用戶的可用小時數。\

      如需排程的詳細資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有關用戶FTE值的詳細資訊，請參閱  [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront管理員選擇「預設排程」時，會使用以下公式計算使用者的可用時數：

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **範例:**\
      例如，如果預設計畫每週40小時，用戶配置檔案中的FTE為0.5，則用戶每週可工作20小時。

      如果使用者一天有1小時的休息時間，其可用小時數的計算方式如下：

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

      <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
        <div class="example" data-mc-autonum="<b>Example: </b>">      
        <span class="autonumber"><span><b>Example: </b></span></span>      
        <div>      
        <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
        <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
        <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
        </div>      
        </div></li>      
        -->

   * **使用者的排程**: [!DNL Workfront] 使用用戶的計畫以及系統的預設計畫來計算資源管理工具中用戶的可用FTE值。 「可用時數」僅根據使用者的排程計算。 忽略用戶的FTE值。 這是預設設定。

      >[!NOTE]
      >
      >如果用戶未與某個計畫關聯，則使用預設計畫計算用戶的可用小時數。

      用戶的可用FTE按以下公式計算：

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **範例：** 例如，如果預設計畫是每週40小時，而用戶的計畫是每週30小時，則用戶的FTE為0.75。

      如果用戶有一天有2小時的休假時間，則其每週可用FTE的計算方式如下：

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
