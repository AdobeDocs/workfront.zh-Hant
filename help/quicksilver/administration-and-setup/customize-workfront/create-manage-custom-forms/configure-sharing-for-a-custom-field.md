---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用舊版表單產生器設定自訂欄位和Widget的共用
description: 根據預設，當您新增自訂欄位或Widget至自訂表單時，系統中有權存取自訂表單的任何人都可以編輯該專案的屬性，例如其標籤和名稱。 您可以透過控制誰可以與其共用來變更此專案。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 使用舊版表單產生器設定自訂欄位和Widget的共用

{{form-designer-default}}

根據預設，當您新增自訂欄位或Widget至自訂表單時，系統中有權存取自訂表單的任何人都可以編輯該專案的屬性，例如其標籤和名稱。 您可以透過控制誰可以與其共用來變更此專案。

如需自訂表單中的自訂欄位和Widget相關資訊，請參閱[使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)，以及[使用舊版表單產生器新增或編輯自訂表單中的資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 設定自訂欄位或Widget的共用

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 如果您在貴組織的Workfront例項中為自訂欄位或Widget設定共用，請執行以下操作：

   1. 按一下&#x200B;**欄位**&#x200B;以開啟[欄位]區域。
   1. 選取您要設定共用的專案，然後按一下![共用圖示](assets/share-icon.png)。

   或者，如果您要設定現有自訂表單中自訂欄位或Widget的共用，請執行下列動作：

   1. 選取自訂表單，然後按一下![編輯圖示](assets/edit-icon.png)。
   1. 在右側的表單編輯區域中，選取您要設定共用的專案。
   1. 在左側面板中，按一下&#x200B;**共用欄位**。

1. 在顯示的&#x200B;**自訂欄位存取**&#x200B;方塊中，指定您要與誰共用專案以及要如何共用：

   1. 在&#x200B;**自訂欄位存取**&#x200B;方塊的左下角附近，在&#x200B;**授與自訂欄位存取權**&#x200B;下方，開始輸入您要共用專案的使用者、團隊、工作角色、群組或公司的名稱，然後按一下名稱。

      ![](assets/share-field-give-access-to.jpg)

   1. 如果您想更明確地說明要如何共用專案，請按一下名稱右側的下拉式清單，然後使用下列任一選項：

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">檢視它</td> 
         <td> <p>您可以按一下<strong>進階設定</strong>，指定您是否希望使用者能夠使用其存取許可權將專案新增至自訂表單，或與其他使用者共用。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">管理它</td> 
         <td> <p>允許存取以編輯自訂欄位，並在欄位庫和建立自訂表單的頁面上檢視它。</p> <p>您可以按一下<strong>進階設定</strong>，指定您是否希望使用者能夠使用其存取許可權從系統刪除專案或與其他使用者共用。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （可選）重複上一步驟，將其他名稱新增至清單並設定其選項。
1. （選擇性）如果要為欄位選擇全系統共用選項，請按一下右上角的齒輪圖示![](assets/gear-icon-settings.png)。

   並非下列所有選項會同時顯示在此下拉式功能表中。 例如，只有在選取其他兩個選項之一時，才會顯示第二個選項。

   * **讓此專案在系統範圍內可編輯，讓Workfront中的每個人都可以編輯它** （預設選項）

     當您新增自訂欄位或Widget且您未限制其共用時，系統中有權存取自訂表單的所有人都可以檢視並編輯其屬性。

   * **移除系統範圍編輯存取權**

     限制只有您已新增至清單的使用者才可存取。

   * **讓此專案在整個系統內可見，讓Workfront中的每個人都可以看到它**

1. 按一下&#x200B;**儲存**&#x200B;或&#x200B;**儲存+關閉**。

## 共用自訂表單時繼承對自訂欄位和Widget的存取權

當有人與群組、工作角色、團隊或公司共用自訂表單時，收件者會繼承對表單上任何自訂欄位和Widget的檢視存取權。 對表單上這些專案的這種存取層級一律會保留，以便表單可以按照建立者的預期為收件者運作。 即使是擁有表單編輯存取權的收件者，亦是如此。

您可以瞭解誰繼承了自訂欄位或Widget的存取權，並且可以移除其存取權。

>[!NOTE]
>
>如果收件者擁有共用自訂表單上自訂欄位或Widget的管理存取權，該存取權會保留給收件者。

* [瞭解誰繼承了自訂欄位或Widget的存取權](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [移除對自訂欄位或共用自訂表單中Widget的存取權](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 瞭解誰繼承了自訂欄位或Widget的存取權 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 按一下&#x200B;**欄位**，然後選取欄位、影像或存取Widget。
1. 在顯示的方塊中，按一下&#x200B;**繼承許可權**&#x200B;並檢視顯示的名稱。
1. 按一下&#x200B;**取消**。

### 移除對自訂欄位或共用自訂表單中Widget的存取權 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要移除對自訂欄位或共用之自訂表單中Widget的存取權，則需要取消共用表單。 如需指示，請參閱文章[共用自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)中的[移除自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare)存取權一節。
