---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在Adobe Workfront Fusion中處理擲回錯誤
description: 在某些情況下，您可能會想要強制停止案例執行，然後是「復原」或「認可」階段，或停止處理路由，並選擇性地將其儲存在「檢視」佇列中，並解決Adobe Workfront Fusion中的不完整執行。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 在中擲回錯誤處理 [!DNL Adobe Workfront Fusion]

在某些情況下，您可能想要強制停止案例執行，然後執行 [復原](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 或 [認可](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 階段或停止處理路由，並選擇性地將其儲存在未完成執行的佇列中。

目前，錯誤處理指示詞不能用於 [錯誤處理常式路由](../../workfront-fusion/errors/error-handling.md#error) 和 [!DNL Adobe Workfront Fusion] 不提供可讓您輕鬆有條件產生（擲回）錯誤的模組。

如需不完整執行的資訊，請參閱 [在Adobe Workfront Fusion中檢視和解決未完成的執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

如需錯誤處理指示的詳細資訊，請參閱 [中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
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

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 擲回的因應措施

若要有條件地擲回錯誤，您可以設定模組，使其在操作期間選擇性地故意失敗。 一種可能方式是採用 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組(請參閱 [JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md))，設定為選擇性擲回錯誤（在此例中為BundleValidationError）：

然後，您可以將其中一個錯誤處理指示附加至錯誤處理路由：

* 強制案例執行停止並執行倒回階段： [!UICONTROL 復原]
* 強制案例執行停止並執行認可階段： [!UICONTROL 認可]
* 停止處理路由： [!UICONTROL 忽略]
* 停止處理路由，並將其儲存在未完成執行佇列資料夾中： [!UICONTROL 中斷]

以下範例說明如何使用 [!DNL Rollback] 指令：

![](assets/rollback-directive-350x175.png)
