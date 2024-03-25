---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中檢視案例的執行歷史記錄
description: 您可以顯示某個案例所有執行的相關資訊，也可以搜尋特定資料之案例的所有執行。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: ae57c38149bf6db3bbbb471fad8f3567b7d712a7
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# 在中檢視案例的執行歷史記錄 [!DNL Adobe Workfront Fusion]

您可以顯示某個案例所有執行的相關資訊，也可以搜尋特定資料之案例的所有執行。

案例的執行歷史記錄會顯示案例在過去30天中的所有執行。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 檢視案例的所有執行

### 在上檢視案例執行歷史記錄 [!UICONTROL 案例詳細資訊] 頁面

1. 按一下 **[!UICONTROL 情境]** 標籤，然後按一下情境。

   或

   如果您在案例編輯器中處理案例，請按一下向左箭頭 ![](assets/exit-editing-arrow.png) 靠近視窗左上角。

1. 檢視右側清單中的資訊。

   ![](assets/open-history-tab-350x202.png)

   您也可以按一下，檢視此資訊的完整頁面檢視。 全頁檢視可讓您篩選歷史記錄，以檢視特定執行。

   以下是此情境每次執行的詳細資料：

   * 執行日期 **[!UICONTROL 已開始]**
   * **[!UICONTROL 狀態]** （成功或失敗）
   * 執行 **[!UICONTROL 持續時間]**
   * 數量 **[!UICONTROL 作業]**
   * 大小 **[!UICONTROL 資料傳輸]**
   * 連結至 **[!UICONTROL 詳細資料]**

>[!NOTE]
>
>案例歷史記錄會顯示 **處理中** 徽章位於最近執行的案例旁，而執行詳細資訊會寫入儲存空間。 處理會在案例執行後立即發生。 和不應超過幾分鐘。 處理執行時，可能無法看到案例執行的詳細資訊。

### 在上檢視案例執行歷史記錄 [!UICONTROL 歷史記錄] 標籤

此 [!UICONTROL 歷史記錄] 標籤顯示的詳細資料多於 [!UICONTROL 案例詳細資料] 頁面。 您還可以對上的執行進行篩選和排序 [!UICONTROL 歷史記錄] 標籤。

1. 按一下 **[!UICONTROL 情境]** 標籤，然後按一下情境。

   或

   如果您在案例編輯器中處理案例，請按一下向左箭頭 ![](assets/exit-editing-arrow.png) 靠近視窗左上角。

1. 按一下 **[!UICONTROL 歷史記錄]** 索引標籤在頁面左上角附近
1. （選用）如需有關所選案例執行的詳細資訊（包括已處理哪些組合），請按一下 **[!UICONTROL 詳細資料]** 連結。

   如需處理套裝的詳細資訊，請參閱 [中的案例執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* 此 [!UICONTROL 詳細資料] 只有在執行有可用的詳細資料時，才會顯示連結。
   >
   >* 案例歷史記錄會顯示 **處理歷史記錄** 徽章位於最近執行的案例旁，而執行詳細資訊會寫入儲存空間。 處理會在案例執行後立即發生。 和不應超過幾分鐘。 處理執行時，可能無法看到案例執行的詳細資訊。

## 篩選案例執行歷史記錄

您可以篩選執行歷史記錄，以僅檢視具有指定值的執行。

1. 開啟情境的全頁記錄，如所述 [在上檢視案例執行歷史記錄 [!UICONTROL 歷史記錄] 標籤](#view-scenario-execution-history-on-the-history-tab) 本文章內容。
1. 按一下 [!UICONTROL 篩選] 圖示 ![](assets/fusion-scenario-filter-icon.png) 欄標題中作為篩選依據的。
1. 在 [!UICONTROL 篩選] 對話方塊中，輸入您要用來篩選的值。
1. 按一下「**[!UICONTROL 儲存]**」。

若欄中有目前作用中的篩選器，則篩選器圖示為橘色。

## 排序案例執行歷史記錄

您可以排序案例執行歷史記錄。

1. 開啟情境的全頁記錄，如所述 [在上檢視案例執行歷史記錄 [!UICONTROL 歷史記錄] 標籤](#view-scenario-execution-history-on-the-history-tab) 本文章內容。
1. 按一下 [!UICONTROL 排序] 圖示來篩選依據。
1. 可選：若要反轉排序順序，請按一下 [!UICONTROL 排序] 圖示再次顯示。

## 搜尋情境的所有執行

1. 按一下 **[!UICONTROL 情境]** 圖示 ![](assets/scenarios-icon.png) 在左側面板中，然後按一下情境。

   或

   如果您在案例編輯器中處理案例，請按一下向左箭頭 ![](assets/exit-editing-arrow.png) 靠近視窗左上角。

1. 按一下 **[!UICONTROL 歷史記錄]** 在熒幕左上角附近按tab鍵。
1. 按一下 **[!UICONTROL 全文搜尋]** 在執行清單頂端。

   或

   型別 **Ctrl+Shift+F** (Windows)或 **Cmd+Shift+F** (Mac) [!UICONTROL 在記錄中搜尋] 視窗會開啟。

1. （可選）若要搜尋包含特定文字的執行，請在的搜尋列中輸入文字 **[!UICONTROL 在記錄中搜尋]** 視窗。

   若要搜尋精確文字，請以雙引號（「範例」）括住文字。

   >[!INFO]
   >
   >**範例：** 如果您想尋找建立特定專案的執行，請在中輸入專案ID [!UICONTROL 全文搜尋] 長條圖。
   >
   >「625ef2ef0006036bd1794b6e52d737c5」

1. （選擇性）若要依日期範圍限制搜尋，請在「 」中選取所要搜尋的開始和結束日期 [!UICONTROL 依日期範圍] 區域。

   >[!NOTE]
   >
   >* 執行只適用於之前的30天。
   >
   >* [!DNL Workfront Fusion] 會儲存webhook裝載30天。 在建立webhook裝載超過30天後存取該裝載會導致錯誤»[!UICONTROL 無法從儲存體讀取檔案。]&quot;


1. （選擇性）若要依狀態限制搜尋，請在 **[!UICONTROL 依狀態]** 下拉式清單。


   可用的狀態包括：

   * [!UICONTROL 全部]

   * [!UICONTROL 錯誤]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （選擇性）變更結果在 **[!UICONTROL 依日期排序]** 下拉式清單。

1. （選用）若要複製案例執行ID，請按一下 **[!UICONTROL 複製執行ID]** 圖示 <img src="assets/copy-fusion-execution-id-icon.png"> 在所需執行的列中

1. （選用）按一下 [!UICONTROL 全文搜尋] 檢查包含資訊的案例模組輸出組合。
