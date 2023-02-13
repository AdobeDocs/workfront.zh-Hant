---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任務區域建立前置任務關係
description: 您可以使用前置任務（或僅前置任務）來連結依賴其他任務啟動或完成的任務。 例如，在發送邀請（前置任務）之前，您不想主機某個交易方（相關任務）。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 使用前置任務區域建立前置任務關係

您可以使用前置任務（或僅前置任務）來連結依賴其他任務啟動或完成的任務。 例如，在發送邀請（前置任務）之前，您不想主機某個交易方（相關任務）。

本文說明如何使用任務中的「前置任務」頁簽來設定前置任務。

有關在任務清單中設定前置任務的資訊，請參見 [在任務清單上建立前置關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

您可以在下列Adobe Workfront區域中檢視前置任務：

* 在從屬任務的前置任務部分中
* 在甘特圖中
* 在「前置任務」列的任務清單中

有關前置任務的資訊，請參閱 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務和專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 為任務建立前置任務

1. 轉到要指定為相依任務的任務，然後按一下 **前置任務** 中。

   您可能需要按一下 **顯示更多**，然後 **前置任務**.

1. 按一下 **+添加前置項**.
1. （可選）若要新增跨專案前置項目，請取代 **上層專案** 欄位，然後鍵入要作為前置任務的任務或任務的名稱。

   如需新增跨專案前置作業的相關資訊，請參閱 [建立跨專案的前置項目](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 鍵入要指定為前置任務的任務或任務的名稱。

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. 選取 **相依類型**.

   有關任務依賴關係類型的資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **延遲** 天數。

   如需延遲類型的相關資訊，請參&#x200B;閱 [延遲類型概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 選擇 **強制** 如果要執行兩個任務之間的前置關係。

   有關強制前置任務的資訊，請參閱 [強制前置作業](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. 按一下&#x200B;**儲存**。
