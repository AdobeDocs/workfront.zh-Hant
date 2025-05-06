---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任務區域建立前置任務關係
description: 您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 使用前置任務區域建立前置任務關係

<!-- Audited: 5/2025 -->

您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，您傳送邀請（前置任務）之前，不想主持一方（相依任務）。

本文說明如何使用任務中的「前置任務」標籤來設定前置任務。

如需有關在任務清單中設定前置任務的資訊，請參閱[在任務清單上建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)。

您可以在Adobe Workfront的下列區域中檢視前置任務：

* 在相依任務的「前置任務」區段中
* 在甘特圖中
* 在「前置任務」欄的工作清單中

有關前置任務的資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

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
   <p>新增：標準 </p>
   <p>或 </p>
   <p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件的存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立任務的前置任務

1. 瀏覽至要指定為相依性工作的工作。

1. 在左側面板中，按一下&#x200B;**前置任務**。

1. 在&#x200B;**前置任務**&#x200B;區段中，按一下&#x200B;**+新增前置任務**。 **新增前置任務**&#x200B;對話方塊開啟。

1. （選擇性）若要新增跨專案前置任務，請將&#x200B;**父專案**&#x200B;欄位中的專案名稱取代為其他專案。

   如需詳細資訊，請參閱[建立跨專案前置任務](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。

1. 在&#x200B;**任務**&#x200B;欄位中，輸入您要指定做為前置任務的一個或多個任務的名稱，然後在它們出現在下拉式清單中時選取它們。

1. 選取&#x200B;**相依性型別**。

   如需詳細資訊，請參閱[任務相依性型別的概觀](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. 輸入&#x200B;**延遲**&#x200B;量。

   如需詳細資訊，請參閱{&#x200B;0}延遲型別概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md)。[

   ![新增前置任務對話方塊](assets/add-predecessor-dialog-box.png)

1. 如果要強制兩個任務之間的前置任務關係，請選取&#x200B;**強制**&#x200B;核取方塊。

   如需詳細資訊，請參閱[強制執行前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

1. 按一下「**儲存**」。
