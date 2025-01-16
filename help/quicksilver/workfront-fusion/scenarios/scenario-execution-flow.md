---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的案例執行流程
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的案例執行流程

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [案例執行流程](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-flow.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

本文說明情境如何執行以及資料如何流經情境。 本檔案也會說明您可在何處找到已處理資料的相關資訊，以及如何讀取這些資訊。

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

## 案例執行流程

正確設定並啟動情境後，情境會根據其定義的排程執行。

當案例開始時，第一個模組會回應已設定為要監視的事件。 如果它傳回任何組合（資料），它們會傳遞到下一個模組，而案例會繼續，逐一傳遞每個後續模組的組合。

如果所有模組的組合正確處理，則情境詳細資訊區域中會標示為成功，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)中的情境詳細資訊所說明。

* 如需設定案例的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)中的案例編輯器。
* 如需啟用案例的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中啟用或停用案例。
* 如需排程案例的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中排程案例。
* 如需模組的詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)。

### 範例：工作自動化]的[!UICONTROL [!DNL Workfront Fusion]

>[!INFO]
>
>**範例：**&#x200B;在監看[!DNL Workfront]中的傳入要求，然後將它們轉換成[!DNL Workfront]專案的案例中，資料將依照以下方式流動。
>
>此情境的第一個步驟由第一個模組執行，是觀察請求。 傳入的每個請求都視為一個組合。 如果模組執行時未發現任何組合，則案例會在第一個模組後結束。
>
>如果第一個模組傳回束，則束會通過案例的其餘部分。 在此範例中，此案例的其餘部分包含第二個和最後一個模組，此模組會將請求轉換為專案。
>
>？![](assets/example-execution-flow-wf-only-350x157.png)

### 範例：工作自動化與整合的[!UICONTROL [!DNL Workfront Fusion]]

>[!INFO]
>
>**範例：**&#x200B;在從[!DNL Adobe Workfront]下載檔案並將它們傳送到[!DNL Dropbox]中的資料夾的案例中，資料將按如下方式流動。
>
>此情境的第一個步驟由第一個模組執行，是監視組合（檔案）。 在此範例中，模組會監看[!DNL Workfront]中的組合。 如果不傳回套件組合，則案例會在第一個模組後結束。
>
>如果傳回束，則束會通過場景的其餘部分。 在此範例中，此案例的其餘部分包含第二個和最後一個模組，這個模組會將套件上傳至[!DNL Dropbox]資料夾。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一個模組傳回多個組合，則在上傳第二個組合之前，會將第一個組合上傳至[!DNL Dropbox]。 然後上傳第二個套件，再上傳第三個套件，依此類推。

## 已處理套裝的相關資訊

對於每個模組，此套件組合會先進行4步驟的流程，然後再繼續進行下一個模組或到達其最終目的地。 4步驟流程為「初始化」、「操作」、「認可/回覆」和「最終化」。 這稱為交易處理，有助於說明資料在模組中是如何處理的。

案例執行完成後，每個模組都會顯示一個圖示，顯示執行的運算元量。 您可以按一下此圖示，以上述格式顯示已處理套裝的詳細資訊。 您可以檢視哪些模組設定已使用，以及哪個模組傳回哪些組合。

![](assets/info-processed-bundles-350x396.png)

模組收到以下輸入資訊：

* 已轉換的影像
* 影像應上傳到的選取資料夾
* [!DNL Facebook]影像的原始名稱

處理之後，模組傳回以下輸出資訊：

* [!DNL Dropbox]指派的影像ID
* [!DNL Dropbox] [!DNL Workfront Fusion]中已上傳檔案的完整路徑

分別擷取每個套裝的上述資訊，如影像中的下拉式方塊[!UICONTROL 作業1]和[!UICONTROL 作業2]所標示。

如需交易處理的詳細資訊，請參閱[案例執行、週期和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的階段。

## 執行案例時發生錯誤

在案例執行期間可能會發生錯誤。 例如，如果您刪除在模組設定中設定為目標資料夾的[!DNL Dropbox]資料夾，情境會以錯誤訊息結束。 如需有關如何處理錯誤的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中的[錯誤處理。
