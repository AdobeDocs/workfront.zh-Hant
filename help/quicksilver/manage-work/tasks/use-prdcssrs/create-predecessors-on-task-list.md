---
product-area: projects
navigation-topic: use-predecessors
title: 在任務清單上建立前置關係
description: 您可以使用前置任務（或僅前置任務）來連結依賴其他任務啟動或完成的任務。 例如，在發送邀請（前置任務）之前，您不想主機某個交易方（相關任務）。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 在任務清單上建立前置關係

您可以使用前置任務（或僅前置任務）來連結依賴其他任務啟動或完成的任務。 例如，在發送邀請（前置任務）之前，您不想主機某個交易方（相關任務）。

本文說明如何在任務清單中建立前置任務。

您可以在下列Adobe Workfront區域中檢視前置任務：

* 在「前置任務」列的任務清單中。
* 在甘特圖中
* 在從屬任務的前置任務部分中

如需詳細資訊，請參閱 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>編輯對任務和項目的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務和專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立前置任務

1. 前往專案。
1. 按一下 **工作** 中。
1. 請確定您目前的檢視顯示 **前身** 欄。

   如果視圖未顯示前置項列，請更改為顯示前置項的視圖，或將該列添加到您的視圖中。

1. 選擇要指定為相依任務的任務。
1. 按一下內部 **前置任務** 欄。
1. 鍵入要指定為選定任務前置任務的任務編號，然後按鍵 **輸入**.

   前置任務標籤為完成時，前置任務表徵圖將變為綠色。 這表示相依任務已準備就緒可供使用。

   有關「前置項」(Preceverses)列中可用的關係類型的詳細資訊，請參見 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 查看前置項詳細資訊

您可以從任務清單中快速查看有關前置任務的詳細資訊。

1. 在任務清單中，將滑鼠移到 **前置任務** 欄。

   隨即顯示包含前置項詳細資訊的方塊。

   ![前置任務詳細資訊](assets/predecessor-details-in-task-list.png)

   會顯示下列詳細資料：

   **前置名稱：** 引用的前置項的名稱。 包括前置任務的任務編號。 按一下任務名稱以開啟它。 在上述範例中，前身是生產/執行/傳送。

   **項目名稱：** 前置項所在的項目的名稱。 如果前置項與任務屬於相同項目，則將項目標識為當前項目；如果前置項屬於不同項目，則將標識為交叉項目。 在上述範例中，專案名稱為「數位資產生產（整合） — 專案」。 如需跨專案前置作業的詳細資訊，請參閱 [建立跨專案的前置項目](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   您可以展開專案詳細資訊，查看專案的計劃開始和結束日期、條件、狀態、完成百分比及擁有者。 對於跨專案，您可以按一下 **請參閱專案** 來開啟專案。

   **ID:** 前置項所在項目的參考編號。

   **計劃開始：** 前置任務的計畫起始日期。

   **計畫結束：** 前置任務的計畫完成日期。

   **前置任務數：** 被引用的前置任務的數目。 在上例中，引用的前置有1個前置。

   **後繼者數：** 被引用的前身的後繼（或從屬）任務數。 在上例中，被引用的前置有1個後置。
