---
title: 管理Adobe Workfront Planning應用程式內通知
description: 當有人在記錄評論中標籤您或您的團隊時，您會收到該標籤的電子郵件通知。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 1%

---


# 管理Adobe Workfront Planning應用程式內通知

{{planning-important-intro}}

當存在以下情況時，您可以從Workfront Planning接收應用程式內通知：

* 有人在記錄評論中為您或您的團隊加上標籤

  如需有關在記錄註解中標籤其他人的資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人向您要求存取檢視或工作區的許可權
* 有人確認已授予您檢視或工作區的存取權<!--Isk confirmed there is no notification for denying permissions - did not test-->

## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront執行個體必須上線至Adobe統一體驗。</p> 
<p>只有當您的組織加入Adobe Unified Experience時，您組織中的使用者才會收到來自Workfront Planning的通知。 </p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準、光源或貢獻者</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>檢視或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
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
