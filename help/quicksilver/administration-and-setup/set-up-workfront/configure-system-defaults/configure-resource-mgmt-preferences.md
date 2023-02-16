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
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 設定 [!UICONTROL 資源管理] 偏好設定

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">本頁強調顯示的資訊指的是尚未普遍提供的功能。 它僅在預覽環境中可用。</span>

作為 [!DNL Adobe Workfront] 管理員 [!UICONTROL 資源管理] 系統的首選項。 這些首選項決定如何計算用戶小時數或FTE可用性或容量 [!DNL Workfront] 資源調度和規劃工具。

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>系統管理員訪問級別</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>附註</b>:

如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 計算使用者容量時考量的資訊

計算使用者容量時，Workfront會考量下列資訊：

* 排程小時數，如使用者的排程或Workfront系統的 [!UICONTROL 預設排程]
* [!UICONTROL 排程] [!UICONTROL 例外] (取決於 [!UICONTROL 排程] ，則可能是使用者排程的例外，或與 [!DNL Workfront] [!UICONTROL 預設排程])
* 用戶休息時間
* 全時等價值([!UICONTROL FTE])或 [!DNL Workfront] 系統。 此 [!UICONTROL FTE] 等於1，當使用者全時運作（如排程中所定義）。
* <span class="preview">的值 [!UICONTROL 工作時間] 指使用者花在專案相關工作上的時間。 這不包括額外費用時間，如會議和培訓。 此 [!UICONTROL 工作時間] 等於1，當使用者可以持續工作時(如 [!UICONTROL FTE] 或者時間表，這意味著他們不會花任何時間在與項目無關的工作上，如會議或培訓。</span>

有關計畫和計畫資源的資訊，請參閱 [!DNL Workfront]，請參閱 [開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## 設定 [!UICONTROL 資源管理] 偏好設定

>[!NOTE]
>
>因為這是全局設定，所以此選擇會影響所有資源管理工具中整個系統（對所有用戶）的所有計算。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 按一下 **[!UICONTROL 資源管理]**.
1. 選取下列其中一種方法，以計算 [!DNL Workfront]:

   * **預設排程**: [!DNL Workfront] 使用系統的預設計畫和用戶的單個FTE來計算資源管理工具中用戶的可用小時數。

      如需排程的詳細資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      如需關於找到使用者 [!UICONTROL FTE]，請參閱  [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront會在Workfront管理員選擇 [!UICONTROL 預設排程]:


      在生產環境中：

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > 例如，若 [!UICONTROL 預設排程] 每週40小時，而 [!UICONTROL FTE] 在使用者的設定檔0.5中，使用者每週可工作20小時。
      >如果使用者一天有1小時的休息時間，其可用小時數的計算方式如下：
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```

      <div class="preview">

      在預覽環境中：

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >例如，如果預設計畫是每週40小時，則用戶配置檔案中的FTE為0.5，用戶有1小時的休息時間，而 [!UICONTROL 工作時間] 在使用者的設定檔中，使用者每週可實際工作9.5小時。
      >
      >如果使用者一天有1小時的休息時間，其可用小時數的計算方式如下：
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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

   * **使用者的排程**: [!DNL Workfront] 使用使用者的排程，以及 [!UICONTROL 預設排程] 計算可用 [!UICONTROL FTE] 資源管理工具中用戶的值。 「可用時數」僅根據使用者的排程計算。 的值 [!UICONTROL FTE] 會忽略。 這是預設設定。

      如需排程的詳細資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      如需使用者的 [!UICONTROL 排程]，請參閱  [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >如果使用者未與排程相關聯，系統只會使用 [!UICONTROL 預設排程].

      在生產環境中：


      使用者的可用小時數依下列公式計算：

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      可用 [!UICONTROL FTE] 使用者的計算公式如下：

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >例如，若 [!UICONTROL 預設排程] 為每週40小時，而使用者的排程為每週30小時，則 [!UICONTROL FTE] 0.70。
      >  
      >如果使用者一天有2小時的休息時間，則可使用每週 [!UICONTROL FTE] 計算方式如下：
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <div class="preview">

      在預覽環境中：

      使用者的可用小時數依下列公式計算：

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      可用 [!UICONTROL FTE] 使用者的計算公式如下：

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >例如，若 [!UICONTROL 預設排程] 每週40小時，使用者的排程是每週30小時，而使用者的 [!UICONTROL 工作時間] 是0.5 [!UICONTROL FTE] 0.35。
      >
      >如果使用者一天有2小時的休息時間，則可使用每週 [!UICONTROL FTE] 計算方式如下：
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
