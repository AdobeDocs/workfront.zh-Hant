---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在Adobe Workfront Fusion中擲回錯誤處理
description: 在某些情況下，您可能希望強制停止在回滾或提交階段之後的方案執行，或停止路由的處理，並選擇將其儲存在視圖隊列中，並解決Adobe Workfront Fusion中的不完整執行。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 在中擲回錯誤處理 [!DNL Adobe Workfront Fusion]

在某些情況下，您可能想要強制停止執行案例，隨後是 [回復](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 或 [提交](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 分階段或停止路由的處理，並可選擇將其儲存在未完成的執行隊列中。

當前，錯誤處理指令不能用於 [錯誤處理程式路由](../../workfront-fusion/errors/error-handling.md#error) 和 [!DNL Adobe Workfront Fusion] 不提供可讓您輕鬆有條件地產生（擲回）錯誤的模組。

有關未完成執行的資訊，請參見 [檢視並解決Adobe Workfront Fusion中的不完整執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

有關錯誤處理指令的資訊，請參見 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 擲回因應措施

若要有條件地擲回錯誤，您可以設定模組，讓其在操作期間選擇性地故意失敗。 一種可能是 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組(請參閱 [JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md))，可選地擲回錯誤（此例中為BundleValidationError）:

然後，可以將其中一個錯誤處理指令附加到錯誤處理路由，以：

* 強制執行方案以停止並執行回滾階段： [!UICONTROL 回復]
* 強制執行方案以停止並執行提交階段： [!UICONTROL 提交]
* 停止路由處理： [!UICONTROL 忽略]
* 停止路由的處理並將其儲存在未完成執行資料夾的隊列中： [!UICONTROL 插播]

下列範例說明 [!DNL Rollback] 指令：

![](assets/rollback-directive-350x175.png)
