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
TQID: https://experienceleague.adobe.com/qreUbwUFma8OVt5z0Nyiex3c-MWoiN5jPRM-Bgl7ev8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 388
ht-degree: 4%

---

# 轉換物件時傳輸自訂表單資料

根據您組織的業務需求，任務或問題中定義的工作可能會變得太大，無法在任務或問題中管理。 在這種情況下，您可以將它們轉換為較大的工作專案：

* 您可以將問題轉換為任務或專案
* 您可以將任務轉換為專案

若要將自訂表單資料從問題傳輸至任務或專案，您必須依照以下順序完成本文中的兩個任務。

如需詳細資訊，請參閱[在Adobe Workfront中轉換問題的總覽](../../../manage-work/issues/convert-issues/convert-issues.md)或[在Adobe Workfront中轉換問題的總覽](../../../manage-work/issues/convert-issues/convert-issues.md)。

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

## 第一：新增其他物件至自訂表單

{{step-1-to-setup}}

1. 按一下&#x200B;**自訂Forms**。
1. 尋找您需要的表單，然後按一下![編輯圖示](assets/edit-icon.png)。
1. 在表單頂端，新增您計畫轉換任務或問題的物件。

   >[!INFO]
   >
   >**範例**：如果您想要將自訂表單資料傳輸至專案，請選取[專案]。

1. 按一下表單底部的&#x200B;**套用**。

1. 繼續到[秒：轉換問題或任務並傳輸自訂表單資料](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data)。

## 第二：轉換問題或任務並傳輸自訂表單資料 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 在您要轉換的問題或任務上新增其他物件至自訂表單，如本文中[第一：新增其他物件至自訂表單](#first-add-additonal-objects-to-the-custom-form)小節所述。
1. 使用顯示的方塊中的&#x200B;**自訂Forms**&#x200B;選項轉換問題或任務，以選取您需要的自訂表單。 如需指示，請參閱下列文章：

   * [將問題轉換為專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [將問題轉換為任務](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [將任務轉換為專案](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 在顯示的&#x200B;**轉換成（物件型別）**&#x200B;對話方塊中，按一下&#x200B;**新增Forms**&#x200B;下拉式功能表，並選取您在上一節中複製的表單。

   在問題的自訂欄位中擷取的資訊現在已轉移到任務上的自訂表單。


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->
