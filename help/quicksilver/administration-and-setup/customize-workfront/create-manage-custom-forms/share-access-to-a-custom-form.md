---
title: 共用自訂表格
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以設定自訂表單的存取權，以控制誰可以檢視、共用和編輯該表單。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 264419f747b1e975cda8843b37558e78501d93de
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 2%

---

# 共用自訂表格

{#preview-fast-release-general}

您可以設定自訂表單的存取權，以控制誰 — 人員、角色、群組、團隊、公司、企業設定檔 — 可以檢視、共用及編輯它。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取自訂表格 {#access-to-custom-forms}

根據預設，當您建立新的自訂表單且有人將其附加到物件時，任何指派給該物件的使用者都可以檢視並填寫表單。 這包括擁有貢獻者或請求授權的使用者，以及外部使用者。

但是，在尚未附加自訂表單的物件上，使用者（即使他們具有「規劃工具」存取層級）無法從「自訂Forms」下拉式選單中附加它，除非以下其中一項為True：

* <span class="preview">有人共用自訂表單，因為「系統中的每個人都可以檢視和附加」</span>
* 有人將自訂表單與使用者共用，或與其團隊、工作角色、群組、公司或企業設定檔共用，已選取附加至自訂資料並至少授予檢視許可權
* 使用者擁有標準或計畫授權，其存取層級允許對自訂表單的管理存取權

<!--

## Share a custom form from the list of forms

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access-to-custom-forms) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Select the custom form, then click ![Share icon](assets/share-icon.png).
1. In the box that displays, under **Give custom form access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the custom form with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, company, or business profile you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>This option provides the ability to view and fill out the custom form on objects. At the object level, users must also have at least Contribute access with the <strong>Edit custom form</strong> advanced setting enabled. For example, if the form is attached to a project, users must have Contribute access to that project, or they will not be able to fill out the form.</p>
      
      <p><b>NOTE</b>: For users with Light and Contributor licenses (or Work, Review, and Request licenses), this is the highest available option.</p>
      
      <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><strong>Share</strong>: Ability to share the custom form with others in the system</p> <p>Users with a Light or Contributor license (or Work, Review, or Request license) can share a custom form only through the API or a custom forms report.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>This option available only for users with a Standard or Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow following:</p> 
       <ul> 
        <li> <p><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
        <li><strong>Delete</strong>: Delete the custom form from the system</li> 
        <li><strong>Share</strong>: Share the custom form with others in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Remove system-wide access**.

   If you change your mind, you can click **Make this visible system-wide** (the default option).

   >[!NOTE]
   >
   >* When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >* Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use **Make this visible system-wide**. When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.

1. Click **Save**.

-->

## 共用自訂表格

您可以為特定使用者、工作角色、群組、團隊、公司和企業設定檔設定特定層級的表單存取權，而不是將自訂表單保留在預設共用狀態（本文中關於存取自訂表單[&#128279;](#access-to-custom-forms)的說明）。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 在清單中選取自訂表格，然後按一下![共用圖示](assets/share-icon.png)。

   或

   開啟自訂表單或建立新的自訂表單。 然後，按一下表單設計工具右上角的&#x200B;**共用**。

1. 在共用方塊中，在&#x200B;**授與自訂表單存取權**&#x200B;下方，開始輸入您要與共用自訂表單的使用者、團隊、工作角色、群組、公司或企業設定檔的名稱，然後在名稱顯示時按&#x200B;**Enter**。
1. 若要調整您剛新增的使用者、團隊、工作角色、群組、公司或企業設定檔的存取權，請按一下名稱右側的下拉式功能表，然後設定下列其中一個可用選項及其任何進階設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視</td> 
      <td> <p>此選項提供在物件上檢視和填寫自訂表單的功能。 在物件層級，使用者必須至少擁有Contribute存取權，並啟用<strong>編輯自訂表單</strong>進階設定。 例如，如果表單附加至專案，使用者必須擁有該專案的Contribute存取權，否則將無法填寫表單。</p>

   <p><b>注意</b>：對於擁有輕度授權和貢獻者授權（或工作、檢閱和請求授權）的使用者，這是最高的可用選項。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</li> 
        <li> <p><strong>共用</strong>：能夠與系統中的其他人共用自訂表單</p> <p>具有輕度或貢獻者授權（或工作、檢閱或請求授權）的使用者只能透過API或自訂表單報表共用自訂表單。</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理</td> 
      <td> <p>此選項僅適用於擁有Standard或Plan授權的使用者。 </p> <p>除了能夠將表單新增到他們有權編輯的物件之外，使用者還可以完全編輯自訂表單，包括新增、編輯和刪除欄位。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li> <p><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</p> </li> 
        <li><strong>刪除</strong>：從系統中刪除自訂表單</li> 
        <li><strong>共用</strong>：與系統中的其他人共用自訂表單</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複步驟5至6，將其他名稱新增至清單並設定其選項。
1. （選擇性）如果您想要將自訂表單（在其附加的物件上）的存取許可權制在您先前步驟中指定的物件上，請按一下「**誰有存取權**」下的下拉式箭頭，然後選取「**只有受邀者才能存取**」。

   如果您改變心意，可以選取&#x200B;**系統中的每個人都可以檢視**。

   >[!NOTE]
   >
   >* 當您將自訂表單設定為全系統可見時，您僅允許使用者在指派給他們的物件上看見並填寫它，不允許將其附加到其他物件。 您可以使用步驟6中說明的「附加至自訂資料」選項，授與將自訂表單附加至物件的功能。
   >* 大多陣列織都想要確保系統中的每個人都可以填寫自訂表單，將其附加到他們工作的物件上，並在報表中檢視其資料。 如果您的組織有此情況，建議您使用&#x200B;**系統中的每個人都可以檢視**。
   >* <span class="preview">若您選取&#x200B;**系統中的每個人都可以檢視和附加**，則所有使用者都可以將表單附加到其他物件。</span>
   >
   >在預覽環境中<span class="preview">範例影像：</span>
   >![共用自訂表單](assets/share-custom-forms-all-can-attach.png)
   >   
   >生產環境中的影像範例：
   >![共用自訂表單](assets/share-custom-form-in-designer.png)
   >   
   >如果您擔心自訂表單附加至特定物件時，使用者可能會輸入敏感資料，限制共用&#x200B;*物件*&#x200B;可能比限制存取表單本身更有效率。

1. 按一下「**儲存**」。

## 移除對自訂表單的存取權

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 在清單中選取自訂表格，然後按一下![共用圖示](assets/share-icon.png)。
1. 在共用方塊中，按一下您不想再擁有表單的特殊存取許可權的使用者、團隊、角色、群組、公司或企業設定檔名稱右側的下拉式功能表，然後選取&#x200B;**移除**。
1. （選擇性）對您要移除的其他名稱重複上述步驟。
1. 按一下「**儲存**」。
