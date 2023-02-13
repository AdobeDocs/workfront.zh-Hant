---
title: 轉換物件時傳輸自訂表單資料
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 當工作項中定義的工作變得過大時，您可以將其轉換為較大的工作項。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 轉換物件時傳輸自訂表單資料

根據貴組織的業務需要，任務或問題中定義的工作可能會變得過大，無法在任務或問題中管理它。 在這種情況下，您可以將它們轉換為較大的工作項目：

* 您可以將問題轉換為工作或專案
* 您可以將任務轉換為專案

若要將自訂表單資料從問題傳輸至任務或專案，您必須依照下列順序完成本文中的兩個工作。

如需詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md) 或 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## 第一：複製自訂表單 {#first-copy-the-custom-form}

首先，您需要確保保留要轉換的任務或問題上的任何自定義表單資料。 由於自訂表單資料必須與轉換的項目完全相符，因此最佳作法是複製表單，以便您將其附加至新物件。

>[!TIP]
>
>在此情況下，保留自訂表單資料的另一種方法是將較大的物件類型新增至自訂表單。 如需指示，請參閱 [開始編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) 在文章中 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms**.
1. 選擇任務類型或問題類型自定義表單，然後按一下 **複製**.
1. 在 **自訂表單** 對話框，指定新表單的名稱。

1. 從 **表單類型** 下拉式選單中，選擇要建立新自訂表單的對象類型

   **範例：** 如果要將自訂表單資料傳輸至專案，請選取「專案」。

1. 按一下 **複製表單**.

   現在可將此複製的自訂表單附加至任務或專案。

1. 繼續 [第二：轉換問題或任務並傳輸自訂表單資料](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 第二：轉換問題或任務並傳輸自訂表單資料 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 複製您要轉換的問題或任務的自訂表單，如 [第一：複製自訂表單](#first-copy-the-custom-form) 這篇文章。
1. 使用 **自訂Forms** 選項，以選取您複製的自訂表單。 如需指示，請參閱下列文章：

   * [將問題轉換為Adobe Workfront中的專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [將問題轉換為Adobe Workfront中的任務](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [將任務轉換為項目](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 在 **轉換為（物件類型）** 對話框，按一下 **新增Forms** 下拉式選單中，並選取您在上一節中複製的表單。

   在問題的自訂欄位中擷取的資訊現在會傳輸至任務上的自訂表單。

