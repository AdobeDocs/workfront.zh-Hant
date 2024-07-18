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

# 將[!UICONTROL 甘特圖]匯出至PDF

您可以將[!UICONTROL 甘特圖]匯出至PDF。

將[!UICONTROL 甘特圖]匯出至PDF後，您可以列印或附加至電子郵件，以與其他使用者共用。

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
   <td> <p>[！UICONTROL檢視]或更高的專案和任務存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 匯出[!UICONTROL 甘特圖]

1. 存取您要匯出至PDF的[!UICONTROL 甘特圖]，如[開始使用[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)中所述。
1. 在匯出之前，請確定您已將[!UICONTROL 甘特圖]設定為顯示適當的資訊。

   >[!NOTE]
   >
   >如果您從專案清單匯出[!UICONTROL 甘特圖]，則PDF檔案僅包含清單中的專案，而不包含每個專案上的任務。 如果要匯出任務清單，可以從與其關聯的專案中匯出，也可以建立任務報告並在[!UICONTROL 甘特圖]中顯示報告結果。

   您可以設定下列資訊：

   * 工作清單中所需的篩選器、檢視和群組。 檢視[!UICONTROL 甘特圖]時，會維護清單檢視中選取的任何篩選器和群組。 檢視只會在第一頁的[!UICONTROL 甘特圖]旁顯示的清單中，反映在匯出的[!UICONTROL 甘特圖]上。 檢視不會顯示在[!UICONTROL 甘特圖]本身。

     >[!TIP]
     >
     >若要讓[!UICONTROL 甘特圖]本身有更多空間，請套用包含儘可能少欄的檢視。

   * [!UICONTROL 甘特圖]上的組態選項。 例如，您可以啟用里程碑、日期、[!UICONTROL 基準線]或完成百分比[!UICONTROL 在[!UICONTROL 甘特圖]上顯示。]

     如需詳細資訊，請參閱   [設定資訊在[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的顯示方式。

     >[!NOTE]
     >
     > 將[!UICONTROL 甘特圖]匯出至PDF時，[!UICONTROL 甘特圖]上不會顯示指派。 將[!UICONTROL 甘特圖]匯出至PDF時，指派僅會顯示在清單檢視中。

   * 顯示在[!UICONTROL 甘特圖]上的時段。\

     如需詳細資訊，請參閱[檢視[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的資訊。

     在匯出檔案中顯示時間週期的方式，取決於您選取了&#x200B;**[!UICONTROL 我看到的內容]**&#x200B;或在後續步驟中選取了&#x200B;**[!UICONTROL 多頁]**。

1. （選擇性）若要在匯出的PDF中僅包含某些工作，請選取您要包含的工作。

   如果您未選取任何任務，則所有任務都會包含在匯出的PDF中。

   例如，如果您正在檢視包含50個任務的專案的[!UICONTROL 甘特圖]，但您只想在匯出的[!UICONTROL 甘特圖]上顯示10個任務，請選取您要顯示的10個任務。

1. 按一下印表機圖示。\
   顯示&#x200B;**[!UICONTROL 匯出至PDF]**&#x200B;對話方塊。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 選取您是否要只匯出所見或整個[!UICONTROL 甘特圖]：

   * **[!UICONTROL 我看到的內容]：**&#x200B;匯出在匯出最多500個專案之前顯示在畫面上的所有任務（包括任何子任務）。 （**[!UICONTROL 預覽]**&#x200B;區段中並未顯示這個專案；[!UICONTROL 預覽]區段僅包含範例資料。）

     即使父任務已摺疊且子任務不可見，子任務也會包含在匯出的PDF中。 若只要包含父系任務，請選取要包含的父系任務，並保留任何子任務為未選取。

     您可以使用&#x200B;**[!UICONTROL 縮放為]**&#x200B;下拉式功能表或滑桿工具，只顯示[!UICONTROL 甘特圖]的一部分，如[檢視[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的資訊中所述。

   * **[!UICONTROL 多個頁面]：**&#x200B;匯出整個[!UICONTROL 甘特圖]，即使它在目前熒幕上不可見，最多500個專案。\

     您可以使用&#x200B;**[!UICONTROL 縮放至]**&#x200B;下拉式功能表或滑桿工具來決定每個頁面上顯示的資訊量，如[設定[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上資訊的顯示方式。 選取較精細的選項以顯示更多要匯出的頁面，或選取較精細的選項以顯示較少要匯出的頁面。

     >[!NOTE]
     >
     >如果您需要匯出包含超過500個專案的[!UICONTROL 甘特圖]，請在檢視[!UICONTROL 甘特圖]之前先將篩選器套用至清單，以便顯示少於500個專案或250頁。 如需如何套用篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
     >
     >
     >在下列情況下，無法匯出整個甘特圖：
     >
     >   
     >   
     >   * 跨越250頁時
     >   * 當它包含超過500個專案




1. 如果PDF在匯出為PDF後才會列印，請在&#x200B;**[!UICONTROL 頁面大小]**&#x200B;下拉式功能表中，選取您要列印的紙張大小。\
   您可以選取&#x200B;**[!UICONTROL Letter]**、**[!UICONTROL Legal]**、**[!UICONTROL Ledger]**、**[!UICONTROL A1]**、**[!UICONTROL A2]**、**[!UICONTROL A3]** （僅適用於某些語言）或&#x200B;**[!UICONTROL A4]**。
1. 在&#x200B;**[!UICONTROL 頁面方向]**&#x200B;區段中，選取您要以橫向或縱向匯出PDF。
1. 若要在匯出的PDF中包含圖例，請選取&#x200B;**[!UICONTROL 顯示圖例]**。
1. 按一下&#x200B;**[!UICONTROL 匯出]**。

   [!UICONTROL 甘特圖]的PDF已建立並下載至您的電腦。

   請注意匯出檔案底部的圖例。 它僅說明您在[!UICONTROL 甘特圖]中啟用的選項，以及工作清單中可用的選項。

   例如，只有在您至少有一個工作與里程碑相關聯時，里程碑才會顯示在圖例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
