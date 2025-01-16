---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在Adobe Workfront Fusion中擲回錯誤處理
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中擲回錯誤處理

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [設定`throw`錯誤因應措施](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在某些情況下，您可能會想要強制停止案例執行，然後是[回覆](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)或[認可](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit)階段，或停止路由處理，並選擇性地將其儲存在未完成執行的佇列中。

目前，錯誤處理指示詞不能在[錯誤處理常式路由](../../workfront-fusion/errors/error-handling.md#error)的範圍之外使用，而且[!DNL Adobe Workfront Fusion]未提供可讓您輕易有條件產生（擲回）錯誤的模組。

如需有關未完成執行的資訊，請參閱[在Adobe Workfront Fusion中檢視及解決未完成的執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

如需錯誤處理指示的資訊，請參閱[指示在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中錯誤處理。

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
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 擲回的因應措施

若要有條件地擲回錯誤，您可以設定模組，使其在操作期間選擇性地故意失敗。 一種可能是採用[!UICONTROL JSON] > [!UICONTROL 剖析JSON]模組（請參閱[JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md)），其設定為可選擇擲回錯誤（在此例中為BundleValidationError）：

然後，您可以將其中一個錯誤處理指示附加至錯誤處理路由：

* 強制案例執行停止並執行復原階段： [!UICONTROL 復原]
* 強制案例執行停止並執行認可階段： [!UICONTROL 認可]
* 停止處理路由： [!UICONTROL 忽略]
* 停止處理路由，並將其儲存在未完成執行佇列資料夾： [!UICONTROL 中斷]

下列範例顯示[!DNL Rollback]指示詞的使用：

![](assets/rollback-directive-350x175.png)
