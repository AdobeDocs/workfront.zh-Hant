---
title: 授予對文檔的訪問權
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中檔案的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 授予對文檔的訪問權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對檔案的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

此訪問也適用於文檔資料夾。

如需使用自訂存取層級來管理使用者對Workfront中其他物件類型的存取權限的相關資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。&gt;。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定義訪問級別配置用戶對文檔的訪問權限

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   ![document_access.png](assets/document-access.png)

   您可以讓使用者針對他們有權存取的專案、工作和問題執行下列動作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">建立</td> 
      <td>上傳檔案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td> <p>刪除已上載的文檔。</p> <p>此 <b>建立</b> 選項啟用時，系統會自動啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用</td> 
      <td>與特定使用者、工作角色、團隊共用檔案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用公開文件</td> 
      <td>與外部使用者共用檔案(沒有Workfront授權)。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用系統範圍</td> 
      <td> <p>讓檔案可供Workfront執行個體中的所有人使用。</p> <p>如果出現以下情況，系統中的任何人都可以看到以此方式共用的文檔：</p> 
       <ul> 
        <li> <p>您會將連結傳送給上傳檔案的頁面。</p> </li> 
        <li> <p>他們在Workfront找</p> </li> 
       </ul> <p>此 <b>共用</b> 選項啟用時，系統會自動啟用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >為特定類型的對象配置訪問級別設定時，該配置不會影響用戶對級別較低的對象的訪問。 例如，您可以限制用戶刪除其訪問級別中的項目，但這不會限制用戶刪除與項目相比排名較低的文檔。有關對象層次結構的詳細資訊，請參閱部分 [對象的相互依存和層次](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （可選）要限制較高排名對象的文檔的繼承權限，請按一下 **設定其他限制**，然後選取 **從不繼承項目、任務、問題等的文檔訪問**.
1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按許可類型訪問文檔

有關每個訪問級別中的用戶可以對文檔執行哪些操作的詳細資訊，請參閱部分 [檔案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 對共用文檔的訪問

將檔案上傳至Workfront後，您可以授與其他使用者權限，將檔案與他們共用，如 [共用檔案](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

當您與其他使用者共用任何物件時，收件者對其的權利由兩項內容的組合所決定：

* 您授予物件收件者的權限
* 對象類型的收件人的訪問級別設定
