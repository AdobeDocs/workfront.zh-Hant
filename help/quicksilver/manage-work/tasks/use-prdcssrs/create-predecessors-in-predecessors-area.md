---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任務區域建立前置任務關係
description: 您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 使用前置任務區域建立前置任務關係

您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。

本文說明如何使用任務中的「前置任務」標籤來設定前置任務。

如需有關在任務清單中設定前置任務的資訊，請參閱 [在任務清單上建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

您可以在Adobe Workfront的下列區域中檢視前置任務：

* 在相依任務的「前置任務」區段中
* 在甘特圖中
* 在「前置任務」欄的工作清單中

有關前置任務的資訊，請參閱 [前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 建立任務的前置任務

1. 移至要指定為相依性工作的工作，然後按一下 **前置任務** 在左側面板中。

   您可能需要按一下 **顯示更多**，然後 **前置任務**.

1. 按一下 **+新增前置任務**.
1. （可選）若要新增跨專案前置任務，請在以下位置取代專案名稱： **父級專案** 欄位中指定其他專案，然後輸入您想要作為前置任務的一個或多個任務的名稱。

   如需關於新增跨專案前置任務的資訊，請參閱 [建立跨專案前置任務](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 輸入您要指定為前置任務的一或多個任務的名稱。

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. 選取 **相依性型別**.

   如需有關作業「相依性型別」的資訊，請參閱 [作業相依性型別的概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **延遲** 以天為單位的金額。

   如需延遲型別的相關資訊，請參閱&#x200B;。 [延遲型別概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 選取 **強制** 如果要強制兩個任務之間的前置任務關係。

   如需強制前置任務的相關資訊，請參閱 [強制執行前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. 按一下「**儲存**」。
