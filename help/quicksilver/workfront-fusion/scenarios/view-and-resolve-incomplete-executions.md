---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中檢視和解決未完成的執行 [!DNL Adobe Workfront Fusion]
description: 此 [!UICONTROL 未完成的執行] 資料夾儲存因錯誤而未成功完成的案例執行。 每個儲存的不完整執行都可以手動或自動解決。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 在中檢視和解決未完成的執行 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 未完成的執行] 資料夾儲存因錯誤而未成功完成的案例執行。 每個儲存的不完整執行都可以手動或自動解決。

>[!NOTE]
>
>依預設，不完整執行的儲存已停用。 若要啟用此功能，請啟用 [!UICONTROL 允許儲存未完成的執行] 情境進階設定中的選項。
>
>如需案例設定的詳細資訊，請參閱 [中的案例設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## 檢視未完成的執行

如果模組在操作期間遇到錯誤，則會將新的未完成執行新增到未完成執行資料夾。 每個未完成的執行都包含情境的藍圖以及可對應至失敗模組的所有套件組合。 您可以按一下 [!UICONTROL 未完成的執行] 「案例詳細資訊」頁面上的標籤：

![](assets/incomplete-executions-tab-350x102.png)

如需詳細資訊，請參閱 [導致不完整執行的錯誤](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>每個組織未解決未完成執行資料夾的目前大小限製為500 MB。 如果您的組織超過此限制，您可能會看到下列錯誤：
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>如需詳細資訊，請參閱 [啟用資料遺失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 在 [中的案例設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 解決不完整的執行

儲存新的未完成執行時，您可以依照以下方式解析它：

1. 按一下 **[!UICONTROL 未完成的執行]** 標籤。
1. 找到您要解析的未完成執行，然後按一下 **[!UICONTROL 詳細資訊]**.


   如果您想在嘗試解析未完成的執行之前檢視所有模組作業的記錄，您可以從 [!UICONTROL 歷史記錄] 資料夾：

1. 按一下 **[!UICONTROL 歷史記錄]** 標籤。
1. 找到案例失敗的執行記錄檔，然後按一下 **[!UICONTROL 詳細資料]**.
1. 開啟模組的記錄，其中顯示所有模組的操作。
1. 找到失敗的作業，然後按一下 **[!UICONTROL 解決]**：

   ![](assets/resolve-btn-350x188.png)

## 與未完成執行相關的選項

下列選項位於 [!UICONTROL 案例設定] 面板決定是否要儲存未完成的執行以及儲存方式：

* 允許儲存未完成的執行
* 循序處理
* 啟用資料遺失

如需這些選項的詳細資訊，請參閱 [中的案例設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 導致不完整執行的錯誤

有幾種錯誤類別會導致儲存不完整的執行。 這些可能包括：

* 驗證錯誤源於不完整或錯誤的資料，大多是因為遺漏了預期的專案，以便成功處理通過模組的所有資料。
* 由於暫時或長期的連線失敗（例如，連線至電子郵件或遠端FTP伺服器期間）而導致最終目的地無法使用而發生的錯誤。

如果情境中的第一個模組發生錯誤，執行會立即停止，且不會儲存不完整的執行。

如果任何其他模組發生錯誤，且沒有附加錯誤處理常式路由，則會發生下列其中一種情況：

* 如果錯誤型別為 `ConnectionError`， `RateLimitError`， `OutOfSpaceError` 或 `ModuleTimeoutError`，會儲存具有自動重試的不完整執行記錄。
* 如果錯誤型別為 `DataError`， `InvalidConfigurationError`， `InvalidAccessTokenError`， `UnexpectedError`， `MaxFileSizeExceededError`，或 `MaxResultsExceededError`，會儲存不含自動重試的不完整執行記錄。
* 如果錯誤型別不是上述型別，則執行會失敗。
