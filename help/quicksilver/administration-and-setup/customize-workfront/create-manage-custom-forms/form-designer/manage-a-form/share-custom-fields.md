---
title: 設定自訂欄位和Widget的共用
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 根據預設，當您新增自訂欄位或Widget至自訂表單時，系統中有權存取自訂表單的任何人都可以編輯該專案的屬性，例如其標籤和API名稱。 您可以透過控制誰可以與其共用來變更此專案。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1eda36eb74aca2b731f2632eac3aae60e6b8ef9d
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 2%

---

# 設定自訂欄位和Widget共用

根據預設，當您新增自訂欄位或Widget至自訂表單時，系統中有權存取自訂表單的任何人都可以編輯該專案的屬性，例如其標籤和API名稱。 您可以透過控制誰可以與其共用來變更此專案。

如需自訂表單中自訂欄位和Widget的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

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

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## 設定共用自訂欄位或Widget

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 若要從表單和欄位清單共用：

   1. 按一下&#x200B;**欄位**&#x200B;以開啟[欄位]區域。
   1. 選取您要共用的欄位，然後按一下![共用圖示](assets/share-icon.png)。

1. 若要從表單設計工具共用：
   1. 開啟自訂表單或建立新的自訂表單。
   1. 在表單設計工具中，選取您要共用的欄位，然後按一下右側欄位編輯區域中的&#x200B;**共用**。

1. 在共用方塊中，在&#x200B;**授與欄位存取權**&#x200B;下，開始輸入您要共用專案的使用者、團隊、工作角色、群組、公司或企業設定檔的名稱，然後在名稱顯示時按下&#x200B;**Enter**。
1. 如果您想更詳細地說明共用專案的方式，請按一下名稱右側的下拉式功能表，然後使用下列任一選項：

   * **檢視**：按一下&#x200B;**進階設定**&#x200B;圖示![進階設定圖示](assets/configure-options-icon.png)，指定您是否要讓使用者將專案新增至自訂表單，或是與其他使用者共用。
   * **管理**：允許存取以編輯自訂欄位，並在欄位程式庫和表單設計工具中檢視它。 按一下&#x200B;**進階設定**&#x200B;圖示![進階設定圖示](assets/configure-options-icon.png)，指定您是否要讓使用者能夠刪除系統上的專案，或是與其他使用者共用專案。

1. （可選）重複步驟5至6，將其他名稱新增至清單並設定其選項。
1. （選擇性）為欄位選擇全系統共用選項：

   * **系統中的每個人都可以編輯** （預設選項）

     當您新增自訂欄位或Widget且您未限制其共用時，系統中有權存取自訂表單的所有人都可以檢視並編輯其屬性。

   * **系統中的每個人都可以檢視**

     系統中有權存取自訂表單的所有人都可以檢視欄位但不能編輯它。

   * **只有受邀者可以存取**

     限制僅存取您新增至清單中的人員。

   ![共用選項](assets/share-field-in-designer.png)

1. 按一下「**儲存**」。

## 共用自訂表單時繼承對自訂欄位和Widget的存取權

當有人與群組、工作角色、團隊、公司或企業設定檔共用自訂表單時，收件者會繼承對表單上任何自訂欄位和Widget的檢視存取權。 對表單上這些專案的這種存取層級一律會保留，以便表單可以按照建立者的預期為收件者運作。 即使是擁有表單編輯存取權的收件者，亦是如此。

您可以瞭解誰繼承了自訂欄位或Widget的存取權，並且可以移除其存取權。

>[!NOTE]
>
>如果收件者擁有共用自訂表單上自訂欄位或Widget的管理存取權，該存取權會保留給收件者。

### 瞭解誰繼承了自訂欄位或Widget的存取權 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 按一下&#x200B;**欄位**，然後選取欄位、影像或存取Widget。
1. 在顯示的方塊中，按一下&#x200B;**繼承許可權**&#x200B;並檢視顯示的名稱。
1. 按一下&#x200B;**取消**。

### 移除對自訂欄位或共用自訂表單中Widget的存取權 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要移除對自訂欄位或共用之自訂表單中Widget的存取權，則需要取消共用表單。 如需指示，請參閱文章[共用自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)中的[移除自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form)存取權一節。


