---
product-area: projects
navigation-topic: create-tasks
title: 建立子任務
description: 在Adobe Workfront中，任務可以有父子關係。 子任務稱為子任務。 您可以將主要任務設為子任務，以在任務清單中建立子任務。 您也可以將子任務設為主要任務。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 建立子任務

<!-- Audited: 01/2025 -->

在Adobe Workfront中，任務可以有父子關係。 子任務稱為子任務。 您可以將主要任務設為其他任務的子任務，以在任務清單中建立子任務。 您也可以將子任務設為主要任務。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>為專案貢獻許可權，並可新增任務或以上專案</p> 
   <p>建立任務時，您會自動收到該任務的「管理」許可權</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 建立子任務

您可以從任務清單或任務子任務區段建立子任務。

>[!TIP]
>
>為專案建立子任務類似於在範本上建立範本子任務以範本任務。


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
>您的Workfront或群組管理員可能會使用版面配置範本移除您環境中的「子任務」區段。

1. 前往您要建立子任務的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;區段。
1. 按一下要建立子任務的工作名稱。
1. 按一下左側面板中的&#x200B;**子任務**&#x200B;區段（如果有的話）。
1. 按一下&#x200B;**新增工作。**

   如需有關建立任務的資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

1. 按一下&#x200B;**建立任務。**

   新任務會建立為您在步驟3中所選任務的子任務。<!--ensure this is accurate-->

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
