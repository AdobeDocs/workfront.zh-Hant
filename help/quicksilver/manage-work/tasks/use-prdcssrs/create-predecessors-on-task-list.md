---
product-area: projects
navigation-topic: use-predecessors
title: 在任務清單上建立前置任務關係
description: 您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# 在任務清單上建立前置任務關係

<!-- Audited: 5/2025 -->

您可以使用前置任務（或只是前置任務）來連結依賴其他任務開始或完成的任務。 例如，在傳送邀請（前置任務）之前，您不想主持一方（相依任務）。

本文說明如何在任務清單中建立前置任務。

您可以在Adobe Workfront的下列區域中檢視前置任務：

* 在「前置任務」欄的工作清單中。
* 在甘特圖中。
* 在相依任務的「前置任務」區段中。

如需詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>新增：標準 </p><p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立前置任務

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上選取專案。
1. 按一下左側面板中的&#x200B;**工作**。
1. 在&#x200B;**檢視**&#x200B;下拉式清單中，選取顯示&#x200B;**前置任務**&#x200B;欄的檢視，或將欄新增至您目前的檢視。

1. 選取要指定為相依性工作的工作。
1. 按一下任務的&#x200B;**前置任務**&#x200B;欄。
1. 輸入您要指定為所選任務之前置任務的任務編號，然後按&#x200B;**Enter**。

   >[!TIP]
   >
   >若要新增跨專案前置任務，請執行下列動作：
   >
   >1. 按一下&#x200B;**計畫模式**&#x200B;圖示，然後選擇&#x200B;**自動儲存**。
   >
   >1. 輸入前置任務專案的「參考編號」，後面加上冒號和任務編號。 例如，輸入&#x200B;*765021：12*&#x200B;表示前置任務專案的參考號碼為765021，而前置任務為專案上的任務號碼12。
   >
   >1. 新增此前置任務的相依性型別。 如需詳細資訊，請參閱[建立跨專案前置任務](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。
   >
   >1. 按&#x200B;**Enter**。
   >
   >**重要**
   >
   >當任務清單以手動儲存模式顯示時，您無法新增跨專案前置任務。

   前置任務被標示為完成時，前置任務圖示會變成綠色。 這表示相依任務已準備好工作。

   如需「前置任務」欄中可用關聯性型別的詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 檢視前置任務詳細資訊

您可以從任務清單中快速檢視有關前置任務的詳細資訊。

1. 在任務清單上，將游標停留在&#x200B;**前置任務**&#x200B;欄中的前置任務編號上。 隨即顯示含有前置任務詳細資訊的方塊。

   ![前置任務詳細資料](assets/predecessor-details-in-task-list.png)

   會顯示下列詳細資料：

   **前置任務名稱：**&#x200B;被參考的前置任務名稱。 已包含前置任務的任務編號。 按一下工作名稱以開啟它。

   **專案名稱：**&#x200B;前置任務所在的專案名稱。 如果前置任務屬於與任務相同的專案，則會將該專案識別為目前專案；如果前置任務屬於不同的專案，則會將該專案識別為跨專案。 如需跨專案前置任務的詳細資訊，請參閱[建立跨專案前置任務](../../tasks/use-prdcssrs/cross-project-predecessors.md)。

   您可以展開專案詳細資料以檢視專案的計劃開始和結束日期、條件、狀態、完成百分比以及擁有者。 如果是跨專案，您可以按一下&#x200B;**檢視專案**&#x200B;以開啟專案。

   **ID：**&#x200B;前置任務所在專案的參考號碼。

   **計劃開始：**&#x200B;前置任務的計劃開始日期。

   **計畫結束：**&#x200B;前置任務的計畫完成日期。

   **前置任務數目：**&#x200B;被參考的前置任務的前置任務數目。

   **後續任務的數目：**&#x200B;參考之前置任務的後續任務（或相依）數目。
