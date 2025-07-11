---
title: 管理Adobe Workfront Planning電子郵件通知
description: 當有人在Adobe Workfront Planning的記錄評論中為您或您的團隊加標籤時，您會收到該標籤的電子郵件通知。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---


# 管理Adobe Workfront Planning電子郵件通知

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

當存在以下情況時，您可以從Workfront Planning接收電子郵件通知：

* 有人在記錄評論中為您或您的團隊加上標籤

  如需有關在記錄註解中標籤其他人的資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人向您要求存取檢視或工作區的許可權
* 有人確認已授予您檢視或工作區的存取權<!--Isk confirmed that there is nno email for denying access but did not test-->
* 您提交Workfront Planning請求。 如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)
* 某人核准或拒絕您提交的Workfront Planning請求。 如需詳細資訊，請參閱[在Adobe Workfront Planning中核准請求](/help/quicksilver/planning/requests/approve-request.md)
* 狀態會變更為您提交的Workfront Planning請求。

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
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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


## 當有人在評論中標籤您時管理電子郵件通知

1. （有條件且選用）在記錄中某人為您或團隊加入評論後，請移至通知您標籤和評論的電子郵件通知。 電子郵件的寄件者為Adobe Experience Cloud。

   ![電子郵件通知範例](assets/email-notification-example.png)

1. （選擇性）按一下電子郵件內&#x200B;**Workfront**&#x200B;方塊中的訊息。

   記錄詳細資訊頁面會在Workfront中開啟。 您可以更新記錄或回覆註解。

1. （視條件而定）如果可用，請按一下&#x200B;**檢視所有通知**。 <!--check with Lilit - do non-IMS users have this button??-->
**通知**&#x200B;頁面會在Adobe Experience Cloud中開啟。 會顯示所有Adobe Experience Cloud應用程式的所有通知。

## 請求和授與許可權時管理電子郵件通知

1. （有條件且選用）某人要求或授予您存取檢視或工作區的許可權後，請前往通知您許可權要求的電子郵件。 電子郵件的寄件者為Adobe Experience Cloud。

1. （選擇性）按一下電子郵件內&#x200B;**Workfront**&#x200B;方塊中的訊息。

   記錄詳細資訊頁面會在Workfront中開啟。 您可以更新記錄或回覆註解。

1. （視條件而定）如果可用，請按一下&#x200B;**檢視所有通知**。
**通知**&#x200B;頁面會在Adobe Experience Cloud中開啟。 會顯示所有Adobe Experience Cloud應用程式的所有通知。


如需有關要求、授與或拒絕檢視或工作區許可權的資訊，請參閱[要求檢視或工作區的許可權](/help/quicksilver/planning/access/request-permissions.md)。

如需有關管理Workfront Planning通知的資訊，請參閱[管理Adobe Workfront Planning通知偏好設定](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。

## 管理有關提交、核准或拒絕Workfront Planning請求的電子郵件通知

1. （選用）前往Workfront傳送給您的電子郵件
在您提交請求之後，或您提交的請求已核准或拒絕之後。 電子郵件的寄件者為Adobe Workfront。

1. （選擇性）按一下&#x200B;**開啟請求**。 這會在Workfront Planning中開啟請求。

1. 按一下畫面右上角的&#x200B;**通知**&#x200B;圖示![通知區域圖示Unified Shell](assets/notifications-area-icon-unified-shell.png)以存取&#x200B;**通知**&#x200B;頁面。

   如需有關管理Workfront Planning通知的資訊，請參閱[管理Adobe Workfront Planning通知偏好設定](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。
