---
navigation-topic: use-the-gantt-chart
title: 將甘特圖導出為PDF
description: 可以將甘特圖導出到PDF。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# 匯出 [!UICONTROL 甘特圖] PDF

您可以匯出 [!UICONTROL 甘特圖] 到PDF。

匯出 [!UICONTROL 甘特圖] 若要PDF，您可以列印或附加至電子郵件，以便與其他使用者共用。

## 存取需求

您必須具備下列條件，才能遵循本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]許可證*</td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>[!UICONTROL視圖]或更高的項目和任務訪問權限</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>[!UICONTROL視圖]或更高版本對項目的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 匯出 [!UICONTROL 甘特圖]

1. 存取 [!UICONTROL 甘特圖] 要導出到PDF，如 [開始使用 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 請確定您已設定 [!UICONTROL 甘特圖] 以在導出資訊之前顯示相應資訊。

   >[!NOTE]
   >
   >如果您匯出 [!UICONTROL 甘特圖] 從專案清單中，PDF檔案只包含清單中的專案，不包含每個專案的任務。 如果要導出任務清單，可以從任務關聯的項目或建立任務報告並在中顯示報告結果 [!UICONTROL 甘特視圖].

   您可以設定下列資訊：

   * 視需要在任務清單中篩選、檢視和群組。 檢視 [!UICONTROL 甘特圖]. 檢視會反映在匯出的 [!UICONTROL 甘特圖] 僅顯示在 [!UICONTROL 甘特圖] 在第一頁。 檢視不會顯示在 [!UICONTROL 甘特圖] 本身。

      >[!TIP]
      >
      >為 [!UICONTROL 甘特圖] 本身，則套用盡可能少的欄的檢視。

   * 配置選項 [!UICONTROL 甘特圖]. 例如，您可以啟用里程碑、日期、 [!UICONTROL 基線]，或 [!UICONTROL 百分比完成] 顯示於 [!UICONTROL 甘特圖].

      如需詳細資訊，請參閱   [設定資訊在 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > 分配不會顯示在 [!UICONTROL 甘特圖] 當 [!UICONTROL 甘特圖] 會匯出至PDF。 當 [!UICONTROL 甘特圖] 導出到PDF時，分配僅顯示在清單視圖中。

   * 顯示在 [!UICONTROL 甘特圖].\

      如需詳細資訊，請參閱 [檢視 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      匯出檔案中顯示時段的方式取決於您是否選取 **[!UICONTROL 我看到的]** 或 **[!UICONTROL 多個頁面]** 的URL。

1. （可選）要在導出的PDF中僅包括某些任務，請選擇要包括的任務。

   如果未選擇任何任務，則所有任務都將包含在導出的PDF中。

   例如，如果您檢視的 [!UICONTROL 甘特圖] 若專案包含50個工作，但您只想在匯出的項目中顯示10個工作 [!UICONTROL 甘特圖]，選擇要顯示的10個任務。

1. 按一下打印機表徵圖。\
   此 **[!UICONTROL 匯出至PDF]** 對話框。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 選取您只要匯出您看到的內容或整個 [!UICONTROL 甘特圖]:

   * **[!UICONTROL 我看到的]:** 匯出最多500個項目之前，會先匯出畫面上顯示的所有工作（包括任何子工作）。 (這不是顯示在 **[!UICONTROL 預覽]** 部分；the [!UICONTROL 預覽] 區段僅包含範例資料。)

      即使父任務折疊且子任務不可見，子任務仍包含在導出PDF中。 要僅包括父任務，請選擇要包括的父任務，並取消選擇任何子任務。

      您可以使用 **[!UICONTROL 縮放至]** 下拉式選單或滑桿工具，只顯示 [!UICONTROL 甘特圖]，如 [檢視 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 多個頁面]:** 匯出整個 [!UICONTROL 甘特圖]，即使在目前畫面上看不到的項目最多500個項目。\

      您可以使用 **[!UICONTROL 縮放至]** 下拉式選單或滑桿工具，以決定每個頁面上顯示多少資訊，如 [設定資訊在 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 選取更精細的選項以顯示更多要匯出的頁面，或選取較精細的選項以顯示較少要匯出的頁面。

      >[!NOTE]
      >
      >如果您需要匯出 [!UICONTROL 甘特圖] 包含500個以上項目的篩選器，請在檢視 [!UICONTROL 甘特圖] 以便顯示少於500個項目或250頁。 如需如何套用篩選器的相關資訊，請參閱  [篩選器概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >在以下情況下，不能導出整個甘特圖：
      >
      >   
      >   
      >   * 跨越超過250頁時
      >   * 包含超過500個項目時





1. 如果PDF在匯出至PDF後會列印，請在 **[!UICONTROL 頁面大小]** 下拉菜單，選擇要打印的紙張的大小。\
   您可以選取 **[!UICONTROL 信函]**, **[!UICONTROL 法律資訊]**, **[!UICONTROL 分類帳]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** （僅適用於某些語言），或 **[!UICONTROL A4]**.
1. 在 **[!UICONTROL 頁面方向]** 區段，選擇要以橫向還是縱嚮導出PDF。
1. 選擇 **[!UICONTROL 顯示圖例]** 如果要在導出的PDF中包含圖例。
1. 按一下 **[!UICONTROL 匯出]**.

   的 [!UICONTROL 甘特圖] 已建立並下載至您的電腦。

   請注意匯出檔案底部的圖例。 它只說明您已在 [!UICONTROL 甘特圖] 任務清單中可用。

   例如，只有在至少有一個任務與里程碑相關聯時，里程碑才會顯示在圖例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
