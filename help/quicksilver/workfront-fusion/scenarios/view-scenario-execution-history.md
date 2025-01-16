---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中檢視情境歷史記錄
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中檢視情境歷史記錄

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [檢視情境的執行歷程記錄](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-scenario-execution-history.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

您可以顯示情境的事件或執行相關資訊，也可以搜尋情境的所有執行以尋找特定資料。

案例執行代表案例的單一執行。

案例事件是對案例的修改，例如編輯、啟用或停用。

>[!NOTE]
>
>情境歷史記錄會顯示情境過去30天的所有事件和執行。

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
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 檢視案例歷史記錄

### 在[!UICONTROL 案例詳細資料]頁面上檢視案例歷史記錄

1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]**&#x200B;索引標籤，然後按一下案例。

   或

   如果您正在案例編輯器中處理案例，請按一下視窗左上角附近的向左箭頭![](assets/exit-editing-arrow.png)。

1. 在右側面板的&#x200B;**History**&#x200B;索引標籤中檢視執行歷史記錄。

   以下是此情境每次執行的詳細資料：

   * 執行開始於&#x200B;**[!UICONTROL 的日期]**
   * **[!UICONTROL 狀態]** （成功或失敗）
   * 執行&#x200B;**[!UICONTROL 持續時間]**
   * **[!UICONTROL 作業數目]**
   * **[!UICONTROL 資料傳輸]**&#x200B;的大小

   >[!NOTE]
   >
   >案例歷史記錄會在最近執行的案例旁邊顯示&#x200B;**處理**&#x200B;徽章，而執行詳細資訊會寫入儲存體。 處理會在案例執行後立即發生。 和不應超過幾分鐘。 處理執行時，可能無法看到案例執行的詳細資訊。

1. 若要檢視特定案例執行的詳細資訊，請按一下右側面板中的該執行。
1. 若要檢視事件，請按一下右側面板的&#x200B;**事件**&#x200B;標籤。


### 在[!UICONTROL 歷程記錄]標籤上檢視案例歷程記錄

[!UICONTROL 歷程記錄]索引標籤顯示的詳細資訊比[!UICONTROL 案例詳細資料]頁面上提供的還多。 您也可以在[!UICONTROL 歷程記錄]索引標籤上篩選及排序執行。

1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]**&#x200B;索引標籤，然後按一下案例。

   或

   如果您正在案例編輯器中處理案例，請按一下視窗左上角附近的向左箭頭![](assets/exit-editing-arrow.png)。

1. 按一下頁面左上角附近的&#x200B;**[!UICONTROL 歷程記錄]**&#x200B;索引標籤
1. （選擇性）如需所選取案例執行的詳細資訊，包括已處理哪些組合，請按一下該行中的&#x200B;**[!UICONTROL 詳細資料]**&#x200B;按鈕。

   如需有關處理套裝的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[案例執行流程。

   >[!NOTE]
   >
   >* [!UICONTROL 詳細資料]連結只有在執行有可用的詳細資料時才可見。
   >
   >* 案例歷史記錄會在最近執行的案例旁邊顯示&#x200B;**處理歷史記錄**&#x200B;徽章，而執行詳細資訊會寫入儲存體。 處理會在案例執行後立即發生。 和不應超過幾分鐘。 處理執行時，可能無法看到案例執行的詳細資訊。

1. 若要檢視事件，請啟用&#x200B;**顯示事件**&#x200B;切換。

## 篩選案例執行歷史記錄

您可以篩選執行歷史記錄，以僅檢視具有指定值的執行。

1. 開啟情境的全頁記錄，如本文中[!UICONTROL 歷程記錄]索引標籤](#view-scenario-execution-history-on-the-history-tab)上的[檢視情境執行歷程記錄中所述。
1. 按一下要作為篩選依據之欄標題中的[!UICONTROL 篩選器]圖示![](assets/fusion-scenario-filter-icon.png)。
1. 在[!UICONTROL 篩選器]對話方塊中，輸入您要作為篩選依據的值。
1. 按一下「**[!UICONTROL 儲存]**」。

若欄中有目前作用中的篩選器，則篩選器圖示為橘色。

## 排序案例執行歷史記錄

您可以排序案例執行歷史記錄。

1. 開啟情境的全頁記錄，如本文中[!UICONTROL 歷程記錄]索引標籤](#view-scenario-execution-history-on-the-history-tab)上的[檢視情境執行歷程記錄中所述。
1. 按一下要作為篩選依據之欄標題中的[!UICONTROL 排序]圖示。
1. 可選：若要反轉排序順序，請再按一下[!UICONTROL 排序]圖示。

## 搜尋情境的所有執行

1. 開啟情境的全頁記錄，如本文中[!UICONTROL 歷程記錄]索引標籤](#view-scenario-execution-history-on-the-history-tab)上的[檢視情境執行歷程記錄中所述。
1. 按一下執行清單頂端的&#x200B;**[!UICONTROL 全文檢索搜尋]**。

   或

   輸入&#x200B;**Ctrl+Shift+F** (Windows)或&#x200B;**Cmd+Shift+F** (Mac)
會開啟[!UICONTROL 搜尋歷史記錄]視窗。

1. （選擇性）若要搜尋包含特定文字的執行，請在&#x200B;**[!UICONTROL 在歷程記錄]**&#x200B;視窗中搜尋的搜尋列中輸入文字。

   若要搜尋精確文字，請以雙引號（「範例」）括住文字。

   >[!INFO]
   >
   >**範例：**&#x200B;如果您想要尋找建立特定專案的執行，請在[!UICONTROL 全文檢索搜尋]列中輸入專案識別碼。
   >
   >「625ef2ef0006036bd1794b6e52d737c5」

1. （選擇性）若要依日期範圍限制搜尋，請在[!UICONTROL 依日期範圍]區域選取所要搜尋的開始和結束日期。

   >[!NOTE]
   >
   >* 執行只適用於之前的30天。
   >
   >* [!DNL Workfront Fusion]儲存webhook裝載30天。 存取webhook裝載時，若在裝載建立超過30天後進行，會導致&#39;&#39;[!UICONTROL 無法從儲存空間讀取檔案。]&#39;&#39;


1. （選擇性）若要依狀態限制搜尋，請在&#x200B;**[!UICONTROL 依狀態]**&#x200B;下拉式清單中選取所需的狀態。


   可用的狀態包括：

   * [!UICONTROL 全部]

   * [!UICONTROL 錯誤]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （選擇性）變更結果在&#x200B;**[!UICONTROL 依日期排序]**&#x200B;下拉式清單中的顯示順序。

1. （選擇性）若要複製案例執行ID，請按一下&#x200B;**[!UICONTROL 複製執行ID]**&#x200B;圖示 所需執行列中的<img src="assets/copy-fusion-execution-id-icon.png">

1. （選擇性）按一下[!UICONTROL 全文檢索搜尋]的結果，以檢查包含資訊的案例模組輸出組合。
