---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 匯出資料
description: 匯出資料的部分原因為 — EDIT ME。
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '2182'
ht-degree: 0%

---

# 匯出資料

您可以從各種清單、報表、控制面板和搜尋匯出Adobe Workfront資料。
本條中的資訊不適用於下列出口：

* 從圖表報表匯出資訊。

   如需匯出圖表報表的詳細資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 從甘特圖導出資訊。

   有關導出甘特圖的詳細資訊，請參見 [將甘特圖導出為PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* 從資源計畫器導出資訊。

   有關從資源計畫器導出資訊的詳細資訊，請參閱 [資源計畫員導航概覽](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

匯出資料的部分原因如下：

* 您想要將資料的硬式副本提供給Workfront以外的人。
* 您想要將報表結果作為附件傳送給外部使用者。
* 您想要建立Workfront資料的外部備份。
* Workfront Web應用程式內的一個頁面上限制只顯示2,000個結果。 如果您的報表產生的數量超過2,000個，您可以將報表匯出為下列任何格式，並在一個清單中檢視報表中的所有結果。

您可以手動從Workfront介面匯出報表，或排程報表的傳送，該報表稍後會傳送給您。 如需排程傳送報表的詳細資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高存取報表、控制面板、日曆以匯出報表</p> <p>查看或更高訪問清單中查看的對象以導出清單</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視報表或控制面板的或更高權限，以匯出報表或控制面板</p> <p>查看清單中您查看的對象的或更高權限以導出清單</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

必須先建立報表，才能匯出其資料。

如需建立報表的詳細資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 匯出格式和限制

* [匯出格式](#export-formats)
* [匯出限制](#export-limits)

### 匯出格式 {#export-formats}

資訊可以以下列格式匯出：

* PDF（信函橫向或直向、法律、分類帳和A4）
* Excel(.xls)
* Excel(.xlsx)
* 頁籤分隔檔

>[!NOTE]
>
>控制面板只能打印或導出為.pdf檔案。

### 匯出限制 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Workfront中報表的顯示方式，以及透過手動匯出、傳送報表或API匯出的方式，都有幾項限制。

* **50,000列：** 匯出.pdf和Tab分隔檔案的報表中允許的資料列數。

   * 對於Excel .xls檔案，此限制為 **65,000列**.
   * 若為Excel .xlsx檔案，此限制為 **100,000列**.
   * 這些限制會排除欄標題，以及報表中分組的列。 例如，若報表中有6個群組，以及50,000列或資料，則匯出的檔案將會有50,000列。

   >[!IMPORTANT]
   >
   >匯出報表（在欄中包含集合參考）可能會導致錯誤，即使報表不在所列的匯出限制內亦然。 如果引用的集合太大，則導出進程會超時，並隨後導致錯誤。
   >
   >要避免此錯誤，請排除引用大型集合的列，或在導出之前縮小引用的集合的大小。

   如果報表的項目數超過這些限制，您會收到匯出未成功的錯誤。 將您在畫面上看到的項目數減少為小於或等於這些限制，以便匯出結果。

   如果您的報表超過50,000/65,000/100,000列，且您想要匯出所有資料，建議您使用篩選器或提示來取得較少的資料載入，並執行多次匯出。

   如需使用篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   有關使用提示的資訊，請參見 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* 這些限制適用於：

   * 手動匯出報表。
   * 排程報表。
   * 透過API整合匯出。
   * 透過啟動匯出的資料。

      如需透過啟動匯出資料的詳細資訊，請參閱 [透過Kick-Starts從Adobe Workfront匯出資料](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

      >[!NOTE]
      >
      >雖然您只能將資料匯出為Excel格式檔案，但您仍可匯出啟動檔案中的50,000列。 

   * 導出項目的利用率資訊。

      有關導出項目的利用率資訊的詳細資訊，請參見 [資源利用率報告概覽](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB檔案大小：** 已排程傳送之任何匯出報表的檔案大小限制。 如果附加至電子郵件的匯出檔案大於5MB，則會以電子郵件傳送可下載檔案的連結，而非附加的匯出報表。
* **65,530個超連結：** 這是Excel對包含65,530個以上超連結的檔案所施加的限制。 手動匯出或在傳送的報表中傳送這些檔案時，無法開啟這些檔案。 請注意， Excel文檔可能只有200行資料，但如果文檔內有65,530個以上的連結，則該文檔不會開啟。 此限制僅存在於Excel檔案中，不存在於其他支援的格式中。 
* **256欄**:這是Excel對包含256欄以上的檔案所施加的限制。 無法手動匯出這些檔案，或在傳送的報表中傳送。 此限制僅存在於Excel檔案中，不存在於其他支援的格式中。

如果您嘗試匯出超過限制的資料，可能不會在匯出中收到所有預期的資料。 而是在限制內產生修改的報表。

此外，執行超過60分鐘的報表將會暫停。

若您對限制有疑慮或有問題，請聯絡Workfront技術支援。

## 匯出資料

* [從報表或清單匯出資料](#export-data-from-a-report-or-list)
* [從控制面板匯出資料](#export-data-from-a-dashboard)

### 從報表或清單匯出資料 {#export-data-from-a-report-or-list}

1. 前往要匯出的報表或清單。
1. 選取要匯出的項目。 （選取個別項目只會匯出您選取的項目。）

   例如，在專案中，選取您要匯出的任務。

   或

   保留取消選取所有項目以匯出整個清單。

1. 按一下 **匯出**，然後選取格式。

   >[!NOTE]
   若要匯出控制面板報表，您必須具備計畫授權。\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   或

   按一下 **匯出** 圖示 ![](assets/export-icon-nwe.png)，然後選取格式。

   用於PDF導出的選項取決於Workfront用戶設定中的區域設定：

   * 北美 — 信函（預設）、法律、分類帳、A4

      <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * 北美以外的所有地點 — A3、A4（預設）、信函、法律、分類帳

      <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. （條件性）視您使用的作業系統而定，您可能可以選擇開啟或儲存檔案。 開啟包含關聯應用程式的檔案或將其保存到硬碟。
1. 繼續 [使用導出的文檔](#use-the-exported-document).

### 從控制面板匯出資料 {#export-data-from-a-dashboard}

您可以從控制面板列印資訊，或將其匯出為.pdf檔案。

如需從控制面板匯出資料的詳細資訊，請參閱 [匯出控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## 使用導出的文檔 {#use-the-exported-document}

* [檔案名](#file-names)
* [標題](#titles)
* [時間戳記](#timestamps)
* [格式](#formatting)
* [連結](#links)
* [品牌化](#branding)

### 檔案名 {#file-names}

無論是導出對象清單還是導出報告，導出的檔案都會有檔案名和標題。 您可以參照檔案名稱，在電腦上找到匯出的檔案。 報表標題可讓使用者在與他們共用時，了解匯出的檔案代表什麼。

* [導出清單的檔案名](#file-names-for-exported-lists)
* [匯出報表的檔案名](#file-names-for-exported-reports)

#### 導出清單的檔案名 {#file-names-for-exported-lists}

導出對象清單時，對象類型將顯示在導出檔案的檔案名和清單的標題中。

匯出任務或問題清單時， **檔案名** 可以是下列其中一項：

* 導出項目中的任務和問題清單時：

   * *The_project_name_Exported_Tasks*(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*
   * *The_project_name_Exported_Issues*(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*

* 導出任務（子任務）中的任務和問題清單時：

   * **The_project_name_the_task_name_Exported_Tasks**(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*
   * **The_project_name_the_task_name_Exported_Issues**(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*

將項目中的任何其他對象的清單導出到PDF檔案時，導出文檔的檔案名將指示導出的對象的類型。\
例如，檔案名稱可能是：

* *Exported_Users*，在專案上匯出「人物」標籤時(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*
* *Exported_Risks*，在導出項目風險清單時(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*

#### 匯出報表的檔案名 {#file-names-for-exported-reports}

匯出報表時，匯出報表的檔案名為：

*The_report_name*(*以PDF、Excel、Excel(.xlsx)或Tab分隔格式)*

### 標題 {#titles}

導出對象清單時，只有PDF格式的檔案具有標題。 如果您將清單或報表匯出為Excel、Excel(.xlsx)或Tab分隔格式，則檔案沒有標題。

* [導出清單的標題](#titles-for-exported-lists)
* [匯出報表的標題](#titles-for-exported-reports)

#### 導出清單的標題 {#titles-for-exported-lists}

將項目中的任務和問題清單導出到PDF檔案時，導出文檔的標題如下：

* *項目名稱 — 導出的任務*
* *專案名稱 — 匯出的問題*

將任務中的任務和問題清單導出到PDF檔案時，導出文檔的表徵圖如下：

* *項目名稱 — 任務名稱 — 導出的任務*
* *專案名稱 — 任務名稱 — 匯出的問題*

將項目中的任何其他對象清單導出到PDF檔案時，導出文檔的標題指示導出的對象的類型。\
例如，標題可能是：

* *匯出的使用者*，在匯出專案的「人物」標籤時。
* *出口風險*，在導出項目風險清單時。

#### 匯出報表的標題 {#titles-for-exported-reports}

匯出至PDF檔案的報表會有標題。

如果報表匯出為Excel、Excel(.xlsx)或Tab分隔格式，則匯出的報表將沒有標題。 匯出檔案的標題是報表的名稱，如Workfront Web應用程式中所示。

如果報表有說明，則會包含在匯出的檔案中。

### 時間戳記 {#timestamps}

從導出項目的用戶的上下文導出的文檔上顯示時間戳。

時間戳記包括：

* 日期
* 時間
* 項目導出時的時區

根據導出的文檔類型，時間戳會顯示在不同的位置：

* **PDF:** 時間戳記會顯示在每個頁面的頁尾和檔案名稱中。
* **Excel:** 時間戳記會顯示在檔案名稱中。

### 格式 {#formatting}

將專案匯出為.pdf時，任何子任務都會以縮排顯示為其父任務。 導出的清單不會折疊任何父任務。

在傳送或排程傳送報表時，除非報表有特殊檢視，否則一律會收到報表的預設索引標籤。

如果您的報表在Web應用程式中有特殊格式，當「詳細資訊」和「矩陣」索引標籤僅針對.pdf和Excel檔案傳送時，應以特殊格式傳送報表。

>[!NOTE]
如果您要匯出的資料包含共用欄，而您匯出為Excel或Tab分隔格式，則這些欄會在匯出的檔案中分開。

如需如何自訂報表中格式的詳細資訊，請參閱 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### 連結 {#links}

連結可以指向Workfront中支援連結的任何物件。 將Workfront中的清單導出為.pdf時，原始文檔中存在的任何受支援連結在導出的文檔中都保持為即時狀態。

>[!TIP]
如果行 `valueformat=HTML` 以文本模式顯示自定義欄位列，而連結值不顯示在導出的.pdf檔案中，您需要以文本模式在列中輸入其他代碼行。
例如，如果您有一個名為「開啟第1季專案」的自訂欄位包含連結，則會新增下列程式碼：

```
link.url=customDataLabelsAsString(Open Q1 Projects)
linkedname=direct
```

匯出為Excel格式時，匯出的檔案中只會包含Workfront中物件的連結，且只有可選取允許匯出Excel檔案中的連結（例如報表傳送）的位置才支援這些連結。

## 品牌化 {#branding}

如果您的Workfront管理員已在全域導覽列的Workfront執行個體中新增自訂品牌，則匯出的.pdf檔案也會包含您的個人化標誌。

以任何其他格式匯出的資料無法以您的標誌個人化。

如需將Workfront例項與全域導覽列品牌化的詳細資訊，請參閱 [品牌化您的Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
