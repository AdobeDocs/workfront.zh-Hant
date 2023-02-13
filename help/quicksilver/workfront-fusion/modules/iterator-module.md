---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的迭代器模組
description: 迭代器模組是將陣列轉換為一系列捆綁的特殊類型模組。 每個陣列項作為單獨的束輸出。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL 迭代器] 模組 [!DNL Adobe Workfront Fusion]

安 [!UICONTROL 迭代器] 模組是將陣列轉換為一系列套件的特殊類型模組。 每個陣列項作為單獨的束輸出。

如需詳細資訊，請參閱 [模組類型](../../workfront-fusion/modules/module-types.md) 和 [在Adobe Workfront Fusion中對應陣列](../../workfront-fusion/mapping/map-an-array.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買Adobe Workfront Fusion和Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 迭代器] 模組配置

您設定 [!UICONTROL 迭代器] 模組與您設定任何其他模組的模組相同。 此 [!UICONTROL 陣列] 欄位包含要轉換或分割為個別套件的陣列。

![](assets/set-up-iterator-350x190.jpg)

如需詳細資訊，請參閱 [在Adobe Workfront Fusion中配置模組的設定](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**範例:**
>
>* 以下案例顯示如何檢索包含附件的電子郵件，以及將附件另存為選定檔案中的單個檔案 [!DNL Dropbox] 檔案夾。
   >
   >   電子郵件可包含一系列附件。 此 [!UICONTROL 迭代器] 插入在第一個模組之後的模組將允許您單獨處理每個附件。 此 [!UICONTROL 迭代器] 模組會將附件陣列分割為單一套件組合。 然後，每個包含一個附件的套件會一次在選取的套件中儲存一個 [!DNL Dropbox] 檔案夾。 此 [!UICONTROL 迭代器] 模組設定如下所示：the [!UICONTROL 陣列] 欄位應包含 `Attachments` 陣列。
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* 為了方便，許多 [!DNL Workfront Fusion] 應用程式提供專業化 [!UICONTROL 迭代器] 模組，並簡化設定。 例如， [!UICONTROL 電子郵件] 應用程式包含特殊 [!UICONTROL 迭代器] 模組 [!UICONTROL 電子郵件] > [!UICONTROL 迭代附件] 會產生與一般 [!UICONTROL 迭代器] 模組。
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## 疑難排解：「對應」面板未顯示下方的可映射項目 [!UICONTROL 迭代器] 模組

當 [!UICONTROL 迭代器] 模組沒有有關陣列項的結構的資訊，在模組中的映射面板位於 [!UICONTROL 迭代器] 模組在下方只顯示2個項目 [!UICONTROL 迭代器] 模組：`Total number of bundles` 和 `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

這是因為每個模組都負責提供其輸出項目的相關資訊，以便這些項目能夠在後續模組的對應面板中正確顯示。 但是，某些模組可能無法提供這些資訊；例如， [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 或 [!UICONTROL Webhook] > [!UICONTROL 自訂Webhook] 缺少資料結構的模組。

解決方案是手動執行情境，讓模組了解其輸出的項目，以便向下列模組提供資訊。

例如，如果您有 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組（不含資料結構），如下所示：

![](assets/json-parse-json-350x285.png)

如果你把 [!UICONTROL 迭代器] 模組，您將無法將模組的輸出對應至 [!UICONTROL 迭代器] 模組：

![](assets/connect-iterator-module-350x146.png)

若要解決此問題，請在案例編輯器中手動啟動案例。 您可以在 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 用於防止流進一步進行的模組。 或者，您可以在 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組與選擇 **[!UICONTROL 僅運行此模組]** 從上下文菜單僅執行 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組。

當 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 執行時，它會了解它輸出的項目，並將此資訊提供給所有後續模組，包括迭代器模組。 迭代程式設定中的對應面板隨即顯示項目：

![](assets/mapping-panel-displays-items-350x131.png)

此外，在模組中的映射面板在 [!UICONTROL 迭代器] 模組會顯示陣列項目中包含的項目：

![](assets/items-contained-in-array-350x156.png)

如果您在模組的對應面板中看不到某些項目，請執行一次方案，以便所有模組都能了解其輸出的項目，並將此資訊提供給以下模組。
