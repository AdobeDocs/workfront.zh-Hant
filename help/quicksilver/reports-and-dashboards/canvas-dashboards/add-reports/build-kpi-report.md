---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布控制面板中建立KPI報告
description: 主要顯示單一彙總KPI的KPI報告可新增至畫布控制面板。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d76ad0d51f28191cbd04af950e10a2247414830e
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 0%

---

# 在畫布控制面板中建立KPI報告

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

您可以建立KPI報表，並將其新增至畫布控制面板，以視覺化方式將關鍵績效指標資料呈現為數字，讓您用於檢視專案和團隊的成效。

![KPI報告範例](assets/kpi-example-main.png)

## 存取需求

+++ 展開以檢視存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>目前：計畫 </p> 
<p>新增：標準</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr>  
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先建立儀表板，才能建立KPI報表。

## 在畫布控制面板中建立KPI報告

建置KPI報表有許多可用的設定選項。 在本節中，我們將引導您進行建立資料庫的一般程式。

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 按一下右上角的&#x200B;**新儀表板**。

1. 在&#x200B;**建立儀表板**&#x200B;方塊中，輸入儀表板的&#x200B;**名稱**&#x200B;和&#x200B;**描述**。

1. 按一下「**建立**」。

1. 在&#x200B;**新增報告**&#x200B;方塊中，選取&#x200B;**建立報告**。

1. 在左側，選取&#x200B;**KPI**。

1. 按一下右上角的&#x200B;**建立報告**。

1. 請依照下列步驟設定&#x200B;**詳細資料**&#x200B;區段：

   1. 輸入報告&#x200B;**名稱**。
   1. 輸入報告&#x200B;**描述**。

      >[!NOTE]
      >
      >此說明將用作KPI值下方的標題。 如果您未輸入說明，系統會根據您在下列步驟中選取的彙總及彙總型別，為您產生標題。

1. 請依照下列步驟設定&#x200B;**建置KPI**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**建置KPI** ![建置KPI圖示](assets/build-kpi-icon.png)圖示。

   1. 按一下&#x200B;**選取欄位**，然後指定您要新增至報告的欄位。

   1. 在&#x200B;**彙總型別**&#x200B;下拉式清單中，選取資料如何彙總以產生KPI輸出。 此欄位中的選項會依上個步驟中選取的欄位型別而有所不同。

1. 請依照下列步驟設定&#x200B;**篩選器**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**篩選器** ![篩選器圖示](assets/filter-icon.png)圖示。

   1. 選取&#x200B;**編輯篩選器**。

   1. 按一下&#x200B;**新增條件**，然後指定您要篩選的欄位，以及定義欄位必須符合何種條件的修飾元。

   1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

      如需篩選的詳細資訊，請參閱[在畫布儀表板中編輯報告篩選](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md)。

1. 請依照下列步驟設定&#x200B;**向下鑽研資料行設定**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**向下鑽研欄** ![向下鑽研欄圖示](assets/drilldown-column.png)圖示。 圖表中的欄位會自動顯示為右側預覽區段中的欄。

   1. （選擇性）若要更新任何現有的欄設定，請在&#x200B;**目前的欄**&#x200B;區段中選取要更新的欄，然後更新所需的資訊（例如標籤、連結狀態和格式規則）。

   1. 按一下&#x200B;**新增欄**，然後選取您要在表格中顯示為欄的欄位。 對要新增的每個欄重複此程式。

1. 請依照下列步驟設定&#x200B;**向下鑽研群組設定**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**群組設定** ![向下鑽研群組圖示](assets/drilldown-group-icon.png)圖示。

   1. 按一下「**新增群組**」按鈕，然後選取要建立為群組的欄位。

1. 按一下&#x200B;**儲存**&#x200B;以建立報告並將其新增到儀表板。

## 建立KPI報告範例

在本節中，我們將逐步說明建立可顯示待處理檔案核准的KPI報告。

如需KPI報告範例的詳細資訊，請參閱[建立報告儀表板以供檢閱和核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 按一下右上角的&#x200B;**新儀表板**。

1. 在&#x200B;**建立儀表板**&#x200B;方塊中，輸入儀表板的&#x200B;**名稱**&#x200B;和&#x200B;**描述**。

1. 按一下「**建立**」。

1. 在&#x200B;**新增報告**&#x200B;方塊中，選取&#x200B;**建立報告**。

1. 在左側，選取&#x200B;**KPI**。

1. 按一下右上角的&#x200B;**建立報告**。

1. 請依照下列步驟設定&#x200B;**詳細資料**&#x200B;區段：

   1. 在&#x200B;*名稱*&#x200B;欄位中輸入&#x200B;**擱置中**。
   1. 在&#x200B;*描述*&#x200B;欄位中輸入&#x200B;**擱置核准**。 這會在KPI值下方顯示為標題。

1. 請依照下列步驟設定&#x200B;**建置KPI**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**建置KPI** ![建置KPI圖示](assets/build-kpi-icon.png)。

   1. 按一下&#x200B;**選取欄位**。

   1. 尋找並選取&#x200B;**檔案核准**&#x200B;資料夾。

   1. 選取&#x200B;**狀態**。

   1. 在&#x200B;**彙總型別**&#x200B;下拉式清單中，選取&#x200B;**計數**。

1. 請依照下列步驟設定&#x200B;**篩選器**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**篩選器** ![篩選器圖示](assets/filter-icon.png)圖示。

   1. 選取&#x200B;**編輯篩選器**。

   1. 按一下&#x200B;**新增條件**。

   1. 按一下空白條件篩選，按一下&#x200B;**挑選欄位**，然後選擇&#x200B;**狀態**。
   1. 將運運算元保留為&#x200B;**Equal**，然後在文字方塊中輸入&#x200B;_擱置檢閱_。
      ![擱置的KPI篩選範例](assets/pending-kpi-filter.png)
1. 按一下熒幕右上角的&#x200B;**儲存**。

## 建立KPI報表時的考量事項

### 利用欄位選擇器

**建置KPI**&#x200B;區段中的&#x200B;**區段**&#x200B;下拉式清單設計用來縮小欄位選取器中的選擇範圍，以便在建置表格報告時更容易找到物件。 若要開始，您可以選取基礎實體物件。

* **所有區段**： Workfront Workflow和Workfront Planning中的所有物件型別。
* **Workfront物件**：原生Workfront工作流程物件。
* **Planning記錄型別**： Workfront Planning中定義的自訂記錄型別。

![區段下拉式清單](assets/sections-dropdown.png)

選取基底實體物件後，**區段**&#x200B;下拉式清單會以適用的欄位型別選項更新，以便從中進行選擇。

* **所有區段**：原生欄位、自訂欄位和相關物件。
* **所有欄位**：原生和自訂欄位（排除關係）。
* **自訂欄位**：自訂表單或Planning記錄上的客戶定義欄位。
* **Workfront欄位**：僅限原生欄位。
* **關係**：連線的記錄。

![可報告物件選擇](assets/reportable-objects-selection.png)

### 參照子物件

其他欄、篩選選項和群組屬性的可用關係通常僅限於Workfront物件階層中較高的物件，或在報表的基本實體物件上具有單一選取範圍。 但有一些例外，包括：

* 專案>任務
* 檔案核准>檔案核准階段
* 檔案核准階段>檔案核准階段參與者

使用上面列出的任何父項至子項關係時，您會在表格中看到連線到父物件的每個子記錄的一列。


