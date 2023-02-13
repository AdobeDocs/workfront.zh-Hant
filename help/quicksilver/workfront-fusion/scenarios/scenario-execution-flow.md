---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的情境執行流程
description: 本文說明案例的執行方式，以及資料如何透過它流動。 此外也說明您可在何處找到已處理資料的相關資訊，以及如何讀取。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 中的方案執行流程 [!DNL Adobe Workfront Fusion]

本文說明案例的執行方式，以及資料如何透過它流動。 此外也說明您可在何處找到已處理資料的相關資訊，以及如何讀取。

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

## 方案執行流程

正確設定並啟動案例後，會根據其定義的排程執行。

當情境開始時，第一個模組會回應其已設定為監看的事件。 如果它返回任何包（資料），則它們會傳遞到下一個模組，然後情境會繼續，逐個將包傳遞到每個連續的模組。

如果套件組合在所有模組中都正確處理，則情境會在案例詳細資料區域中標示為成功，如 [中的方案詳細資料 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 如需設定案例的詳細資訊，請參閱 [中的基本案例設定 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 如需啟用案例的詳細資訊，請參閱 [在中啟用或停用案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 如需排程藍本的詳細資訊，請參閱 [在中排程藍本 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 如需模組的詳細資訊，請參閱 [模組類型](../../workfront-fusion/modules/module-types.md).

### 範例： [!UICONTROL [!DNL Workfront Fusion] 工作自動化]

>[!INFO]
>
>**範例：** 在以下情境中，會監視傳入的請求： [!DNL Workfront] 然後將它們轉換為 [!DNL Workfront] 項目中，資料會如下。
>
>案例的第一個步驟（由第一個模組執行）是監看請求。 每個傳入的要求都視為一個套件。 如果模組執行時未找到任何套件組合，則情境會在第一個模組之後結束。
>
>如果第一個模組傳回套件組合，套件組合會穿過其餘的案例。 在此範例中，其餘的案例包含第二個和最後一個模組，可將要求轉換為專案。
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 範例： [!UICONTROL [!DNL Workfront Fusion] 工作自動化和整合]

>[!INFO]
>
>**範例：** 在從 [!DNL Adobe Workfront] 並將它們傳送至 [!DNL Dropbox]，資料會如下流動。
>
>方案的第一步（由第一個模組執行）是監視套件組合（檔案）。 在此範例中，模組會監視 [!DNL Workfront]. 如果未傳回套件組合，案例會在第一個模組之後結束。
>
>如果傳回套件組合，套件組合會穿過其餘的案例。 在此範例中，其餘的案例包含第二個和最後一個模組，這會將套件組合上傳至 [!DNL Dropbox] 檔案夾。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一個模組傳回多個套件組合，則第一個套件組合會上傳至 [!DNL Dropbox] 上傳第二個套件組合之前。 然後第二個套件會上傳，然後再上傳第三個套件，依此類推。

## 已處理套件組合的相關資訊

對於每個模組，套件會先經過4個步驟的程式，再繼續前往下一個模組或到達其最終目的地。 四步過程是初始化、操作、提交/回滾和最終處理。 這稱為交易處理，有助於說明在模組中如何處理資料。

方案執行完成後，每個模組都會顯示圖示，顯示執行的操作數。 您可以按一下此圖示，以上述格式顯示已處理套件組合的詳細資訊。 您可以查看使用了哪些模組設定，以及哪個模組傳回了哪些套件組合。

![](assets/info-processed-bundles-350x396.png)

模組接收輸入資訊，例如：

* 轉換的影像
* 將影像上傳到的所選資料夾
* 原始名稱 [!DNL Facebook] 影像

處理後，模組返回以下輸出資訊：

* 影像ID指派者 [!DNL Dropbox]
* 進入的完整路徑 [!DNL Dropbox] [!DNL Workfront Fusion] 已上傳檔案

系統會分別擷取每個套件的上述資訊，如下拉式方塊所標示 [!UICONTROL 操作1] 和 [!UICONTROL 操作2] 在影像中。

有關事務處理的詳細資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 執行方案時出錯

方案執行期間可能會發生錯誤。 例如，如果您刪除 [!DNL Dropbox] 在模組設定中設定為目標資料夾的資料夾，此情境會終止，並顯示錯誤訊息。 如需如何處理錯誤的詳細資訊，請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
