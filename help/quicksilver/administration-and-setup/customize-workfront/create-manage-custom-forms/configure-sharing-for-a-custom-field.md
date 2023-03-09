---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用舊版表單產生器設定自訂欄位和小工具的共用
description: 預設情況下，將新的自定義欄位或介面工具集添加到自定義表單時，系統中有權訪問自定義表單的任何人都可以編輯該項目的屬性，如其標籤和名稱。 您可以控制可以與誰共用，以變更此項目。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---

# 使用舊版表單產生器設定自訂欄位和小工具的共用

預設情況下，將新的自定義欄位或介面工具集添加到自定義表單時，系統中有權訪問自定義表單的任何人都可以編輯該項目的屬性，如其標籤和名稱。 您可以控制可以與誰共用，以變更此項目。

如需自訂表單中自訂欄位和小工具的相關資訊，請參閱 [使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [使用舊版表單產生器在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 配置自定義欄位或介面工具集的共用

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **自訂Forms**.
1. 如果您正在組織的Workfront例項中設定自訂欄位或介面工具集的共用，請執行下列動作：

   1. 按一下 **欄位** 標籤。
   1. 選擇要配置共用的項目，然後按一下 **共用**.

   或者，如果您要在現有自訂表單中設定自訂欄位或介面工具集的共用，請執行下列操作：

   1. 選取自訂表單，然後按一下 **編輯**.
   1. 在右側的表單編輯區域中，選取要配置共用的項目。
   1. 在左側面板中，按一下 **共用欄位**.


1. 在 **自訂欄位存取** 框，指定要與誰共用項目以及要如何共用項目：

   1. 在 **自訂欄位存取** 框下 **授予自訂欄位存取權**，開始鍵入要與共用項目的用戶、團隊、作業角色、組或公司的名稱，然後在出現時按一下該名稱。

      ![](assets/share-field-give-access-to.jpg)

   1. 如果您想要更明確地了解要如何共用項目，請按一下名稱右側的下拉式清單，然後使用下列任一選項：

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">檢視它</td> 
         <td> <p>您可以按一下 <strong>進階設定</strong> 指定您希望使用者或使用者能夠使用其存取權將項目新增至自訂表單，或與其他使用者共用。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">管理它</td> 
         <td> <p>允許存取編輯自訂欄位，並在欄位資料庫和您建立自訂表單的頁面中查看。</p> <p>您可以按一下 <strong>進階設定</strong> 指定是否希望用戶或用戶能夠使用其訪問權限從系統中刪除項目或與其他用戶共用該項目。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （可選）重複上一步，將其他名稱新增至清單並設定其選項。
1. （選用）按一下齒輪圖示 ![](assets/gear-icon-settings.png) 欄位，請在右上角選擇「系統範圍共用」選項。

   並非所有下列選項都會同時顯示在此下拉式功能表中。 例如，第二個只有在選取其他兩個時才會顯示。

   * **將此可編輯的系統範圍設為Workfront，讓每個人都能編輯它** （預設選項）

      當您新增自訂欄位或介面工具集，但並未限制共用時，系統中有權存取自訂表單的每個人都可以檢視並編輯其屬性。

   * **移除系統範圍編輯存取權限。**

      僅限您新增至清單的使用者存取。

   * **使其在整個系統內都可見，以便 Workfront 中的每個人都可以看到它**

1. 按一下 **儲存** 或 **儲存+關閉**.

## 繼承在共用自訂表單時對自訂欄位和介面工具集的存取

當某人與組、職務角色、團隊或公司共用自訂表單時，收件者將繼承對表單上任何自訂欄位和小工具的「查看」訪問權。 始終保留對表單上這些項的此訪問級別，以便表單能夠按照建立者的預期為收件人運行。 即使是具有表單編輯存取權的收件者，也是如此。

您可以找出誰繼承了自訂欄位或介面工具集的存取權，並移除其存取權。

>[!NOTE]
>
>如果收件者在共用自訂表單上擁有自訂欄位或介面工具集的「管理」存取權，該存取權會保留給收件者。

* [了解誰繼承了自訂欄位或介面工具集的存取權](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [在已共用的自訂表單中，移除對自訂欄位或介面工具集的存取權](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 了解誰繼承了自訂欄位或介面工具集的存取權 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **自訂Forms**.
1. 按一下 **欄位** 頁簽，然後選擇欄位、影像或訪問介面工具集。
1. 在顯示的方塊中，按一下 **繼承的權限** 並查看顯示的名稱。
1. 按一下 **取消**.

### 在已共用的自訂表單中，移除對自訂欄位或介面工具集的存取權 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要移除已共用之自訂表單中自訂欄位或介面工具集的存取權，則需要取消共用表單。 如需指示，請參閱 [移除自訂表單的存取權](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) 在文章中 [共用自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
