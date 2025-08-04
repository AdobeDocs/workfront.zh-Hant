---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任務區域建立前置任務關係
description: 您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '469'
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

+++ 展開以檢視存取需求。

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
   <p>標準 </p>
    <p>規劃 </p> </td> 
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

使用「前置任務」區域為專案任務建立前置任務，類似於為範本上的範本任務建立前置任務。

若要為專案任務建立前置任務：

1. 瀏覽至要指定為相依性工作的工作。

1. 在左側面板中，按一下&#x200B;**前置任務**。

1. 在&#x200B;**前置任務**&#x200B;區段中，按一下&#x200B;**新增前置任務**。 **新增前置任務**&#x200B;對話方塊開啟。

1. （選擇性）若要新增跨專案前置任務，請將&#x200B;**父專案**&#x200B;欄位中的專案名稱取代為其他專案。

   如需詳細資訊，請參閱[建立跨專案前置任務](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。

   >[!TIP]
   >
   >您無法為範本任務建立跨範本前置任務。


1. 在&#x200B;**任務**&#x200B;欄位中，輸入您要指定做為前置任務的一個或多個任務的名稱，然後在它們出現在下拉式清單中時選取它們。

1. 選取&#x200B;**相依性型別**。

   如需詳細資訊，請參閱[任務相依性型別的概觀](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. 輸入&#x200B;**延遲**&#x200B;量。

   如需詳細資訊，請參閱{&#x200B;0}延遲型別概觀[。](../../../manage-work/tasks/use-prdcssrs/lag-types.md)

   ![新增前置任務對話方塊](assets/add-predecessor-dialog-box.png)

1. 如果要強制兩個任務之間的前置任務關係，請選取&#x200B;**強制**&#x200B;核取方塊。

   如需詳細資訊，請參閱[強制執行前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

1. 按一下「**儲存**」。

1. （選擇性）若要移除前置任務，請從前置任務清單中選取它，然後按一下&#x200B;**移除**&#x200B;圖示![移除圖示](assets/remove-or-delete-icon.png)。

   前置任務會從清單中移除。 前置任務未從其專案中刪除。
