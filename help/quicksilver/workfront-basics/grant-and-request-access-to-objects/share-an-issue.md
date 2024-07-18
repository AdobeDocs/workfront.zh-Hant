---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共用問題
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯問題的存取權。 有關授予問題存取權的詳細資訊，請參閱授予問題存取權。
author: Alina
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 2%

---

# 共用問題

當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯問題的存取權。 如需授與問題存取權的詳細資訊，請參閱[授與問題存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視、Contribute或管理您有權共用之特定問題的許可權。 如需存取層級和許可權的詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。

## 關於共用問題的考量事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 依預設，問題的建立者擁有管理許可權。
* 您可以個別共用問題，也可以一次共用數個問題。 共用問題等同於在Workfront中共用其他專案。 如需在Workfront中共用專案的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以向問題授予下列許可權： 

   * 檢視

     ![view_on_issue.png](assets/view-on-issue-221x216.png)

   * 管理

     ![manage_on_issues.png](assets/manage-on-issues-179x199.png)

   * 參與\
     ![contribute_on_issue.png](assets/contribute-on-issue-156x205.png)

* 當您共用問題時，附加到問題的所有檔案都會繼承相同的許可權。

  Workfront管理員可以指定檔案是否應該繼承使用者存取層級中較高物件的許可權。 如需有關限制檔案繼承許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您可以從問題中移除繼承的許可權。 如需詳細資訊，請參閱[從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共用問題的方式

* 手動，類似Workfront中的共用任何其他物件。 如需有關如何在Workfront中共用物件的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 執行下列任一項作業以自動執行：

   * 指定問題之任何父系物件的許可權：專案、方案或投資組合。 問題會繼承其父物件的許可權。 如需有關檢視物件繼承許可權的資訊，請參閱[檢視物件的繼承許可權](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。
   * 在用來建立問題所在專案的範本上，將實體新增到專案共用。 如需從範本共用專案的詳細資訊，請參閱[共用範本](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * 指定編輯專案時專案中所有問題的許可權。 如需有關根據使用者對專案的許可權來管理專案上問題或請求的存取許可權的資訊，請參閱文章[編輯專案](../../manage-work/projects/manage-projects/edit-projects.md)中的[](../../manage-work/projects/manage-projects/edit-projects.md#access)區段。

     >[!TIP]
     >
     >如果您未指定將使用者指派給專案問題的時候您希望使用者擁有哪些問題許可權，預設情況下，他們會獲得在專案上擁有的相同許可權。

   * 指定使用者在建立請求佇列時，針對在請求佇列中提交的問題所接收的許可權。 如需詳細資訊，請參閱[建立要求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

     >[!IMPORTANT]
     >
     >根據專案是否發佈為請求佇列，授予許可權的方式有所不同：
     >
     >   
     >   
     >   * 當使用者將請求提交到作為請求佇列發佈的專案時，主要聯絡人和輸入者使用者將被授予指定的許可權。
     >   * 當使用者將請求提交到未作為請求佇列發佈的專案時，主要聯絡人（如果與「輸入者」使用者不同）被授予指定的許可權，並且「輸入者」使用者被授予該問題的管理許可權。
     >   
     >

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

## 問題許可權

下表顯示當允許使用者檢視、Contribute或管理問題時，您可以授予他們哪些許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>動作</strong> </td> 
   <td><strong>管理</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>檢視</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>新增問題</p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除 </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>附加自訂表單</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯自訂欄位</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>核准問題</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>新增核准流程</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>新增文件</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>複製問題*</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>移動問題</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>記錄時數</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>轉換為專案*</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>接受指派</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新/評論</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>修改計畫日期</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>進行任務指派</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>全系統共用</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
 </tbody> 
</table>

&#42;由專案的存取層級和許可權所控制。
