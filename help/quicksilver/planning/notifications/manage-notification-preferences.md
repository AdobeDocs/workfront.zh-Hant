---
title: 管理Adobe Workfront Planning通知偏好設定
description: 您或許可以管理Adobe Workfront Planning的通知偏好設定。 本文會介紹如何設定您的通知偏好設定。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/C3hvRU9XvH3yqP21zXa4mxH6NrST85Jz98AvqeEHNY4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 4%

---

# 管理Adobe Workfront Planning通知偏好設定

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

本文會說明如何管理Adobe Workfront Planning通知，而是一般管理Adobe Workfront通知。

Workfront Planning中發生下列動作時，您可能會收到應用程式內或電子郵件通知：

* 有人將您或您的團隊新增到記錄頁面上的註解
* 有人要求存取檢視或工作區<!--or <span class="preview">or a record</span>-->的許可權
* 有人授予您存取檢視或工作區<!--or <span class="preview">or a record</span> I could not test this but Isk confirmed-->的許可權
* 您提交Workfront Planning請求。
* 某人核准或拒絕您提交的Workfront Planning請求。
* 狀態會變更為您提交的Workfront Planning請求。

您可以從Workfront Planning活動接收及管理下列型別的通知：

* 應用程式內
* 電子郵件

## 存取權要求


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
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
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
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--
Old:
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
   <td><p><p>Standard, Light, or Contributor
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table>
-->

如需Workfront Planning通知的詳細資訊，另請參閱下列文章：

* 如需有關記錄的註解資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* 如需核准通知的相關資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中核准請求](/help/quicksilver/planning/requests/approve-request.md)
   * [提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)
* 如需有關來自Workfront Planning的應用程式內通知的資訊，請參閱[管理Adobe Workfront Planning的應用程式內通知](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)。
* 如需Workfront Planning電子郵件通知的相關資訊，請參閱[管理Adobe Workfront Planning的電子郵件通知](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)。


## 管理通知偏好設定

>[!NOTE]
>
>您可以使用Workfront偏好設定區域管理Adobe計畫通知，而不是使用使用者設定檔頁面上的Workfront通知區域。

1. 使用您的Adobe Experience Cloud憑證登入Workfront 。
1. 按一下畫面右上角的Experience Cloud![&#128279;](assets/account-menu-icon-on-experience-cloud.png)上的&#x200B;**帳戶功能表**&#x200B;圖示帳戶功能表圖示，然後按一下&#x200B;**偏好設定**。
1. 在&#x200B;**通知**&#x200B;區段下，按一下&#x200B;**Workfront**。
1. 選取您要收到的通知。
或
取消選取您要停止接收的通知。

   適用於Workfront Planning的![Adobe Experience Cloud通知面板](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfront提供下列通知：

   * **核准**：當有人提交計畫請求以進行核准，或想要向您請求計畫物件的存取權時，您會收到通知。
   * **提及**：當有人在Workfront Planning的評論中為您或您的團隊加標籤時，您會收到通知
   * **要求**：當某人執行下列其中一項作業時，您會收到通知：

      * 要求或授予Workfront Planning物件的許可權
      * 您已提交Workfront規劃請求
      * 您提交變更的Workfront Planning請求狀態
      * 請求、授予或拒絕對Workfront Planning請求的核准

   如需有關管理通知的詳細資訊，請參閱[帳戶偏好設定和通知](https://experienceleague.adobe.com/zh-hant/docs/core-services/interface/features/account-preferences)。

<!--
OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
