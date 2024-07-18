---
content-type: overview
product-area: documents
keywords: 證明，許可權
navigation-topic: proofing-overview
title: 校訂許可權設定檔概述
description: 校訂許可權設定檔決定使用者在您的帳戶中擁有所有校訂的整體許可權。 校訂許可權設定檔指派給使用者在其使用者設定檔中。 校訂許可權設定檔與校訂角色不同。
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---

# 校訂許可權設定檔概述

<!--Audited: 12/2023-->

校訂許可權設定檔決定使用者在您的帳戶中擁有所有校訂的整體許可權。 校訂許可權設定檔指派給使用者在其使用者設定檔中。

校訂許可權設定檔與校訂角色不同。 如需校訂角色的詳細資訊，請參閱[校訂角色概觀](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md)。

>[!NOTE]
>
>如果您是管理員，可以為貴組織中的使用者建立自訂設定檔。 如需詳細資訊，請參閱[在Workfront Proof中設定自訂設定檔](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## 校訂許可權設定檔

下表顯示每個校訂許可權設定檔的可用許可權。

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>擁有的專案</strong>
   </td>
   <td colspan="3" ><strong>其他使用者的專案</strong>
   </td>
   <td><strong>管理員</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>新增</strong>
   </td>
   <td><strong>檢視</strong>
   </td>
   <td><strong>編輯</strong>
   </td>
   <td><strong>刪除</strong>
   </td>
   <td><strong>檢視</strong>
   </td>
   <td><strong>編輯</strong>
   </td>
   <td><strong>刪除</strong>
   </td>
   <td><strong>編輯和刪除</strong>
   </td>
  </tr>
  <tr>
   <td>管理員
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>主管
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>經理
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### 管理員

系統管理員可以存取[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)，並具有下列許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>管理員可以：</td> 
   <td>管理員無法：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>建立校樣、上傳檔案和建立資料夾</p> </li> 
     <li> <p>檢視、編輯和刪除校訂和他們建立的檔案</p> </li> 
     <li> <p>檢視、編輯和刪除組織中的所有使用者建立的校訂和檔案</p> </li> 
     <li> <p>刪除其他使用者的公用資料夾</p> </li> 
     <li> <p>編輯帳戶中建立的所有校訂</p> </li> 
     <li> <p>設為拖放區域擁有者*</p> </li> 
     <li> <p>存取「帳戶設定」頁面並編輯帳戶詳細資料</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
     <li> <p>新增、編輯和刪除使用者</p> </li> 
     <li> <p>建立群組並新增連絡人</p> </li> 
     <li> <p>刪除連絡人</p> </li> 
     <li> <p>如果校訂上沒有回覆，則編輯校訂</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>編輯校訂回覆。</p> </li> 
     <li> <p>刪除其他使用者的私人資料夾</p> </li> 
     <li> <p>存取「帳單」頁面或編輯帳單詳細資訊</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;僅適用於Workfront Proof獨立版產品。

### 主管

主管擁有下列許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>主管可以：</td> 
   <td>主管無法：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>建立校樣、上傳檔案和建立資料夾</p> </li> 
     <li> <p>檢視、編輯和刪除校訂和他們建立的檔案</p> </li> 
     <li> <p>檢視、編輯和刪除組織中的所有使用者建立的校訂和檔案</p> </li> 
     <li> <p>刪除其他使用者的公用資料夾</p> </li> 
     <li> <p>編輯帳戶中建立的所有校訂</p> </li> 
     <li> <p>建立群組並新增連絡人</p> </li> 
     <li> <p>刪除連絡人</p> </li> 
     <li> <p>如果校訂上沒有回覆，則編輯校訂</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>編輯校訂回覆。</p> </li> 
     <li> <p>刪除其他使用者的私人資料夾</p> </li> 
     <li> <p>存取「帳單」頁面或編輯帳單詳細資訊</p> </li> 
     <li> <p>新增、編輯或刪除使用者</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 經理

管理員擁有下列許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>管理員可以：</td> 
   <td>管理員無法：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>建立校樣、上傳檔案和建立資料夾</p> </li> 
     <li> <p>檢視、編輯和刪除校訂和他們建立的檔案</p> </li> 
     <li> <p>檢視、稽核及核准其他明確與其共用之使用者的校訂（共用資料夾中所有內容的唯讀許可權）</p> </li> 
     <li> <p>編輯帳戶中建立的所有校訂</p> </li> 
     <li> <p>建立群組並新增連絡人</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>檢視、編輯或刪除組織內其他使用者建立的校訂和檔案。 </p> </li><li><p>編輯校訂回覆。</p> </li> 
     <li> <p>刪除其他使用者的私人或公用資料夾</p> </li> 
     <li> <p>存取「帳單」頁面或編輯帳單詳細資訊</p> </li> 
     <li> <p>新增、編輯或刪除使用者</p> </li> 
     <li> <p> 刪除連絡人</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
