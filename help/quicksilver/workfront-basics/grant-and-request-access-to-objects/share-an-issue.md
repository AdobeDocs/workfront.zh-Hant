---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共用問題
description: 您的Adobe Workfront管理員會授予使用者在指派存取層級時，可檢視或編輯問題的存取權。 有關授予對問題的訪問權限的詳細資訊，請參閱授予對問題的訪問權限。
author: Alina
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 4%

---

# 共用問題

您的Adobe Workfront管理員會授予使用者在指派存取層級時，可檢視或編輯問題的存取權。 如需授與問題存取權的詳細資訊，請參閱 [授予問題的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

除了授予使用者的存取層級之外，您也可以授予使用者檢視、貢獻或管理您有權存取之特定問題的權限。 如需存取層級和權限的詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

權限是Workfront中一個項目專屬的權限，並定義可對該項目採取的動作。

## 共用問題的考量事項

除了下列考量事項外，另請參閱 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理員可以為所有使用者新增或移除系統中任何項目的權限，而不是這些項目的擁有者。

* 問題的建立者預設具有「管理」權限。
* 您可以個別分享問題，也可以一次分享其中幾個問題。 共用問題與在Workfront中共用其他項目相同。 如需在Workfront中共用項目的詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* 您可以授予問題下列權限： 

   * 檢視

      ![view_on_issue.png](assets/view-on-issue-221x216.png)

   * 管理

      ![manage_on_issues.png](assets/manage-on-issues-179x199.png)

   * 參與\
      ![contribute_on_issue.png](assets/contribute-on-issue-156x205.png)

* 當您共用問題時，所有附加至問題的檔案都會繼承相同的權限。

   Workfront管理員可以指定文檔是否應繼承用戶訪問級別較高對象的權限。 有關限制對文檔繼承的權限的詳細資訊，請參見 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 您可以從問題中移除繼承的權限。 如需詳細資訊，請參閱 [從對象中刪除權限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 共用問題的方式

* 手動，類似於在Workfront中共用任何其他物件。 如需如何在Workfront中共用物件的詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* 自動執行下列任一操作：

   * 指定問題任何父對象的權限：專案、方案或產品組合。 問題會繼承其父對象的權限。 有關查看對象繼承的權限的資訊，請參見 [查看對象的繼承權限](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * 在用於建立問題所在專案的範本上，將實體新增至專案共用。 如需從範本共用專案的相關資訊，請參閱 [共用範本](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * 在編輯專案時，指定專案中所有問題的權限。 如需根據使用者對專案的權限管理專案上問題或要求的存取權限的相關資訊，請參閱 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 文章一節 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >如果您未指定將使用者指派給專案上的問題時，希望他們擁有的問題權限，依預設，他們會獲得與專案相同的權限。

   * 指定使用者在建立請求佇列時，在請求佇列中提交的問題時收到的權限。 如需詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

      >[!IMPORTANT]
      >
      >根據專案是否以請求佇列發佈，授予的權限會有所不同：
      >
      >   
      >   
      >   * 當用戶將請求提交到發佈為請求隊列的項目時，「主要聯繫人」和「輸入者」將獲得指定的權限。
      >   * 當用戶向未作為請求隊列發佈的項目提交請求時，主要聯繫人（如果與「輸入者」不同）將獲得指定的權限，而「輸入者」用戶則獲得該問題的「管理」權限。


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 問題權限

下表顯示允許使用者檢視、貢獻或管理問題時，您可授予哪些權限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>動作</strong> </td> 
   <td><strong>管理</strong> </td> 
   <td><strong>參與</strong> </td> 
   <td><strong>檢視</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>新增  個問題</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除 </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>附加自訂表格</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯自訂欄位</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>核准問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>新增核准程式</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>新增文件</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>複製問題*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>移動問題</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>記錄時數</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>轉換至專案*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>接受分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新/注釋</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>修改計畫日期</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>進行任務指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>共用系統範圍</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;由專案的存取層級和權限控制。
