---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在中建立實踐自動化情境 [!DNL Adobe Workfront Fusion]
description: 本文會說明如何使用Adobe Workfront Fusion建立自動化案例。 自動化案例可自動化Workfront程式，包括資料操縱和轉換。 此範例將引導您完成建立案例的程式，該案例會搜尋專案，然後傳回與該專案相關聯的所有任務。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97231a6021aa4e897059063293e649f45dc9908d
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 0%

---

# 在中建立實踐自動化情境 [!DNL Adobe Workfront Fusion]

本文會說明如何使用Adobe Workfront Fusion建立自動化案例。 自動化案例可自動化Workfront程式，包括資料操縱和轉換。 此範例將引導您完成建立案例的程式，該案例會搜尋專案，然後傳回與該專案相關聯的所有任務。

如需有關建立可連線個別應用程式的整合情境的說明，請參閱 [在Adobe Workfront Fusion中建立實務整合情境](../../workfront-fusion/get-started/create-a-practice-scenario.md).

如需每個Workfront Fusion授權可用功能的詳細資訊，請參閱 [Adobe Workfront Fusion授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
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

## 建立實務情境

的作用 [!DNL Adobe Workfront Fusion] 是自動化您的流程，以便您可以專注於新任務，而不是一而再、再而三地重複相同的任務。 其運作方式是連結應用程式和服務內外的動作，以建立自動傳輸和轉換資料的情境。 您建立的案例會監視應用程式或服務中的資料，並處理該資料以提供您想要的結果。

案例由一系列模組組成，這些模組會指出應如何在應用程式內轉換資料，或在應用程式和Web服務之間傳輸資料。
此範例會帶您進行建立案例的過程，以搜尋 [!DNL Workfront] 並傳回專案中的任務。

![](assets/create-practice-scenario-wf-only-350x157.png)

建立情境包含數個主要工作：

## 選擇應用程式並命名情境

1. 登入您的 [!DNL Workfront Fusion] 帳戶。
1. 按一下 **[!UICONTROL 情境]** ![](assets/scenarios-icon.png) 在左側面板中。

   >[!NOTE]
   >
   >如果您看不到左側導覽面板或其圖示，請按一下「功能表」 ![選單](assets/main-menu-icon-left-nav.png) 圖示。

   在灰色 [!UICONTROL 資料夾] 在顯示的面板中，您可以將情境組織到資料夾中。

   在右邊主要區域的頂端，您可以檢視 **[!UICONTROL 全部]** 您已建置的情境，您的 **[!UICONTROL 作用中案例]**， **[!UICONTROL 非使用中案例]**、和 **[!UICONTROL 概念]**. 概念是之前需要更多工作的情境 [!DNL Workfront Fusion] 可將它們分類為作用中或非作用中。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. 在 [!UICONTROL 資料夾] 面板，按一下 **[!UICONTROL 新增資料夾]** 圖示 ![](assets/add-folder-icon.png)，然後為第一個資料夾輸入名稱，如「Practice scenarios」。

1. 開啟資料夾，然後按一下 **[!UICONTROL 建立新情境]** 在頁面的右上角。

   顯示的登入頁面可讓您預先載入您要在要建立的情境中使用的任何應用程式。

1. 在本練習中，請搜尋並選取 **[!DNL Workfront]** 應用程式。
1. 按一下 **[!UICONTROL 繼續]** 位於右上角。

   情境編輯器隨即顯示，其中心包含一個空白模組， [!DNL Workfront] 已預先載入的應用程式，以及底部工具列中的某些選項。

<!--
   ![](assets/scenario-editor-350x235.png)
-->

當您開始建立新情境時，最好從建立其名稱開始。

1. 選取 **[!UICONTROL 新情境]** 左上角的預留位置名稱，然後輸入名稱，例如「Practice scenario 1」。
1. 繼續使用 [新增並設定第一個模組](#add-and-configure-the-first-module) 底下。

## 新增並設定第一個模組

帶有問號的空白模組代表您需要新增的觸發程式模組。 此模組將在每次執行時啟動情境。 空白模組上的時鐘圖示表示是排程模組。

![](assets/empty-module.png)

此模組將包含您想要案例觀看的資料。

在此範例中，我們並未使用觸發程式模組。 相反地，此案例始於搜尋。

1. 按一下空白模組，以選擇要從中選取模組的應用程式。

   您先前預先載入的應用程式會顯示在空白模組旁。 您可以使用 [!UICONTROL 搜尋] 方塊。

   ![](assets/pre-loaded-app-wf-350x172.png)

1. 按一下 **[!DNL Workfront]**.

   清單會變更為全部顯示 [!DNL Workfront] 可作為觸發模組的模組。

1. 按一下搜尋模組 **[!UICONTROL 搜尋]**.

   現在您必須建立已驗證的連線，以連線至 [!DNL Workfront] 帳戶。 您新增至情境的每個模組都必須有與其應用程式的連線。

1. 在 **[!DNL Workfront]** 方塊，下 **[!UICONTROL 連線]**，按一下 **[!UICONTROL 新增]**，然後輸入連線的名稱，例如「Olivia的Workfront帳戶」，然後按一下 **[!UICONTROL 繼續]**.
1. 在顯示的視窗中驗證連線。

   驗證連線的程式可能會因應用程式而異。 以下流程專屬於 [!DNL Workfront]，但程式與許多應用程式類似。

   1. 輸入您的 [!DNL Workfront] 網域，然後按一下 **[!UICONTROL 繼續]**.
   1. 登入 [!DNL Workfront].
   1. 檢查以下存取許可權： [!DNL Workfront Fusion] 正在請求，然後按一下 **[!UICONTROL 允許存取]**.

   如果您需要協助，請參閱 [連線總覽](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 設定第一個模組

連線之後 [!DNL Workfront Fusion] 至您的 [!DNL Workfront] 帳戶，您可以指定 [!DNL Workfront] 您可存取的請求佇列，以及您希望第一個模組處理的資料。

1. 在 [!UICONTROL 記錄型別] 方塊，選取 **[!UICONTROL 專案]**. 這會將模組設定為僅搜尋專案。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 專案]** 在清單中(如果您開始輸入&quot;[!UICONTROL 專案].」

1. 在 **[!UICONTROL 結果集]** 方塊，選取 **[!UICONTROL 第一個比對記錄]**. 這會將模組設定為只傳回它認為符合條件的第一個記錄。 在此範例中，我們只需要傳回一個記錄。
1. 在 **[!UICONTROL 搜尋條件]** 區域，我們將設定篩選器以傳回特定專案。

   1. 在下的第一個方塊中 [!UICONTROL 搜尋條件]，選取您要搜尋其值的欄位。 在此範例中，選取 **[!UICONTROL 名稱]**.
   1. 對於運運算元，選取 [!UICONTROL 包含（區分大小寫）]. 如此一來，模組便可尋找名稱中包含您所選字詞的專案，即使您並未輸入完整名稱或輸入大小寫不正確（例如全部大寫）的名稱亦然。
   1. 在底下的最後一個欄位中 [!UICONTROL 搜尋條件]，輸入您知道位於搜尋專案名稱中的字詞或片語。

1. 在 **[!UICONTROL 輸出]** 清單中，選取您要模組輸出的欄位。 在此範例中，選取 **[!UICONTROL ID]** 和 **[!UICONTROL 名稱]** 欄位。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] 作業系統)或 **Ctrl-F** ([!DNL Windows] OS)以快速找到欄位。

1. 按一下 **[!UICONTROL 確定]**.

   >[!NOTE]
   >
   >（僅供參考）由於這不是觸發程式模組，因此您不會選擇從何處啟動。 使用觸發程式模組時，您現在可以選擇從何處開始執行。
   >
   >
   >如需詳細資訊，請參閱 [選擇觸發程式模組開始的位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. 以滑鼠右鍵按一下模組，然後按一下 **[!UICONTROL 重新命名]**，然後輸入名稱，說明您希望模組執行的動作（例如「搜尋專案」），然後按一下 **[!UICONTROL 確定]**.

   名稱會出現在模組正下方。 在底下， [!DNL Workfront Fusion] 包含模組所執行動作型別的簡短說明。

   ![](assets/module-renamed-wf.png)

1. 繼續使用 [新增並設定第二個模組](#add-and-configure-the-second-module).

## 新增並設定第二個模組

1. 按一下模組右側的部分圓圈，以 **[!UICONTROL 新增另一個模組]**.
1. 選取 [!DNL Workfront] 從應用程式清單中，然後選擇搜尋模組 **[!UICONTROL 讀取相關記錄]**.
1. 您已建立與的連線 [!DNL Workfront] 用於上一個模組。 您不需要在這裡再次建立，但您必須確定此模組使用與上一個模組相同的連線。\
   在 **[!UICONTROL 連線]** 方塊中，選取您為上一個模組建立的連線。
1. 按一下 **[!UICONTROL 記錄型別]**，然後選取 **[!UICONTROL 專案]**，因為我們要讀取與專案相關的記錄。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 專案]** 如果您開始輸入「專案」這個字，請在清單中選取。

1. 按一下 **[!UICONTROL 父記錄ID]** 欄位。 此欄位需要您想要傳回任務之專案的Workfront ID。

   按一下欄位會開啟您可在以下專案中使用的變數清單： **[!UICONTROL 父記錄ID]** 用來識別Workfront中專案的欄位。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 按一下變數 **[!UICONTROL ID]** 將其新增至 **[!UICONTROL 父記錄ID]** 欄位。 這可讓從第一個模組傳回的ID用來作為您要在第二個模組處理的專案識別碼，以確保傳回的任務將屬於該專案。
1. 在 **[!UICONTROL 集合]** 欄位，選取 **[!UICONTROL 任務]**. 這表示模組將傳回與所選專案相關的任務。
1. 按一下 **[!UICONTROL 確定]**

   現在您有工作情境了。

1. 為第二個模組命名，例如「傳回與專案關聯的任務」，然後繼續 [測試情境](#test-the-scenario).

## 測試情境

在啟動情境之前，請務必執行情境至少一次，並檢視結果，以測試情境。 這有助於您瞭解資料如何流經此情境並找出任何錯誤。

我們選擇傳回1個專案，以及與專案關聯的任務。 如果您執行情境，應該就會發生這種情況。

1. 按一下 **[!UICONTROL 執行一次]** 位於情境編輯器的左下角。
1. 情境執行完畢後，按一下第一個模組上方的泡泡。

   ![](assets/click-bubble.png)

   在出現的方塊中，您可以檢視模組所處理資料束的相關資訊，包括從模組傳回的專案中提取的實際資料。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 按一下第二個模組上方的執行檢查器泡泡圖，以檢視資訊的輸入和輸出，這是專案中包含的工作集合。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   您可在下列文章中進一步瞭解如何閱讀案例執行資訊：

   * 如需一般資訊，請參閱 [中的案例執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 如需已處理套裝的詳細資訊，請參閱 [中的案例執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 在 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 儲存]** ![](assets/save-icon.png) 靠近左下角，儲存情境的進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

>[!TIP]
>
>我們建議您選擇加入每個模組相關附註的作法，但此作法相當實用。
>
>1. 用滑鼠右鍵按一下 [!DNL Workfront] 模組，然後按一下 **[!UICONTROL 新增附註]**.
>1. 在顯示的附註中，輸入模組的概觀。
>
>    您可以為一個模組新增多個附註。
>
>1. 關閉 **[!UICONTROL 附註]** 區域。
>
>     將附註新增至情境後， **[!UICONTROL 附註]** 圖示 ![](assets/notes-icon-w-dot.png) 位於案例編輯器底部。
>
>1. 按一下 **[!UICONTROL 附註]** 圖示 ![](assets/notes-icon-w-dot.png) 以檢視您的附註。
>



## 啟動情境

此範例案例沒有觸發程式模組。 如果這是您用於真實資料的情境，它會從觸發模組開始，而您的最後一件事是啟動它。 啟用案例後，預設會每15分鐘執行一次。 您可以定義何時以及多久執行一次來變更此專案。

如需啟用案例的詳細資訊，請參閱 [啟用或停用中的案例 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

如需排程的相關資訊，請參閱 [在中排程情境 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
