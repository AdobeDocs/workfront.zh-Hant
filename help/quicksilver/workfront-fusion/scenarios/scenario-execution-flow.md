---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的案例執行流程
description: 本文說明案例如何執行以及資料如何流經案例。 本檔案也會說明您可在何處找到已處理資料的相關資訊，以及如何讀取資料。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# 案例執行流程 [!DNL Adobe Workfront Fusion]

本文說明案例如何執行以及資料如何流經案例。 本檔案也會說明您可在何處找到已處理資料的相關資訊，以及如何讀取資料。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 案例執行流程

正確設定並啟動情境後，情境會根據其定義的排程執行。

當案例開始時，第一個模組會回應已設定為要監視的事件。 如果它傳回任何組合（資料），則會傳遞至下一個模組，而案例會繼續，將組合逐一傳遞至每個後續模組。

如果所有模組的套件組合皆正確處理，則情境會在情境詳細資訊區域中標示為成功，如中所述 [中的案例詳細資料 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 如需設定案例的詳細資訊，請參閱 [中的基本案例設定 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 如需啟用情境的詳細資訊，請參閱 [啟用或停用中的情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 如需排程情境的詳細資訊，請參閱 [排程情境於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 如需模組的詳細資訊，請參閱 [模組型別](../../workfront-fusion/modules/module-types.md).

### 範例： [!UICONTROL [!DNL Workfront Fusion] 工作自動化]

>[!INFO]
>
>**範例：** 在監視傳入請求的案例中 [!DNL Workfront] 然後將其轉換為 [!DNL Workfront] 專案，資料會依照以下方式流動。
>
>此情境的第一個步驟（由第一個模組執行）是監視請求。 傳入的每個請求都視為一個組合。 如果模組執行時未發現任何組合，則案例會在第一個模組後結束。
>
>如果第一個模組傳回一個組合，該組合會通過案例的其餘部分。 在此範例中，此情境的其餘部分包含第二個和最後一個模組，此模組會將請求轉換為專案。
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 範例： [!UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合]

>[!INFO]
>
>**範例：** 在下載檔案來源情境中 [!DNL Adobe Workfront] 並傳送至中的資料夾 [!DNL Dropbox]，資料會依照以下方式流動。
>
>此情境的第一個步驟（由第一個模組執行）是監視組合（檔案）。 在此範例中，模組會監看中的套件組合 [!DNL Workfront]. 如果不傳回組合，則案例會在第一個模組後結束。
>
>如果傳回束，則束會通過場景的其餘部分。 在此範例中，此情境的其餘部分包含第二個和最後一個模組，此模組會將套件上傳至 [!DNL Dropbox] 資料夾。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一個模組傳回多個組合，則會將第一個組合上傳至 [!DNL Dropbox] 上傳第二個套件組合之前。 然後上傳第二個組合，再上傳第三個組合，依此類推。

## 已處理套裝的相關資訊

對於每個模組，套件組合會先經過4個步驟的流程，再繼續前往下一個模組或到達其最終目的地。 這4個步驟的流程是「初始化」、「操作」、「認可/回覆」和「最終化」。 這稱為交易處理，有助於說明資料在模組中是如何處理的。

案例執行完成後，每個模組都會顯示一個圖示，顯示執行的運算元量。 您可以按一下此圖示，以上述格式顯示已處理套裝的詳細資訊。 您可以檢視哪些模組設定已使用，以及哪個模組傳回哪些組合。

![](assets/info-processed-bundles-350x396.png)

模組已接收輸入資訊，例如：

* 已轉換的影像
* 選取要將影像上傳到的資料夾
* 的原始名稱 [!DNL Facebook] 影像

處理之後，模組傳回以下輸出資訊：

* 影像ID指派者 [!DNL Dropbox]
* 中的完整路徑 [!DNL Dropbox] [!DNL Workfront Fusion] 已上傳檔案

系統會分別擷取每個套件的上述資訊，如下拉式方塊所標示 [!UICONTROL 作業1] 和 [!UICONTROL 作業2] 在影像中。

如需交易處理的詳細資訊，請參閱 [中的案例執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 執行案例時發生錯誤

案例執行期間可能會發生錯誤。 例如，如果您刪除 [!DNL Dropbox] 在模組設定中設定為目標資料夾的資料夾，此案例會以錯誤訊息終止。 如需如何處理錯誤的詳細資訊，請參閱 [中的處理錯誤 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
