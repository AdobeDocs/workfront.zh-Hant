---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在中建立實踐自動化案例 [!DNL Adobe Workfront Fusion]
description: 本文說明如何使用Adobe Workfront Fusion建立自動化案例。 自動化案例可自動化Workfront程式，包括資料操控和轉換。 此示例將帶您完成建立方案的過程，該方案將搜索項目，然後返回與該項目關聯的所有任務。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# 在中建立實踐自動化案例 [!DNL Adobe Workfront Fusion]

本文說明如何使用Adobe Workfront Fusion建立自動化案例。 自動化案例可自動化Workfront程式，包括資料操控和轉換。 此示例將帶您完成建立方案的過程，該方案將搜索項目，然後返回與該項目關聯的所有任務。

如需建立可連接個別應用程式之整合案例的指示，請參閱 [在Adobe Workfront Fusion中建立實務整合案例](../../workfront-fusion/get-started/create-a-practice-scenario.md).

如需每個Workfront Fusion授權可用功能的詳細資訊，請參閱 [Adobe Workfront Fusion授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
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
此範例將逐步引導您建立會搜尋 [!DNL Workfront] 專案，並傳回專案中的任務。

![](assets/create-practice-scenario-wf-only-350x157.png)

建立案例包含數個主要工作：

## 選擇應用程式並為案例命名

1. 登入 [!DNL Workfront Fusion] 帳戶。
1. 按一下 **[!UICONTROL 藍本]** ![](assets/scenarios-icon.png) 中。

   在顯示的左側面板中，您可以將藍本組織到資料夾中。

   在右側的主區域頂端，您可以檢視 **[!UICONTROL 全部]** 您建立的方案， **[!UICONTROL 活動方案]**, **[!UICONTROL 非活動方案]**，和 **[!UICONTROL 概念]**. 概念是之前需要做更多工作的案例 [!DNL Workfront Fusion] 可將其分類為使用中或非使用中。

   ![](assets/scenarios-left-panel-350x215.png)

1. 在左側面板中，按一下 **[!UICONTROL 新增資料夾]** 圖示 ![](assets/add-folder-icon.png)，然後為第一個資料夾輸入「實務案例」之類的名稱。

1. 開啟資料夾，然後按一下 **[!UICONTROL 建立新藍本]** 在頁面的右上角。

   顯示的登錄頁面可讓您預先載入您要建立的案例中要使用的任何應用程式。

1. 對於本練習，請搜尋並選取 **[!DNL Workfront]** 應用程式。
1. 按一下 **[!UICONTROL 繼續]** 在右上角。

   隨即顯示情境編輯器，其中包含中央的空模組， [!DNL Workfront] 應用程式預先載入，以及工具列底部的某些選項。

   ![](assets/scenario-editor-350x235.png)

   當您開始建立新案例時，最好先為其建立名稱。

1. 選取 **[!UICONTROL 新藍本]** 左上角的預留位置名稱，然後輸入名稱，例如「實務案例1」。
1. 繼續 [新增及設定第一個模組](#add-and-configure-the-first-module) 下方。

## 新增及設定第一個模組

帶有問號的空白模組代表您需要新增的觸發程式模組。 此模組每次執行時都會啟動案例。 空模組上的時鐘圖示表示是已排程的模組。

![](assets/empty-module.png)

此模組將包含您希望藍本監視的資料。

在此範例中，我們未使用觸發程式模組。 相反，此情境從搜尋開始。

1. 按一下空白模組，以選擇您要從中選取模組的應用程式。

   您先前預先載入的應用程式會顯示在空白模組旁。 您可以使用 [!UICONTROL 搜尋] 框。

   ![](assets/pre-loaded-app-wf-350x172.png)

1. 按一下 **[!DNL Workfront]**.

   清單會變更為全部顯示 [!DNL Workfront] 可作為觸發模組的模組。

1. 按一下「搜尋模組」 **[!UICONTROL 搜尋]**.

   現在，您需要建立已驗證的連線至 [!DNL Workfront] 帳戶。 您新增至案例的每個模組都必須有與其應用程式的連線。

1. 在 **[!DNL Workfront]** 框下 **[!UICONTROL 連線]**，按一下 **[!UICONTROL 新增]**，然後輸入連線的名稱，例如「Olivia的Workfront帳戶」，然後按一下 **[!UICONTROL 繼續]**.
1. 在顯示的視窗中驗證連線。

   驗證連線的程式可能會在應用程式之間有所不同。 下列程式是 [!DNL Workfront]，但此程式與許多應用程式類似。

   1. 輸入 [!DNL Workfront] 網域，然後按一下 **[!UICONTROL 繼續]**.
   1. 登入 [!DNL Workfront].
   1. 檢查 [!DNL Workfront Fusion] 請求，然後按一下 **[!UICONTROL 允許存取]**.

   如果您需要幫助，請參閱 [關於連接 [!DNL Adobe Workfront Fusion] 至應用程式或服務](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 設定第一個模組

連接後 [!DNL Workfront Fusion] 至 [!DNL Workfront] 帳戶，您可以指定 [!DNL Workfront] 要求您有權存取的佇列，以及您要第一個模組處理的資料。

1. 在 [!UICONTROL 記錄類型] 框，選擇 **[!UICONTROL 專案]**. 這會將模組設為僅搜尋專案。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 專案]** 在清單中[!UICONTROL 專案].&quot;

1. 在 **[!UICONTROL 結果集]** 框，選擇 **[!UICONTROL 第一個匹配記錄]**. 這會設定模組，僅傳回其找到符合條件的第一個記錄。 在此範例中，我們只需傳回一個記錄。
1. 在 **[!UICONTROL 搜尋條件]** 區域，我們會設定篩選器以傳回特定專案。

   1. 在 [!UICONTROL 搜尋條件]，選擇要搜索值的欄位。 在此範例中，選取 **[!UICONTROL 名稱]**.
   1. 對於運算子，請選取 [!UICONTROL 包含（不區分大小寫）]. 這可讓模組尋找專案，其名稱中會包含您選取的字詞，即使您未輸入整個名稱，或輸入名稱且大小寫不正確（例如大寫）。
   1. 在下方的最後一個欄位中 [!UICONTROL 搜尋條件]，請在所搜索項目的名稱中輸入您知道的單詞或短語。

1. 在 **[!UICONTROL 輸出]** 清單中，選擇要輸出問題的欄位。 在此範例中，選取 **[!UICONTROL ID]** 和 **[!UICONTROL 名稱]** 欄位。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F** ([!DNL Windows] OS)快速尋找欄位。

1. 按一下 **[!UICONTROL 確定]**.

   >[!NOTE]
   >
   >（僅限資訊）由於這不是觸發模組，因此您不會選擇啟動它的位置。 使用觸發程式模組時，您現在會選取要啟動它的位置。
   >
   >
   >如需詳細資訊，請參閱 [選擇觸發程式模組的起始位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. 以滑鼠右鍵按一下模組，按一下 **[!UICONTROL 重新命名]**，然後輸入描述您要模組執行的操作的名稱（例如「搜尋專案」），然後按一下 **[!UICONTROL 確定]**.

   名稱會顯示在模組正下方。 下面， [!DNL Workfront Fusion] 包括模組所執行動作類型的簡短說明。

   ![](assets/module-renamed-wf.png)

1. 繼續 [新增及設定第二個模組](#add-and-configure-the-second-module).

## 新增及設定第二個模組

1. 按一下模組右側的部分圓圈，以 **[!UICONTROL 新增其他模組]**.
1. 選擇 [!DNL Workfront] 從應用程式清單中，選擇搜索模組 **[!UICONTROL 讀取相關記錄]**.
1. 您已建立連線至 [!DNL Workfront] 上一個模組。 您不需要在此處再次建立，但必須確定此模組使用與上一個模組相同的連線。\
   在 **[!UICONTROL 連線]** 框中，選擇您為上一個模組建立的連接。
1. 按一下 **[!UICONTROL 記錄類型]**，然後選取 **[!UICONTROL 專案]**，因為我們想要讀取與專案相關的記錄。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 專案]** 在清單中輸入「project」。

1. 按一下 **[!UICONTROL 父記錄ID]** 欄位。 此欄位需要您要傳回任務之專案的Workfront ID。

   按一下欄位會開啟您可在 **[!UICONTROL 父記錄ID]** 欄位來識別Workfront中的專案。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 按一下變數 **[!UICONTROL ID]** 將其新增至 **[!UICONTROL 父記錄ID]** 欄位。 這可讓您將第一個模組傳回的ID，用作您要在第二個模組中使用之專案的識別碼，以確保傳回的任務會屬於該專案。
1. 在 **[!UICONTROL 集合]** 欄位，選擇 **[!UICONTROL 工作]**. 這表示模組將返回與所選項目關聯的任務。
1. 按一下 **[!UICONTROL 確定]**

   現在您有了可行的案例。

1. 為第二個模組命名「回傳與專案相關聯的工作」，然後繼續 [測試情境](#test-the-scenario).

## 測試情境

在啟用案例之前，請務必至少執行一次並檢視結果，以測試其效果。 這可協助您了解資料在案例中的流動方式，並找出任何錯誤。

我們選擇返回1個項目，以及與該項目相關的任務。 如果執行案例，就會發生此情況。

1. 按一下 **[!UICONTROL 執行一次]** 在情境編輯器的左下角。
1. 執行完情境後，按一下第一個模組上方的泡泡。

   ![](assets/click-bubble.png)

   在隨即顯示的方塊中，您可以檢視模組處理之資料組合的相關資訊，包括從模組傳回之專案提取的實際資料。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 按一下「第二個」模組上方的執行檢查器泡泡，查看資訊的輸入和輸出，該輸出是項目中包含的任務的集合。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   您可以在下列文章中進一步了解如何閱讀案例執行資訊：

   * 如需一般資訊，請參閱 [中的方案執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 如需已處理套件組合的相關資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 在 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 儲存]** ![](assets/save-icon.png) 在左下角附近，以儲存您對案例的進度。

   >[!IMPORTANT]
   >
   >磨練和測試情境時經常儲存。

>[!TIP]
>
>建議您使用選用但實用的作法，來新增關於每個模組的附註。
>
>1. 以滑鼠右鍵按一下 [!DNL Workfront] 模組，然後按一下 **[!UICONTROL 新增附註]**.
>1. 在顯示的附註中，輸入模組的概觀。

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

此範例案例沒有觸發器模組。 如果這是您用於實際資料的案例，則會從觸發模組開始，最後一件事就是啟動它。 啟動案例後，依預設，每15分鐘執行一次。 您可以定義執行時間和頻率，以變更此設定。

如需啟用藍本的詳細資訊，請參閱 [在中啟用或停用案例 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

如需排程的相關資訊，請參閱 [在中排程藍本 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
