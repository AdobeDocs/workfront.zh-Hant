---
navigation-topic: use-the-gantt-chart
title: 將甘特圖匯出至PDF
description: 您可以將甘特圖匯出至PDF。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 匯出 [!UICONTROL 甘特圖] 至PDF

您可以匯出 [!UICONTROL 甘特圖] 到PDF。

匯出 [!UICONTROL 甘特圖] 若要PDF，您可以列印或附加至電子郵件，與其他使用者共用。

## 存取需求

您必須具備下列專案才能依照本文所述步驟操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]授權*</td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案和任務存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 匯出 [!UICONTROL 甘特圖]

1. 存取 [!UICONTROL 甘特圖] 要匯出至PDF的檔案，如所述 [開始使用 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 確定您已設定 [!UICONTROL 甘特圖] 以在匯出之前顯示適當的資訊。

   >[!NOTE]
   >
   >如果您匯出 [!UICONTROL 甘特圖] 從專案清單中，PDF檔案僅包含清單中的專案，而不包含每個專案上的任務。 如果您想要匯出任務清單，可以從與其關聯的專案中進行匯出，也可以建立任務報告並在中顯示報告結果。 [!UICONTROL 甘特檢視].

   您可以設定下列資訊：

   * 工作清單中所需的篩選器、檢視和群組。 檢視時，會保留清單檢視中所選的任何篩選器和群組。 [!UICONTROL 甘特圖]. 檢視會反映在匯出的上 [!UICONTROL 甘特圖] 僅顯示在「 」旁邊的 [!UICONTROL 甘特圖] 在第一頁上。 檢視不會顯示在 [!UICONTROL 甘特圖] 本身。

     >[!TIP]
     >
     >為「 」提供更多空間 [!UICONTROL 甘特圖] 它本身會套用包含儘可能少欄的檢視。

   * 上的設定選項 [!UICONTROL 甘特圖]. 例如，您可以啟用里程碑、日期、 [!UICONTROL 基準線]，或 [!UICONTROL 完成百分比] 顯示於 [!UICONTROL 甘特圖].

     如需詳細資訊，請參閱   [設定資訊在 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > 指派不會顯示在 [!UICONTROL 甘特圖] 當 [!UICONTROL 甘特圖] 會匯出至PDF。 當 [!UICONTROL 甘特圖] 會匯出至PDF，指派只會顯示在清單檢視中。

   * 顯示在「 」上的時段 [!UICONTROL 甘特圖].\

     如需詳細資訊，請參閱 [在中檢視資訊 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     時間週期在匯出檔案中的顯示方式取決於您是否選取 **[!UICONTROL 我看到的內容]** 或 **[!UICONTROL 多頁]** 在稍後的步驟中。

1. （選擇性）若要在匯出的PDF中僅包含某些工作，請選取您要包含的工作。

   如果您未選取任何任務，則所有任務都會包含在匯出的PDF中。

   例如，如果您檢視的是 [!UICONTROL 甘特圖] 針對包含50項任務，但您想在匯出的專案上只顯示10項任務的專案 [!UICONTROL 甘特圖]，選取您要顯示的10項工作。

1. 按一下印表機圖示。\
   此 **[!UICONTROL 匯出至PDF]** 對話方塊隨即顯示。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 選擇您是隻想匯出您所看到的內容，還是想匯出整個 [!UICONTROL 甘特圖]：

   * **[!UICONTROL 我看到的內容]：** 匯出最多500個專案之前，會匯出畫面上顯示的所有任務（包括任何子任務）。 (這並非下列專案中所顯示的內容： **[!UICONTROL 預覽]** 區段； [!UICONTROL 預覽] 區段僅包含範例資料。)

     即使父任務已摺疊且子任務不可見，子任務也會包含在匯出的PDF中。 若只要包含父系任務，請選取要包含的父系任務，並保留任何子任務為未選取。

     您可以使用 **[!UICONTROL 縮放為]** 下拉式功能表或滑桿工具，只顯示 [!UICONTROL 甘特圖]，如所述 [在中檢視資訊 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 多頁]：** 匯出整個 [!UICONTROL 甘特圖]，即使是未在目前熒幕顯示的專案，也有500個專案。\

     您可以使用 **[!UICONTROL 縮放為]** 下拉式功能表或滑桿工具來決定每個頁面上要顯示的資訊量，如中所述 [設定資訊在 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 選取較精細的選項以顯示更多要匯出的頁面，或選取較精細的選項以顯示較少要匯出的頁面。

     >[!NOTE]
     >
     >如果您需要匯出 [!UICONTROL 甘特圖] 若包含500多個專案，請先將篩選器套用至清單，再檢視 [!UICONTROL 甘特圖] 以便顯示少於500個專案或250個頁面。 如需如何套用篩選的詳細資訊，請參閱  [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >在下列情況下，無法匯出整個甘特圖：
     >
     >   
     >   
     >   * 跨越250頁時
     >   * 當它包含超過500個專案




1. 如果PDF在匯出至PDF後會列印，請在 **[!UICONTROL 頁面大小]** 下拉式功能表，選取您要列印的紙張大小。\
   您可以選取 **[!UICONTROL 字母]**， **[!UICONTROL 法律]**， **[!UICONTROL Ledger]**， **[!UICONTROL A1]**， **[!UICONTROL A2]**， **[!UICONTROL A3]** （僅適用於某些語言），或 **[!UICONTROL A4]**.
1. 在 **[!UICONTROL 頁面方向]** 區段，選取您要以橫向或縱向匯出PDF。
1. 選取 **[!UICONTROL 顯示圖例]** 如果您想要在匯出的PDF中包含圖例。
1. 按一下 **[!UICONTROL 匯出]**.

   的pdf [!UICONTROL 甘特圖] 已建立並下載至您的電腦。

   請注意匯出檔案底部的圖例。 它僅說明您已在「 」中啟用的選項 [!UICONTROL 甘特圖] 以及工作清單中可用的專案。

   例如，只有在您至少有一個工作與里程碑相關聯時，里程碑才會顯示在圖例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
