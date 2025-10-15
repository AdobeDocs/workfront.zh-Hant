---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 設定資源管理喜好設定
description: 作為 [!DNL Adobe Workfront] 管理員，您可以設定系統的資源管理喜好設定。 這些「資源管理」偏好設定會決定如何計算 [!DNL Workfront] 資源排程與計畫工具的使用者可用性或產能與FTE。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# 設定[!UICONTROL 資源管理]偏好設定

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

作為[!DNL Adobe Workfront]管理員，您可以設定系統的[!UICONTROL 資源管理]偏好設定。 這些偏好設定決定如何計算[!DNL Workfront]資源排程與計畫工具的使用者小時或FTE可用性或產能。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
       <p>[！UICONTROL計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 計算使用者的容量時考慮的資訊

計算使用者的容量時，Workfront會考量下列資訊：

* 排程的時數，如使用者的排程或Workfront系統的預設排程中所定義。
* 排程例外(視使用的排程而定，可能是使用者排程的例外，或是與Workfront預設排程相關的例外)。
* 使用者的休假。
* 使用者或[!UICONTROL 系統之全時相當值(]FTE[!DNL Workfront])的值。 如排程中所定義，使用者全職工作時，[!UICONTROL FTE]等於1。
* 使用者的[!UICONTROL 工作時間]值，代表使用者花費在專案相關工作的時間。 這不包括管理時間，例如會議和訓練。 當[!UICONTROL 工作時間]等於1，當使用者可以工作整個時間（如[!UICONTROL FTE]或排程所示）時，這表示他們不會花費任何時間在會議或訓練等與專案無關的工作上。


如需[!DNL Workfront]中計畫與排程資源的相關資訊，請參閱[開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。


## 設定[!UICONTROL 資源管理]偏好設定

>[!NOTE]
>
>因為這是全域設定，所以這個選擇會影響所有資源管理工具中整個系統、所有使用者的所有計算。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 資源管理]**。
1. 選取下列其中一個方法，以計算[!DNL Workfront]中使用者的可用性：

   * **預設排程**： [!DNL Workfront]會使用系統的預設排程和使用者的個別FTE，來計算使用者在資源管理工具中的可用時數。

     如需詳細資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)和[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     選取此選項時，Workfront會使用下列公式計算使用者的「可用時數」：


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >例如，如果預設排程是一週40小時，使用者設定檔中的FTE為0.5，使用者一天有1小時的休假，而使用者設定檔中的[!UICONTROL 工作時間]為0.5，且使用者每週可實際進行9.5小時的專案工作。
     >
     >如果使用者有一天的1小時休假，其「可用時數」的計算如下：
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



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

   * **使用者的排程**： [!DNL Workfront]會使用使用者的排程以及系統的[!UICONTROL 預設排程]，來計算資源管理工具中使用者的可用[!UICONTROL FTE]值。 可用時數只會根據使用者的排程進行計算，而會忽略使用者的[!UICONTROL FTE]的值。 這是預設設定。

     如需詳細資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)和[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     >[!NOTE]
     >
     >如果使用者未與排程關聯，則只會使用[!UICONTROL 預設排程]計算使用者的可用時數。

     使用者的可用時數計算公式如下：


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     使用者的可用[!UICONTROL FTE]由下列公式計算：


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >例如，如果[!UICONTROL 預設排程]是一週40小時，使用者的排程是一週30小時，使用者的[!UICONTROL 工作時間]是0.5，使用者的[!UICONTROL FTE]是0.35。
     >
     >如果使用者一天有2小時的休假，其每週可用的[!UICONTROL FTE]的計算方式如下：
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. 按一下「**[!UICONTROL 儲存]**」。
