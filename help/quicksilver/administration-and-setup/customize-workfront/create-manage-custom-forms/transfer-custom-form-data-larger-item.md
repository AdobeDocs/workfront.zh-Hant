---
title: 轉換物件時傳輸自訂表單資料
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 當在工作專案中定義的工作變得太大時，您可以將其轉換為較大的工作專案。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 轉換物件時傳輸自訂表單資料

根據您組織的業務需求，任務或問題中定義的工作可能會變得太大，無法在任務或問題中管理。 在這種情況下，您可以將它們轉換為較大的工作專案：

* 您可以將問題轉換為任務或專案
* 您可以將任務轉換為專案

若要將自訂表單資料從問題傳輸至任務或專案，您必須依照以下順序完成本文中的兩個任務。

如需詳細資訊，請參閱 [在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md) 或 [在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

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

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 第一：新增其他物件至自訂表單

{{step-1-to-setup}}

1. 按一下 **自訂Forms**.
1. 尋找所需的表單，然後按一下 ![編輯圖示](assets/edit-icon.png).
1. 在表單頂端，新增您計畫轉換任務或問題的物件。

   >[!INFO]
   >
   >**範例**：如果您想要將自訂表單資料傳輸至專案，請選取「專案」。

1. 按一下 **套用** 在表單底部。

1. 繼續前往 [第二：轉換問題或任務並傳輸自訂表單資料](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 第二：轉換問題或任務並傳輸自訂表單資料 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 按照一節中的說明，在轉換的問題或任務上，將其他物件新增到自訂表單 [第一：新增其他物件至自訂表單](#first-add-additonal-objects-to-the-custom-form) 本文章內容。
1. 使用轉換問題或任務 **自訂Forms** 方塊中的選項，用於選取您需要的自訂表單。 如需指示，請參閱下列文章：

   * [在Adobe Workfront中將問題轉換為專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [在Adobe Workfront中將問題轉換為任務](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [將任務轉換為專案](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 在 **轉換為（物件型別）** 對話方塊中，按一下 **新增Forms** 下拉式功能表，並選取您在上一節中複製的表單。

   在問題的自訂欄位中擷取的資訊現在已轉移到任務上的自訂表單。


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->