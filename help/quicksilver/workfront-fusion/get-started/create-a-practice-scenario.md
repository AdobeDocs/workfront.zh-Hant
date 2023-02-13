---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在Adobe Workfront Fusion中建立實務整合案例
description: 本文說明如何使用Adobe Workfront Fusion建立整合案例。 整合情境會將不同的應用程式連結在一起，讓您的資料能夠透過不同的應用程式流動。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中建立實務整合案例

本文說明如何使用Adobe Workfront Fusion建立整合案例。 整合情境會將不同的應用程式連結在一起，讓您的資料能夠透過不同的應用程式流動。

若要建立整合案例，您的組織必須具備 [!DNL Workfront Fusion for Work Automation and Integration] 授權。

如需建置僅限Workfront的自動化案例的指示，請參閱 [在Adobe Workfront Fusion中建立實務自動化案例](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

如需Workfront Fusion授權的詳細資訊，請參閱 [Adobe Workfront Fusion授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>您的組織可能不允許存取Google工作表。 若是如此，您將無法設定此整合，但此處提供的資訊可作為整合案例如何運作的一般範例。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 建立實務案例

角色 [!DNL Adobe Workfront Fusion] 是讓流程自動化，以便您能夠專注於新任務，而不是反複重複相同的任務。 其運作方式是連結應用程式與服務內及之間的動作，以建立可自動傳輸和轉換資料的案例。 您建立的案例會監視應用程式或服務中的資料，並處理該資料以提供您想要的結果。

案例由一系列模組組成，這些模組指出應如何在應用程式內轉換資料，或在應用程式與網站服務之間傳輸資料。

說明如何建立藍本，並在學習使用時強化最佳實務 [!DNL Workfront Fusion]，本文會逐步帶您完成程式。 我們將建立在 [!DNL Workfront] 每一行 [!DNL Google Sheets] 試算表。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>如果您有試算表，其中列出需要在中使用專案時處理的專案，就會有類似的情況 [!DNL Workfront]. 情境可以「監看」試算表中是否有新列，並在中新增專案 [!DNL Workfront] 每個。

建立案例包含數個主要工作：

## 選擇應用程式並為案例命名

1. 下載此 [試算表](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)，然後上傳至 [!DNL Google Drive] 供本練習使用。

   或

   建立或尋找您自己的簡單 [!DNL Google Sheets] 與此類似的試算表：

   ![](assets/spreadsheet-headers-350x55.png)

1. 登入 [!DNL Workfront Fusion] 帳戶。
1. 按一下 **[!UICONTROL 藍本]** ![](assets/scenarios-icon.png) 中。

   在顯示的左側面板中，您可以將藍本組織到資料夾中。

   在右側的主區域頂端，您可以檢視 **[!UICONTROL 全部]** 您建立的方案， **[!UICONTROL 活動方案]** 和 **[!UICONTROL 非活動方案]**，和 **[!UICONTROL 概念]**，這些是之前需要一些工作的情況 [!DNL Workfront Fusion] 可將其分類為使用中或非使用中。

   ![](assets/scenarios-left-panel-350x215.png)

1. 在左側面板中，按一下 **[!UICONTROL 新增資料夾]** 圖示 ![](assets/add-folder-icon.png)，然後為第一個資料夾輸入「實務案例」之類的名稱。

1. 開啟資料夾，然後按一下 **[!UICONTROL 建立新藍本]** 在頁面的右上角。

   顯示的登錄頁面可讓您預先載入您要建立的案例中要使用的任何應用程式。

1. 對於本練習，請搜尋並選取 **[!UICONTROL Google工作表]** 應用程式。
1. 按一下 **[!UICONTROL 繼續]** 在右上角。

   隨即顯示情境編輯器，其中包含中央的空模組， [!DNL Google Sheets] 應用程式預先載入，以及工具列底部的某些選項。

   ![](assets/scenario-editor-350x235.png)

   當您開始建立新案例時，最好先為其建立名稱。

1. 選取 **[!UICONTROL 新藍本]** 左上角的預留位置名稱，然後輸入名稱，例如「實務案例1」。
1. 繼續 [新增及設定第一個模組](#add-and-configure-the-first-module) 下方。

## 新增及設定第一個模組

帶有問號的空白模組代表您需要新增的觸發程式模組。 此模組每次執行時都會啟動案例。 空模組上的時鐘圖示表示是已排程的模組。

![](assets/empty-module.png)

此模組將包含您希望藍本監視的資料。

1. 按一下空白模組，以選擇您要從中選取模組的應用程式。

   您先前預先載入的應用程式會顯示在空白模組旁。 您可以使用 [!UICONTROL 搜尋] 框。

   ![](assets/pre-loaded-apps-350x139.png)

1. 按一下 **[!DNL Google Sheets]**.

   清單會變更為全部顯示 [!DNL Google Sheets] 可作為觸發模組的模組。

1. 按一下觸發程式模組 **[!UICONTROL 關注記錄]**.

   現在，您需要建立已驗證的Google帳戶連線。 您新增至案例的每個模組都必須有與其應用程式的連線。

1. 在 **[!DNL Google Sheets]** 框下 **[!UICONTROL 連線]**，按一下 **[!UICONTROL 新增]**，然後輸入連線的名稱，例如「Olivia的Google帳戶」，然後按一下 **[!UICONTROL 繼續]**.
1. 在顯示的視窗中驗證連線。

   驗證連線的程式可能會在應用程式之間有所不同。 您可能需要登入應用程式。 您通常需要按一下 **[!UICONTROL 允許]** 按鈕。 如果您需要幫助，請參閱 [關於連接 [!DNL Adobe Workfront Fusion] 至應用程式或服務](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 設定第一個模組

連接後 [!DNL Workfront Fusion] 至 [!DNL Google Sheets] 帳戶，您可以指定 [!DNL Google Sheets] 您可存取的試算表，以及您要第一個模組處理的資料。

1. 按一下 **[!UICONTROL 試算表]** 框，然後選擇 **[!UICONTROL Workfront融合實踐場景] #1** 顯示清單中的試算表。

   此試算表包含2張工作表（索引標籤），因此我們需要指定包含所需資料的工作表：

1. 在 **[!UICONTROL 工作表]** 下拉清單，選擇 **[!UICONTROL 專案]**.

   我們的試算表包含標題，而且我們希望模組能使用這些標題來識別我們要處理的資料：

   ![](assets/spreadsheet-headers-350x55.png)

1. 離開 **[!UICONTROL 是]** 已選擇 **[!UICONTROL 表格包含標題]**.

1. 在 **[!UICONTROL 含標題的列]** 框中，您可以指定要包含的行範圍，但將預設A1:Z1保留在此練習中。
1. 在 **[!UICONTROL 限制]** 框中，鍵入1。

   如此一來，每當您執行案例時，模組只會處理試算表中的1列。 這對於在建立案例時簡化測試執行很有幫助。

1. 按一下 **[!UICONTROL 確定]**.

   此 **[!UICONTROL 選擇要開始的位置]** 方塊會提示您指定試算表中要模組開始處理的位置。

1. 按一下 **[!UICONTROL 手動選擇]**，選取出現清單中的頂端選項，然後按一下 **[!UICONTROL 確定]**.
1. 以滑鼠右鍵按一下模組，按一下 **[!UICONTROL 重新命名]**，然後輸入描述您要模組執行的動作的名稱（例如「監看專案清單」），然後按一下 **[!UICONTROL 確定]**.

   名稱會顯示在模組正下方。 下面， [!DNL Workfront Fusion] 包括模組所執行動作類型的簡短說明。

   ![](assets/module-renamed-350x388.png)

1. 繼續 [新增及設定第二個模組](#add-and-configure-the-second-module).

## 新增及設定第二個模組

1. 按一下模組右側的部分圓圈，以 **[!UICONTROL 新增其他模組]**.

   第二個模組必須是 [!DNL Workfront] 模組，但我們沒有預裝 [!DNL Workfront] 應用程式。

1. 若要尋找 [!DNL Workfront] 應用程式，開始鍵入&quot;[!DNL Workfront]」，然後在應用程式出現時按一下。
1. 在 [!DNL Workfront] 顯示的模組，按一下 **[!UICONTROL 建立記錄]**.

1. 如您之前使用Google Sheets應用程式時，按一下 **[!UICONTROL 新增]** 在 [!DNL Workfront] 方塊來新增Workfront Fusion和Workfront之間的連線。

   現在，我們將開始指定要處理試算表中資料的方式。

1. 按一下 **[!UICONTROL 記錄類型]**，然後選取 **[!UICONTROL 專案]** 因為我們想在 [!DNL Workfront] 使用試算表中的列。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 專案]** 在清單中[!UICONTROL 專案].&quot;

   此方塊會展開並顯示所有可用的 [!DNL Workfront] 專案欄位，您可將第一個模組找到的資訊放入其中。

   我們將使用 **[!UICONTROL 名稱]** 欄位：我們希望此模組為 [!DNL Workfront] 在對應的 [!UICONTROL Google工作表] 行。

1. 尋找並按一下 **[!UICONTROL 名稱]** 欄位。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F**([!DNL Windows] OS)快速尋找欄位。

   這會開啟您可在 **[!UICONTROL 名稱]** 欄位來定義在Workfront中建立之每個專案的名稱。

   ![](assets/list-of-available-variables-350x261.png)

   請注意，清單頂端附近的變數對應至試算表中的欄標題。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 按一下變數 **[!UICONTROL 我的項目名(A)]** 將其新增至 **[!UICONTROL 名稱]** 欄位。

   您剛剛映射了此案例的第一個資料。

   讓我們將試算表中的一段資料對應至 [!DNL Workfront]:每個專案的開始日期。

1. 尋找並按一下 **[!UICONTROL 計劃開始日期]** 欄位，然後按一下 **[!UICONTROL 計劃開始日期(E)]** 變數，從試算表中的該欄提取資料。

1. 按一下 **[!UICONTROL 確定]**.

   現在您有了可行的案例。

1. 為第二個模組命名「建立Workfront專案」，然後繼續 [測試情境](#test-the-scenario).

## 測試情境

在啟用案例之前，請務必至少執行一次並檢視結果，以測試其效果。 這可協助您了解資料在案例中的流動方式，並找出任何錯誤。

我們選擇在試算表中處理1列，以在Workfront中建立專案。 如果執行案例，就會發生此情況。

1. 按一下 **[!UICONTROL 執行一次]** 在情境編輯器的左下角。
1. 執行完畢後，按一下 [!DNL Google Sheets] 模組。

   ![](assets/click-bubble.png)

   在隨即顯示的方塊中，您可以檢視模組處理之資料組合的相關資訊，包括從試算表中提取的實際資料（您開始使用的列）。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 按一下 [!DNL Workfront] 模組，查看資訊的輸入和輸出，即現在在 [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   您可以在下列文章中進一步了解如何閱讀案例執行資訊：

   * 如需一般資訊，請參閱 [中的方案執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 如需已處理套件組合的相關資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 前往 [!DNL Workfront] 找「soho downtown loft」，看看情景所創造的項目。 這是試算表中的最後一列。
1. 在 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 儲存]** ![](assets/save-icon.png) 在左下角附近，以儲存您對案例的進度。

   >[!IMPORTANT]
   >
   >磨練和測試情境時經常儲存。

## 最後確定方案並再次測試

我們仍需設定案例，以針對試算表中的所有其他列建立專案。

1. 按一下 **[!UICONTROL 監視行]** 您為Google工作表建立的模組。
1. 變更 **[!UICONTROL 限制]** 到100。

   指定高於您知道的試算表中列數的數字，可確保方案會擷取所有的列。

1. 以滑鼠右鍵按一下 **[!UICONTROL 監視行]** 模組，按一下 **[!UICONTROL 選擇要開始的位置]**，按一下 **[!UICONTROL 全部]**，然後按一下 **[!UICONTROL 確定]**.

1. 按一下 **[!UICONTROL 執行一次]** 看看執行檢查員泡泡里發生了什麼。

   此 [!DNL Google] 工作表 **[!UICONTROL 監視行]** 模組執行一次以讀取所有列。 然後Workfront **[!UICONTROL 建立記錄]** 模組會執行20次，為試算表中其餘20列的每一列建立專案。

1. 按一下 [!DNL Workfront] 模組，查看所有20個操作，然後按一下其中一個操作以查看有關已建立項目的資訊。
1. 按一下 **[!UICONTROL 儲存]** ![](assets/save-icon.png) 靠近左下角。
1. 前往 [!DNL Workfront] 以查看方案建立的專案。

>[!TIP]
>
>建議您使用選用但實用的作法，來新增關於每個模組的附註。
>
>1. 以滑鼠右鍵按一下 [!DNL Workfront] 模組，然後按一下 **[!UICONTROL 新增附註]**.
>1. 在顯示的附註中，輸入模組的概觀。

>
>   此功能很實用，因為您不需要持續開啟模組，就能查看其功能。 您可以輸入「建立專案，使用從試算表映射的名稱、計劃開始日期和優先順序」。
>
>   若 [!UICONTROL Google工作表] 模組中，您可以輸入「針對新增的新列/專案監看專案清單」之類的內容。
>
>   您可以為模組新增多個附註。
>
>1. 關閉 **[!UICONTROL 附註]** 的上界。
>
>   將附註新增至藍本後，橘點會顯示在 **[!UICONTROL 附註]** 圖示 ![](assets/notes-icon-w-dot.png) 在情境編輯器底部。
>
>1. 按一下 **[!UICONTROL 附註]** 圖示 ![](assets/notes-icon-w-dot.png) 來查看注釋。

>




## 啟動案例

如果這是您用於實際資料的案例，您最不要做的就是啟用它。 啟動案例後，依預設，每15分鐘執行一次。 您可以定義執行時間和頻率，以變更此設定。

如需啟用藍本的詳細資訊，請參閱 [啟用或停用Adobe Workfront Fusion中的案例](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

如需排程的相關資訊，請參閱 [排程Adobe Workfront Fusion中的案例](../../workfront-fusion/scenarios/schedule-a-scenario.md).
