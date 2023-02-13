---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共用文檔資料夾
description: 您可以從「文檔」區域共用資料夾及其內容。
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 共用文檔資料夾

您可以從「文檔」區域共用資料夾及其內容。

>[!NOTE]
>
>* 資料夾必須位於對象上資料夾層次結構的前五個級別中。 第六級或第六級以下的每個資料夾都會繼承其上方資料夾的共用配置。
>
>  有關添加子資料夾以建立資料夾層次結構的資訊，請參見部分 [建立資料夾和子資料夾](../../documents/organizing-documents/create-documents-folder.md#creating-folders) 在文章中 [建立文檔資料夾](../../documents/organizing-documents/create-documents-folder.md).
>
>* 無法共用智慧資料夾。
>* 如果為模板中的文檔資料夾配置共用選項，然後有人從該模板建立項目，則您的共用配置不會轉移到新項目中的文檔資料夾。
>* 如果為工作項內的文檔資料夾配置共用選項，然後複製工作項，則共用配置不會轉移到新工作項中的文檔資料夾。
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

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視物件的存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用資料夾

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **檔案**.

   或

   開啟Workfront物件時，按一下 **檔案** 中。

1. 選取資料夾，然後按一下「共用」圖示 ![](assets/share-icon.png) 的下一頁。

   資料夾必須位於對象上資料夾層次結構的前五個級別，並且不能是智慧資料夾。

1. 在顯示的方塊中，於 **授予資料夾存取權**，開始鍵入要與共用資料夾的用戶、團隊、職務角色、組或公司的名稱，然後按鍵 **輸入** 名稱時顯示。
1. 若要調整您剛新增的使用者、團隊、工作角色、群組或公司的存取權，請按一下名稱右側的下拉式功能表，然後設定下列其中一個可用選項及其任何進階設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>檢視資料夾及其內容的功能。</p> <p>按一下 <strong>進階設定</strong> 指定是否允許下列項目：</p> 
       <ul> 
        <li><strong>下載</strong>:能將資料夾及其內容下載為ZIP檔案</li> 
        <li> <p><strong>共用</strong>:可與系統中的其他人共用資料夾</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>檢視及編輯資料夾及其內容的功能</p> <p>按一下 <strong>進階設定</strong> 指定是否允許用戶執行以下操作：</p> 
       <ul> 
        <li><strong>刪除</strong>:從系統中刪除資料夾及其內容</li> 
        <li><b>下載</b>:將資料夾及其內容下載為ZIP檔案</li> 
        <li><strong>共用</strong>:與系統中的其他用戶共用資料夾及其內容</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複步驟3-4將其他名稱新增至清單並設定其選項。
1. （可選）如果您希望系統中的所有人都能查看資料夾及其內容，請按一下齒輪表徵圖 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 在共用方塊的右上角，然後按一下 **使此系統範圍可見。**

   如果您改變心意，可以按一下 **刪除系統範圍的訪問** （預設選項）。

## 使用者如何存取與其共用之資料夾的內容

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

目前，當您共用資料夾時，收件者在其「檔案」區域中看不到該資料夾。 但是，他們可以通過運行文檔報告來訪問其文檔。

如需執行報表的相關資訊，請參閱區段 [對象報告](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 在文章中 [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). 另請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## 共用包含資料夾的物件時繼承的權限

當您共用具有文檔資料夾的對象時，收件者還可以訪問該資料夾：

* 如果您授予收件者對上層物件的「檢視」存取權，則他們擁有資料夾的「檢視」存取權。
* 如果您授予收件者對上層物件的「貢獻」或「管理」存取權，則他們擁有資料夾的「管理」存取權。
* 如果您授予父對象一種訪問類型（查看、貢獻或管理），而授予資料夾另一種訪問類型，則收件者對資料夾內文檔的訪問具有這兩種類型的最高權限

   例如，如果您共用具有「查看」訪問權限的父對象和具有「管理」訪問權限的資料夾，則收件者對資料夾中的文檔具有「管理」權限。

   >[!NOTE]
   >
   >附加的文檔僅繼承附加的對象的權限。 如果在對象上建立資料夾並將文檔移動到資料夾中，它會繼承資料夾的權限。 但是，如果在父或祖父對象上建立資料夾，並將文檔移入該資料夾，則不會繼承該資料夾的權限。

* 如果在收件人的訪問級別中啟用了「從項目、任務、問題等中繼承文檔訪問」選項，則這些人將不會繼承您與他們共用的資料夾中文檔的權限。 要授予他們對資料夾中文檔的訪問權，必須共用該文檔。

   有關「從不繼承」選項的資訊，請參見 [設定Adobe Workfront的存取權](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

   有關共用文檔的資訊，請參閱 [共用檔案](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
