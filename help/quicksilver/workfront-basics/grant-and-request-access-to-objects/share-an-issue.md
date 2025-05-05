---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共用問題
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯問題的存取權。 有關授予問題存取權的詳細資訊，請參閱授予問題存取權。
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 2%

---

# 共用問題

當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯問題的存取權。 如需授與問題存取權的詳細資訊，請參閱[授與問題存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視、貢獻或管理您有權共用之特定問題的許可權。 如需存取層級和許可權的詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p> 
   或
   <p>目前：工作或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於共用問題的考量事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 問題的建立者預設擁有其「管理」許可權。
* 您可以個別共用問題，也可以一次共用數個問題。 共用問題等同於在Workfront中共用其他專案。 如需在Workfront中共用專案的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以向問題授予下列許可權： 

   * 檢視
   * 參與
   * 管理

* 當您共用問題時，附加到問題的所有檔案都會繼承相同的許可權。

  Workfront管理員可以指定檔案是否應該繼承使用者存取層級中較高物件的許可權。 如需有關限制檔案繼承許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您可以從問題中移除繼承的許可權。 如需詳細資訊，請參閱[從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共用問題的方式

* 手動，類似Workfront中的共用任何其他物件。
* 執行下列任一項作業以自動執行：

   * 指定問題之任何父系物件的許可權：專案、方案或投資組合。 問題會繼承其父物件的許可權。 如需有關檢視物件繼承許可權的資訊，請參閱[檢視物件的繼承許可權](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。
   * 在用來建立問題所在專案的範本上，將實體新增到專案共用。 如需從範本共用專案的詳細資訊，請參閱[共用範本](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * 指定編輯專案時專案中所有問題的許可權。 如需有關根據使用者對專案的許可權來管理專案上問題或請求的存取許可權的資訊，請參閱文章[編輯專案](../../manage-work/projects/manage-projects/edit-projects.md)中的[&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access)區段。

     >[!TIP]
     >
     >如果您未指定將使用者指派給專案問題的時候您希望使用者擁有哪些問題許可權，預設情況下，他們會獲得與專案相同的許可權。

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

## 共用問題

1. 導覽至您要共用的問題。

1. 在問題名稱的右側，按一下&#x200B;**共用**。 **共用[問題名稱]**&#x200B;對話方塊開啟。

   ![共用問題按鈕](assets/share-issue-button.png)

1. 在&#x200B;**授與問題存取權**&#x200B;欄位中，開始輸入您要與其共用問題的使用者、團隊、角色、群組或公司的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用問題。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取問題的存取層級：

   * **只有受邀人員才能存取：**&#x200B;只有受邀參與問題的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以在沒有邀請的情況下檢視問題。

1. 按一下使用者名稱右側的下拉式清單，然後選取其對此問題的許可權層級：

   * **檢視**：使用者可以檢視並共用問題。
   * **貢獻**：使用者可以更新、記錄資訊、進行次要編輯及共用問題（也包括所有檢視許可權）。
   * **管理**：使用者擁有此問題的完整存取權，但無管理許可權，這些許可權是在存取層級授與的（也包含所有[檢視]和[貢獻]許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定問題的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-permission-options.png)

1. （選擇性）若要使用連結快速共用問題，請按一下[複製連結] **，然後將其轉寄給收件者。**

1. 按一下「**儲存**」。

## 大量共用問題

1. 導覽至包含您要共用之問題的專案。

1. 在專案頁面的「**問題**」標籤中，選取您要共用之每個問題左側的方塊，然後按一下頁面頂端的「**共用**」圖示「![共用」圖示](assets/share-icon.png)。 共用強制回應視窗隨即開啟。

   ![大量共用問題](assets/bulk-share-issues.png)

1. 在&#x200B;**授與問題存取權**&#x200B;欄位中，開始輸入您要與其共用問題的使用者、團隊、角色、群組或公司的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用問題。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取問題的存取層級：

   * **只有受邀人員才能存取：**&#x200B;只有受邀參與問題的使用者才能存取問題（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以在沒有邀請的情況下檢視問題。


1. 按一下使用者名稱右側的下拉式清單，並選取其問題的許可權層級：

   * **檢視**：使用者可以檢視和共用問題。
   * **貢獻**：使用者可以更新、記錄資訊、進行次要編輯及共用問題（也包括所有檢視許可權）。
   * **管理**：使用者擁有問題的完整存取權，但沒有管理許可權，這些許可權是在存取層級授與的（也包含所有檢視和貢獻許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定問題的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-permission-options.png)

1. 按一下「**儲存**」。

## 問題許可權

下表顯示當允許使用者檢視、貢獻或管理問題時，您可以授予他們哪些許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>動作</strong> </td> 
   <td><strong>管理</strong> </td> 
   <td><strong>貢獻</strong> </td> 
   <td><strong>檢視</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>新增問題</p> </td> 
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
   <td>附加自訂表單</td> 
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
   <td>新增核准流程</td> 
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
   <td>轉換為專案*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>接受指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新/評論</td> 
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
   <td>全系統共用</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;由專案的存取層級和許可權所控制。
