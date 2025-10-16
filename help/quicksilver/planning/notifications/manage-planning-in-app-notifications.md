---
title: 管理Adobe Workfront Planning應用程式內通知
description: 當有人在記錄評論中標籤您或您的團隊時，您會收到該標籤的電子郵件通知。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---


# 管理Adobe Workfront Planning應用程式內通知

{{planning-important-intro}}

當存在以下情況時，您可以從Workfront Planning接收應用程式內通知：

* 有人在記錄評論中為您或您的團隊加上標籤

  如需有關在記錄註解中標籤其他人的資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人向您要求存取檢視或工作區的許可權
* 有人確認已授予您檢視或工作區的存取權<!--Isk confirmed there is no notification for denying permissions - did not test-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p> <p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>淺色或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>檢視或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


<!--
OLD:

+++ Expand to view access requirements. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## 當有人在評論中標籤您時管理應用程式內通知

1. （視條件而定）有人在記錄上的評論中為您或您的團隊加上標籤後，請前往Adobe Experience Cloud中的應用程式內&#x200B;**通知**&#x200B;圖示![Experience Cloud通知圖示](assets/experience-cloud-notifications-icon.png)。

   ![應用程式內通知範例](assets/in-app-notification-example.png)

1. 按一下通知。

   記錄詳細資訊頁面會在Workfront Planning中開啟。 您可以更新記錄或回覆註解。

1. （選擇性）按一下&#x200B;**全部標示為已讀取**，表示您已讀取所有通知。
1. （選擇性）按一下「檢視全部&#x200B;**」，移至Adobe Experience Cloud中的**&#x200B;通知&#x200B;**頁面。**

## 請求和授與許可權時管理應用程式內通知

有人要求或授予您檢視或工作區的許可權時，您會收到應用程式內通知。

如需有關要求、授與或拒絕檢視或工作區許可權的資訊，請參閱[要求檢視或工作區的許可權](/help/quicksilver/planning/access/request-permissions.md)。

如需有關管理Workfront Planning通知的資訊，請參閱[管理Adobe Workfront Planning通知偏好設定](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。
