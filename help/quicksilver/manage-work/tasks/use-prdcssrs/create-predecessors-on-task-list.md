---
product-area: projects
navigation-topic: use-predecessors
title: 在任務清單上建立前置任務關係
description: 您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# 在任務清單上建立前置任務關係

您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。

本文說明如何在任務清單中建立前置任務。

您可以在Adobe Workfront的下列區域中檢視前置任務：

* 在「前置任務」欄的工作清單中。
* 在甘特圖中
* 在相依任務的前置任務區段中

如需詳細資訊，請參閱 [前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 存取需求

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準 </p><p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 建立前置任務

1. 前往專案。
1. 按一下 **任務** 在左側面板中。
1. 確定您目前的檢視顯示 **前置任務** 欄。

   如果檢視未顯示「前置任務」欄，請變更為顯示前置任務的檢視，或將欄新增至您的檢視。

1. 選取要指定為相依性工作的工作。
1. 按一下 **前置任務** 欄。
1. 輸入您要指定為所選任務的前置任務編號，然後按 **輸入**.

   >[!TIP]
   >
   >若要新增跨專案前置任務，請執行下列動作：
   >
   >1. 按一下 **計畫模式** 圖示並選擇 **自動儲存**.
   >
   >1. 輸入前置任務專案的「參考編號」，後面加上冒號和任務編號。 例如，輸入： 765021：12。 這表示前置任務專案的參考編號是765021，而前置任務是專案上的任務編號12。
   >
   >1. 新增此前置任務的相依性型別。 如需詳細資訊，請參閱 [建立跨專案前置任務](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >按下 **輸入**.
   >
   >**重要**
   >
   >當任務清單以手動儲存模式顯示時，您無法新增跨專案前置任務。

   前置任務被標示為完成時，前置任務圖示會變成綠色。 這表示相依任務已準備好工作。

   如需「前置任務」欄中可用關係型別的詳細資訊，請參閱 [前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) 在 [前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 檢視前置任務詳細資訊

您可以從任務清單中快速檢視有關前置任務的詳細資訊。

1. 在任務清單上，將滑鼠游標停留在 **前置任務** 欄。

   顯示含有前置任務詳細資訊的方塊。

   ![前置任務詳細資訊](assets/predecessor-details-in-task-list.png)

   會顯示下列詳細資料：

   **前置任務名稱：** 被參考的前置任務名稱。 已包含前置任務的任務編號。 按一下工作名稱以開啟它。 在上述範例中，前置任務為「生產/執行/傳送」。

   **專案名稱：** 前置任務所在的專案名稱。 如果前置任務屬於與任務相同的專案，則會將該專案識別為目前專案；如果前置任務屬於不同的專案，則會將該專案識別為跨專案。 在上述範例中，專案名稱為Digital Asset Production (Integrated) - Project。 如需跨專案前置任務的詳細資訊，請參閱 [建立跨專案前置任務](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   您可以展開專案詳細資料以檢視專案的計劃開始和結束日期、條件、狀態、完成百分比以及擁有者。 若為跨專案，您可以按一下 **檢視專案** 以開啟專案。

   **ID：** 前置任務所在專案的參考號碼。

   **計劃開始：** 前置任務的計劃開始日期。

   **計畫結束：** 前置任務的計畫完成日期。

   **前置任務數量：** 被參考的前置任務的前置任務數量。 在上述範例中，被參考的前置任務有1個前置任務。

   **後置任務數目：** 被參考的前置任務之後置任務（或相依任務）的數目。 在上述範例中，被參考的前置任務有1個後置任務。
