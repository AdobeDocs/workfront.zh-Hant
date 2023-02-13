---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中檢視案例的執行歷史記錄
description: 您可以顯示藍本所有執行的相關資訊，或搜尋藍本的所有執行以取得特定資料。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# 在 [!DNL Adobe Workfront Fusion]

您可以顯示藍本所有執行的相關資訊，或搜尋藍本的所有執行以取得特定資料。

藍本的執行歷史記錄會顯示過去30天內藍本的所有執行。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 查看方案的所有執行

### 在 [!UICONTROL 藍本詳細資料] 頁面

1. 按一下 **[!UICONTROL 藍本]** 標籤，然後按一下藍本。

   或

   如果您正在藍本編輯器中處理藍本，請按一下左箭頭 ![](assets/exit-editing-arrow.png) 靠近窗口的左上角。

1. 檢視右側清單中的資訊。

   ![](assets/open-history-tab-350x202.png)

   C

   您也可以按一下，以檢視此資訊的完整頁面檢視。 全頁檢視可讓您篩選歷史記錄以檢視特定執行。

   會針對每次執行案例列出下列詳細資料：

   * 執行的日期 **[!UICONTROL 已開始]**
   * **[!UICONTROL 狀態]** （成功或失敗）
   * 執行 **[!UICONTROL 持續時間]**
   * 數量 **[!UICONTROL 操作]**
   * 大小 **[!UICONTROL 資料傳輸]**
   * 連結至 **[!UICONTROL 詳細資料]**

### 在 [!UICONTROL 歷史記錄] 標籤

此 [!UICONTROL 歷史記錄] 索引標籤會顯示比上可用更多的詳細資料 [!UICONTROL 藍本詳細資料] 頁面。 您也可以篩選及排序 [!UICONTROL 歷史記錄] 標籤。

1. 按一下 **[!UICONTROL 藍本]** 標籤，然後按一下藍本。

   或

   如果您正在藍本編輯器中處理藍本，請按一下左箭頭 ![](assets/exit-editing-arrow.png) 靠近窗口的左上角。

1. 按一下 **[!UICONTROL 歷史記錄]** 標籤
1. （可選）如需所選藍本執行的詳細資訊，包括已處理的套件組合，請按一下 **[!UICONTROL 詳細資料]** 連結。

   如需處理套件組合的詳細資訊，請參閱 [中的方案執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >此 [!UICONTROL 詳細資訊] 只有在執行有可用的詳細資訊時，連結才會顯示。

## 篩選情境執行歷史記錄

您可以篩選執行歷史記錄，以僅檢視具有指定值的執行。

1. 開啟案例的整頁歷史記錄，如 [在 [!UICONTROL 歷史記錄] 標籤](#view-scenario-execution-history-on-the-history-tab) 這篇文章。
1. 按一下 [!UICONTROL 篩選] 圖示 ![](assets/fusion-scenario-filter-icon.png) 在要篩選依據的欄標題中。
1. 在 [!UICONTROL 篩選] 對話框，輸入要篩選的值。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

篩選器圖示在目前作用中篩選器的欄中為橘色。

## 排序方案執行歷史記錄

您可以排序方案執行歷史記錄。

1. 開啟案例的整頁歷史記錄，如 [在 [!UICONTROL 歷史記錄] 標籤](#view-scenario-execution-history-on-the-history-tab) 這篇文章。
1. 按一下 [!UICONTROL 排序] 表徵圖。
1. 可選：若要反轉排序順序，請按一下 [!UICONTROL 排序] 圖示。

## 搜索方案的所有執行

1. 按一下 **[!UICONTROL 藍本]** 圖示 ![](assets/scenarios-icon.png) 在左側面板中，按一下案例。

   或

   如果您正在藍本編輯器中處理藍本，請按一下左箭頭 ![](assets/exit-editing-arrow.png) 靠近窗口的左上角。

1. 按一下 **[!UICONTROL 歷史記錄]** 標籤。
1. 按一下 **[!UICONTROL 全文搜索]** 執行清單的頂端。

   或

   類型 **Ctrl+Shift+F** (Windows)或 **Cmd+Shift+F** (Mac) [!UICONTROL 在歷史記錄中搜索] 窗口。

1. （可選）要搜索包含特定文本的執行，請在 **[!UICONTROL 在歷史記錄中搜索]** 窗口。

   若要搜尋確切的文字，請以雙引號(&quot;example&quot;)括住文字。

   >[!INFO]
   >
   >**範例：** 如果您想要尋找建立特定專案的執行，請在 [!UICONTROL 全文搜索] 欄。
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. （可選）若要依日期範圍限制搜尋，請在 [!UICONTROL 依日期範圍] 的上界。

   >[!NOTE]
   >
   >* 執行只適用於前30天。
   >
   >* [!DNL Workfront Fusion] 儲存webhook負載30天。 在建立Webhook裝載後30天以上存取該裝載會導致錯誤「[!UICONTROL 無法從儲存讀取檔案。]&quot;



1. （可選）若要依狀態限制搜尋，請在 **[!UICONTROL 依狀態]** 下拉式清單。


   可用狀態包括：

   * [!UICONTROL 全部]

   * [!UICONTROL 錯誤]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （選用）變更結果在 **[!UICONTROL 依日期排序]** 下拉式清單。

1. （選用）若要複製案例執行ID，請按一下 **[!UICONTROL 複製執行ID]** 圖示 <img src="assets/copy-fusion-execution-id-icon.png"> 在所需執行的列中

1. （選用）按一下 [!UICONTROL 全文搜索] 檢查包含資訊的方案模組輸出包。
