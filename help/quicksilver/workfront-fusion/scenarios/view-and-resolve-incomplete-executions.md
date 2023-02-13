---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]
description: 此 [!UICONTROL 未完成執行] 資料夾儲存方案執行由於錯誤而未成功完成。 每個儲存的不完整執行都可手動或自動解決。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 未完成執行] 資料夾儲存方案執行由於錯誤而未成功完成。 每個儲存的不完整執行都可手動或自動解決。

>[!NOTE]
>
>預設情況下，不完整執行的儲存將被禁用。 若要啟用，請啟用 [!UICONTROL 允許儲存不完整的執行] 選項。
>
>如需藍本設定的詳細資訊，請參閱 [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## 查看未完成的執行

如果模組在操作過程中遇到錯誤，則會將新的未完成執行添加到「未完成執行」資料夾。 每個未完成的執行都包含方案的Blueprint以及可映射到失敗模組的所有套件組合。 按一下 [!UICONTROL 未完成執行] 頁簽上的「方案詳細資訊」頁簽：

![](assets/incomplete-executions-tab-350x102.png)

如需詳細資訊，請參閱 [導致執行不完整的錯誤](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>每個組織未解決的未完成執行資料夾的當前大小限制為500 MB。 如果貴組織超過此限制，您可能會看到下列錯誤：
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>如需詳細資訊，請參閱 [啟用資料丟失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 解決不完整的執行

儲存新的未完成執行時，您可以依下列方式加以解析：

1. 按一下 **[!UICONTROL 未完成執行]** 標籤。
1. 找到要解決的未完成執行，然後按一下 **[!UICONTROL 詳細資料]**.


   如果您想在嘗試解析未完成的執行之前查看所有模組操作的日誌，則可以從 [!UICONTROL 歷史記錄] 資料夾：

1. 按一下 **[!UICONTROL 歷史記錄]** 標籤。
1. 找到方案的失敗執行日誌，然後按一下 **[!UICONTROL 詳細資料]**.
1. 開啟模組的日誌，其中顯示模組的所有操作。
1. 找到失敗的操作，然後按一下 **[!UICONTROL 解決]**:

   ![](assets/resolve-btn-350x188.png)

## 與未完成執行相關的選項

下列選項 [!UICONTROL 藍本設定] 面板確定未完成執行的儲存方式：

* 允許儲存不完整的執行
* 循序處理
* 啟用資料丟失

如需這些選項的詳細資訊，請參閱 [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 導致執行不完整的錯誤

存在幾類錯誤，導致儲存不完整的執行。 這些可能包括：

* 驗證錯誤是因資料不完整或錯誤而產生，主要是因為遺漏了預期的項目，以成功處理通過模組的所有資料。
* 由於暫時或長期連線失敗（例如連線至電子郵件或遠端FTP伺服器期間），導致最終目的地無法使用而發生的錯誤。

如果情境中的第一個模組發生錯誤，則執行會立即停止，且不會儲存不完整的執行。

如果任何其他模組發生錯誤，且未附加錯誤處理程式路由，則會發生以下情況之一：

* 如果錯誤類型為 `ConnectionError`, `RateLimitError`, `OutOfSpaceError` 或 `ModuleTimeoutError`，則會儲存自動重試的不完整執行記錄。
* 如果錯誤類型為 `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`，或 `MaxResultsExceededError`，會儲存未自動重試的未完成執行記錄。
* 如果錯誤類型不是上述任何值，則執行會失敗。
