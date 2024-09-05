---
title: 管理Adobe Workfront Planning通知偏好設定
description: 您或許可以管理Adobe Workfront Planning的通知偏好設定。 本文會介紹如何設定您的通知偏好設定。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---


# 管理Adobe Workfront Planning通知偏好設定

{{planning-important-intro}}

Workfront Planning中發生下列動作時，您可能會收到應用程式內或電子郵件通知：

* 有人將您新增至記錄頁面上的註解
* 某人要求存取檢視或工作區的許可權
* 有人授予您存取檢視或工作區<!--I could not test this but Isk confirmed-->的許可權

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具備下列專案才能存取Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront執行個體必須上線至Adobe統一體驗。</p> 
<p>只有當您的組織加入Adobe統一體驗時，您組織中的使用者才會從Workfront Planning接收通知。 </p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p><p>標準、光源或貢獻者
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
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


如需Workfront Planning通知的詳細資訊，另請參閱下列文章：

* 如需有關記錄的註解資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* 如需有關來自Workfront Planning的應用程式內通知的資訊，請參閱[管理Adobe Workfront Planning的應用程式內通知](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)。
* 如需Workfront Planning電子郵件通知的相關資訊，請參閱[管理Adobe Workfront Planning的電子郵件通知](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)。
<!--

OLD: 

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
   <p>In order to receive in-app notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
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
-->

## 管理通知偏好設定

1. 使用您的Adobe Experience Cloud憑證登入Workfront。
1. 按一下熒幕右上角的&#x200B;**帳戶功能表**&#x200B;圖示![](assets/account-menu-icon-on-experience-cloud.png)，然後按一下&#x200B;**偏好設定**。
1. 在&#x200B;**通知**&#x200B;區段下，按一下&#x200B;**Workfront**。
1. 選取您要收到的通知。
或
取消選取您要停止接收的通知。

   ![](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfront提供下列通知：

   * **提及**：當有人在Workfront Planning的評論中為您加上標籤時，您會收到通知
   * **請求**：當有人請求或授予您Workfront規劃物件的許可權時，您會收到通知

   如需有關管理通知的詳細資訊，請參閱[帳戶偏好設定和通知](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences)。

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
