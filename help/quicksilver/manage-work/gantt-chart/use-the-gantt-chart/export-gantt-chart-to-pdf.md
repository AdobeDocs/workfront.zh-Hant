---
navigation-topic: use-the-gantt-chart
title: 將甘特圖匯出至PDF
description: 您可以將甘特圖匯出至PDF。 將甘特圖匯出至PDF後，您可以列印或附加至電子郵件，以便與其他使用者共用。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 1%

---

# 將[!UICONTROL 甘特圖]匯出至PDF

<!--Audited: 09/2024-->

您可以將[!UICONTROL 甘特圖]匯出至PDF。

將[!UICONTROL 甘特圖]匯出至PDF後，您可以列印或附加至電子郵件，以與其他使用者共用。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>新增：[！UICONTROL Light]或更高</p>
   <p>目前：[！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案和任務存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 匯出[!UICONTROL 甘特圖]

1. 存取您要匯出至PDF的[!UICONTROL 甘特圖]，如[開始使用[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)中所述。
1. 在匯出之前，請確定您已將[!UICONTROL 甘特圖]設定為顯示適當的資訊。

   >[!NOTE]
   >
   >如果您從專案清單匯出[!UICONTROL 甘特圖]，PDF檔案將僅包含清單中的專案，而不包含每個專案上的任務。 如果要匯出任務清單，可以從與其關聯的專案中匯出，也可以建立任務報告並在[!UICONTROL 甘特圖]中顯示報告結果。

   設定下列任一資訊：

   * 按一下[!UICONTROL 甘特圖]上方的&#x200B;**篩選器**、**檢視**&#x200B;和&#x200B;**群組**&#x200B;圖示，並新增或編輯套用至[!UICONTROL 甘特圖]中專案清單的現有篩選器、檢視或群組。

     檢視[!UICONTROL 甘特圖]時，會保留清單檢視中選取的任何篩選器和群組。 檢視只會在第一頁的[!UICONTROL 甘特圖]旁顯示的清單中，反映在匯出的[!UICONTROL 甘特圖]上。 檢視不會顯示在[!UICONTROL 甘特圖]本身。

     >[!TIP]
     >
     >若要讓[!UICONTROL 甘特圖]本身有更多空間，請套用包含儘可能少欄的檢視。

   * 選取&#x200B;**切換至預計日期**&#x200B;選項以檢視預計日期而非計畫日期。 依預設，會顯示計畫日期。

   * 按一下甘特圖右上角的&#x200B;**設定**&#x200B;圖示![設定圖示](assets/settings-icon.png)，並選取您想在甘特圖中檢視哪些資訊。 選取後，此資訊會包含在匯出的甘特PDF檔案中。

     從下列選項中選取：

      * 實際日期
      * 指派
      * 基準線
      * 認可日期
      * 完成百分比
      * 關鍵路徑
      * 里程碑菱形
      * 里程碑線
      * 前置任務
      * 進度狀態
      * 計畫日期

     如需詳細資訊，請參閱   [設定資訊在[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的顯示方式。

     >[!NOTE]
     >
     > 將[!UICONTROL 甘特圖]匯出至PDF時，[!UICONTROL 甘特圖]上不會顯示指派。 將[!UICONTROL 甘特圖]匯出至PDF時，指派僅會顯示在清單檢視中。

   * 顯示在[!UICONTROL 甘特圖]上的時段。

     如需詳細資訊，請參閱[檢視[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的資訊。

     期間在匯出檔案中的顯示方式取決於您選取了&#x200B;**[!UICONTROL 我看到的內容]**&#x200B;或在後續步驟中選取了&#x200B;**[!UICONTROL 多頁]**。

1. （可選）若只要在匯出的PDF中包含某些工作，請選取您要包含的工作。

   如果您未選取任何任務，則所有任務都會包含在匯出的PDF中。

   例如，如果您正在檢視包含50個任務的專案的[!UICONTROL 甘特圖]，但您只想在匯出的[!UICONTROL 甘特圖]上顯示10個任務，請選取您要顯示的10個任務。

1. 按一下甘特圖右上角的印表機圖示![印表機圖示](assets/printer-icon.png)。
顯示**[!UICONTROL 匯出至PDF]**&#x200B;對話方塊。

   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 在&#x200B;**匯出**&#x200B;區段中，從下列選項中選取，以指出您是隻想匯出您所看到的內容，還是想匯出整個[!UICONTROL 甘特圖]：

   * **[!UICONTROL 我看到的內容]：**&#x200B;匯出在匯出最多500個專案之前顯示在畫面上的所有任務（包括任何子任務）。 （**[!UICONTROL 預覽]**&#x200B;區段中並未顯示這個專案；[!UICONTROL 預覽]區段僅包含範例資料。）

     即使父任務已摺疊且子任務不可見，子任務也會包含在匯出的PDF中。 若只要包含父系任務，請選取要包含的父系任務，並保留任何子任務為未選取。

     >[!TIP]
     >
     >您可以使用&#x200B;**[!UICONTROL 縮放為]**&#x200B;下拉式功能表或滑桿工具，只顯示[!UICONTROL 甘特圖]的一部分，如[檢視[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的資訊中所述。


   * **[!UICONTROL 多個頁面]：**&#x200B;匯出整個[!UICONTROL 甘特圖]，即使它在目前熒幕上不可見，最多500個專案。

     >[!NOTE]
     >
     >* 您可以使用&#x200B;**[!UICONTROL 縮放至]**&#x200B;下拉式功能表或滑桿工具來決定每個頁面上顯示的資訊量，如[設定[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上資訊的顯示方式。 選取較精細的選項以顯示更多要匯出的頁面，或選取較精細的選項以顯示較少要匯出的頁面。
     >
     >* 如果您需要匯出包含超過500個專案的[!UICONTROL 甘特圖]，請在檢視[!UICONTROL 甘特圖]之前先將篩選器套用至清單，以便顯示少於500個專案或250頁。 如需如何套用篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
     >
     >
     >* 在下列情況下，無法匯出整個甘特圖：
     >   
     >   * 跨越250頁時
     >   * 當它包含超過500個專案


1. 如果PDF在匯出到PDF之後會列印，請在&#x200B;**[!UICONTROL 頁面大小]**下拉式功能表中，選取您要列印的紙張大小。
您可選取下列選項：

   * **[!UICONTROL 字母]**
   * **[!UICONTROL 法律]**
   * **[!UICONTROL 分類帳]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** （僅適用於某些語言）
   * **[!UICONTROL A4]**
1. 在&#x200B;**[!UICONTROL 頁面方向]**&#x200B;區段中，選取您要橫向或縱向匯出PDF。
1. 若要在匯出的PDF中包含圖例，請選取&#x200B;**[!UICONTROL 顯示圖例]**。
1. 按一下&#x200B;**[!UICONTROL 匯出]**。

   [!UICONTROL 甘特圖]的PDF已建立並下載至您的電腦。

   請注意匯出檔案底部的圖例。 它僅說明您在[!UICONTROL 甘特圖]中啟用的選項，以及工作清單中可用的選項。

   例如，只有在您至少有一個工作與里程碑相關聯時，里程碑才會顯示在圖例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
