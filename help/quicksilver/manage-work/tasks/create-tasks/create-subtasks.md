---
product-area: projects
navigation-topic: create-tasks
title: 建立子任務
description: 在Adobe Workfront中，任務可以有父子關係。 子任務稱為子任務。 您可以將主要任務設為子任務，以在任務清單中建立子任務。 您也可以將子任務設為主要任務。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 建立子任務

<!-- Audited: 01/2025 -->

在Adobe Workfront中，任務可以有父子關係。 子任務稱為子任務。 您可以將主要任務設為子任務，以在任務清單中建立子任務。 您也可以將子任務設為主要任務。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>新增：標準</p>
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>專案和父級任務的Contribute許可權（可新增任務或以上任務）</p> <p>您會在建立任務後自動收到該任務的「管理」許可權。</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立子任務

您可以從任務清單或任務子任務區段建立子任務。

### 從任務清單建立子任務 {#create-subtasks-from-the-task-list}

1. 前往您要建立子任務的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;區段。
1. （視條件而定）如果您要建立子項工作的工作尚未直接位於要建立父項工作的正下方，請將其拖放至工作清單中的適當位置。
1. 選取要建立子任務的工作，並執行下列任一項作業：

   * 按一下&#x200B;**縮排**&#x200B;圖示![](assets/indent-icon-nwe-33x29.png)，將選取的工作設為其正上方的子工作。
   * 使用標準英文QWERTY鍵盤時，在鍵盤上按Option + > (Mac)或Alt + > (Windows)。 其他語言可能會使用命令Option + 、 (Mac)或Alt + 、 (Windows)來縮排。

     >[!TIP]
     >
     >當您在內嵌編輯中編輯任務時，鍵盤快速鍵無法運作。 在此情況下，請使用縮排圖示![](assets/indent-icon-nwe-33x29.png)來建立子任務。

   * 將任務拖放到要指定為父系任務的任務上。

     >[!NOTE]
     >
     >只有當任務清單是依任務編號排序的，而且沒有群組套用到任務清單時，您才可以縮排任務。

### 從任務子任務區段建立子任務 {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>您的Workfront或群組管理員可能會隱藏環境中的子任務區段。

1. 前往您要建立子任務的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;區段。
1. 按一下要建立子任務的工作名稱。
1. 按一下左側面板中的&#x200B;**子任務**&#x200B;區段（如果有的話）。
1. 按一下&#x200B;**新增工作。**

   請依照下列文章中的步驟繼續建立子任務： [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

1. 按一下&#x200B;**建立任務。**

## 將子任務設為主要任務

1. 移至您想要將子任務設為主要任務的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;區段。
1. 選取您想要成為主要任務的子任務。
1. 按一下&#x200B;**減少縮排**&#x200B;圖示![](assets/outdent-icon-nwe-31x29.png)，將子工作設為主要工作。

   或

   在標準英文QWERTY鍵盤上，按下Option + &lt; (Mac)或Alt + &lt; (Windows)。 其他語言則可能會使用Option + 。 (Mac)或Alt + 。 (Windows)以縮排。

   >[!NOTE]
   >
   >只有當任務清單是依任務編號排序的，而且沒有群組套用到任務清單時，您才能減少任務數量。
