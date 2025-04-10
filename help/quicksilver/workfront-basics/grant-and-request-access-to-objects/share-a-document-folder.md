---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共用檔案資料夾
description: 您可以從「檔案」區域共用資料夾及其內容。
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 842c61cf6dfee0c79b1c95ff84888083c9f5b5a4
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 共用檔案資料夾

您可以從「檔案」區域共用資料夾及其內容。

>[!NOTE]
>
>* 資料夾必須位於物件上資料夾階層的前五個層級。 第六層級或更低層級的每個資料夾都會從其正上方的資料夾繼承其共用設定。
>
>  如需新增子資料夾以建立資料夾階層的相關資訊，請參閱文章[建立檔案資料夾](../../documents/organizing-documents/create-documents-folder.md)中的[建立資料夾和子資料夾](../../documents/organizing-documents/create-documents-folder.md#creating-folders)小節。
>
>* 無法共用智慧資料夾。
>* 如果您在範本中設定檔案資料夾的共用選項，然後有人從該範本建立專案，則您的共用設定不會轉移到新專案中的檔案資料夾。
>* 如果您為工作專案中的檔案資料夾設定共用選項，然後複製工作專案，則您的共用設定不會轉移到新工作專案中的檔案資料夾。
>

## 存取需求

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視物件的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 共用資料夾

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**檔案**。

   或

   開啟Workfront物件後，按一下左側面板中的&#x200B;**檔案**。

1. 選取資料夾，然後按一下工具列中的「共用」圖示![](assets/share-icon.png)。

   資料夾必須位於物件上資料夾階層的前五個層級，而且不能是智慧型資料夾。

1. 在顯示的方塊中，在&#x200B;**授與資料夾存取權**&#x200B;下方，開始輸入您要共用資料夾的使用者、團隊、工作角色、群組或公司名稱，然後在名稱顯示時按&#x200B;**Enter**。
1. 若要調整您剛新增的使用者、團隊、工作角色、群組或公司的存取權，請按一下名稱右側的下拉式功能表，然後設定下列其中一個可用選項及其任何進階設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>檢視資料夾及其內容的功能。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li><strong>下載</strong>：能夠以ZIP檔案格式下載資料夾及其內容</li> 
        <li> <p><strong>共用</strong>：能夠與系統中的其他人共用資料夾</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>能夠檢視和編輯資料夾及其內容</p> <p>按一下<strong>進階設定</strong>，指定是否要允許使用者執行下列動作：</p> 
       <ul> 
        <li><strong>刪除</strong>：從系統中刪除資料夾及其內容</li> 
        <li><b>下載</b>：將資料夾及其內容下載為ZIP檔</li> 
        <li><strong>共用</strong>：與系統中的其他使用者共用資料夾及其內容</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複步驟3至4，將其他名稱新增至清單並設定其選項。
1. （選擇性）如果您希望系統中的每個人都能檢視資料夾及其內容，請按一下共用方塊右上角的齒輪圖示![](assets/gear-icon-settings-with-dn-arrow.jpg)，然後按一下&#x200B;**讓此內容在整個系統內可見。**

   如果您改變心意，可以按一下&#x200B;**移除系統範圍存取權** （預設選項）。

## 使用者如何存取共用給他們的資料夾內容

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

目前，當您共用資料夾時，收件者在其「檔案」區域中看不到該資料夾。 但是，他們可以透過執行檔案報告來存取其檔案。

如需有關執行報表的資訊，請參閱文章[瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[物件報表](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)一節。 另請參閱[建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## 當您共用包含資料夾的物件時繼承的許可權

當您共用具有檔案資料夾的物件時，收件者也可存取該資料夾：

* 如果您授予收件者對父系物件的檢視存取權，則他們擁有該資料夾的檢視存取權。
* 如果您授予收件者「貢獻」或「管理」存取上層物件的許可權，則他們擁有該資料夾的「管理」存取權。
* 如果您將一種存取權型別（檢視、貢獻或管理）授予父物件，並將另一種存取權型別授予資料夾，則您的收件者對資料夾中的檔案具有這兩種存取權型別中最高的存取權

  例如，如果您共用具有「檢視」存取權的父物件，以及具有「管理」存取權的資料夾，則收件者會擁有該資料夾中檔案的「管理」。

  >[!NOTE]
  >
  >附加的檔案只會從附加它的物件繼承許可權。 如果您在物件上建立資料夾並將檔案移至資料夾，則會繼承資料夾的許可權。 但是，如果您在父項或祖項物件上建立資料夾，並將檔案移至該資料夾，則不會繼承該資料夾的許可權。

* 如果收件者的存取層級中啟用了「不要從專案、任務、問題等繼承檔案存取權」選項，他們將不會繼承您與他們共用之資料夾中檔案的許可權。 若要讓他們存取資料夾中的檔案，您必須共用該檔案。

  如需「永不繼承」選項的詳細資訊，請參閱[設定Adobe Workfront的存取權](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)。

  如需共用檔案的詳細資訊，請參閱[共用檔案](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)。
