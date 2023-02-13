---
product-area: projects
navigation-topic: create-tasks
title: 建立子任務
description: 在Workfront中，任務可以有父子關係。 子任務稱為子任務。 通過將主任務設定為子任務，可以在任務清單上建立子任務。 您也可以將子任務設為主要任務。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: fb1f4e609e0cc2b0e9e4d0b36b7ace3fd8937d26
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 建立子任務

在Workfront中，任務可以有父子關係。 子任務稱為子任務。 通過將主任務設定為子任務，可以在任務清單上建立子任務。 您也可以將子任務設為主要任務。

## 存取需求

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 有關訪問任務的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任務的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為項目和父任務提供權限，並能夠添加任務或更高版本</p> <p>建立任務後，您會自動收到該任務的「管理」權限</p> <p> 有關任務權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用任務 </a>. </p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立子任務

* [從任務清單建立子任務](#create-subtasks-from-the-task-list)
* [從任務子任務部分建立子任務](#create-subtasks-from-the-task-subtasks-section)

### 從任務清單建立子任務 {#create-subtasks-from-the-task-list}

1. 前往您要建立子任務的專案。
1. 按一下 **工作** 區段。
1. （條件性）如果要建立子任務的任務尚未直接位於要建立父任務的任務下，請將其拖動到任務清單中的適當位置。
1. 選擇要建立子任務的任務，並執行以下操作之一：

   * 按一下 **縮進** 圖示 ![](assets/indent-icon-nwe-33x29.png) 使所選任務成為其上方任務的子任務。
   * 使用標準英文QWERTY鍵盤時，請在鍵盤上按Option + >(Mac)或Alt + >(Windows)。 其他語言可能會使用Option + 、(Mac)或Alt + 、(Windows)命令進行縮進。

      >[!TIP]
      >
      >在內嵌編輯中編輯任務時，鍵盤快速鍵無法運作。 在這種情況下，請使用「縮進」表徵圖 ![](assets/cs1.png) 來建立子任務。

   * 將任務拖放到要指定為父任務的任務上。
   >[!NOTE]
   >
   >僅當任務清單按任務編號排序時，以及沒有對任務清單應用分組時，才可縮進任務。

### 從任務子任務部分建立子任務 {#create-subtasks-from-the-task-subtasks-section}

1. 前往您要建立子任務的專案。
1. 按一下 **工作** 區段。
1. 按一下要建立子任務的任務的名稱。
1. 按一下 **子任務** 區段。
1. 按一下 **新任務。**

   請依照下列文章中的步驟繼續建立子任務： [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. 按一下 **保存任務。**

## 將子任務設為主任務

1. 轉至要將子任務設定為主要任務的項目。
1. 按一下 **工作** 區段。
1. 選擇要執行主任務的子任務。
1. 按一下 **輸出** 圖示 ![](assets/outdent-icon-nwe-31x29.png) 使子任務成為主任務。

   或

   在標準英文QWERTY鍵盤上，按Option + &lt;(Mac)或Alt + &lt;(Windows)。 其他語言可能會使用命令Option + 。 (Mac)或Alt + 。 (Windows)取代。

   >[!NOTE]
   >
   >僅當任務清單按任務編號排序時，以及沒有對任務清單應用分組時，才能輸出任務。
