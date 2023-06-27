---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的疊代器模組
description: 疊代器模組是一種特殊型別的模組，可將陣列轉換為一系列組合。 每個陣列專案都會以個別的套件組合輸出。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL 迭代器] 中的模組 [!DNL Adobe Workfront Fusion]

一個 [!UICONTROL 迭代器] 模組是一種特殊型別的模組，可將陣列轉換為一系列組合。 每個陣列專案都會以個別的套件組合輸出。

如需詳細資訊，請參閱 [模組型別](../../workfront-fusion/modules/module-types.md) 和 [在Adobe Workfront Fusion中對應陣列](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>您的組織必須購買Adobe Workfront Fusion和Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 迭代器] 模組設定

您設定 [!UICONTROL 迭代器] 模組，與您設定任何其他模組相同。 此 [!UICONTROL 陣列] 欄位包含要轉換或分割為個別套裝的陣列。

![](assets/set-up-iterator-350x190.jpg)

如需詳細資訊，請參閱 [在Adobe Workfront Fusion中設定模組的設定](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**範例:**
>
>* 以下案例顯示如何擷取含有附件的電子郵件，並將附件儲存為所選檔案中的單一檔案 [!DNL Dropbox] 資料夾。
>
>   電子郵件可以包含一系列附件。 此 [!UICONTROL 迭代器] 第一個模組之後插入的模組可讓您分別處理每個附件。 此 [!UICONTROL 迭代器] 模組會將附件陣列分割成單一組合。 然後，會將每個具有一個附件的套件組合一次儲存在選取的套件組合中 [!DNL Dropbox] 資料夾。 此 [!UICONTROL 迭代器] 模組設定如上所示： [!UICONTROL 陣列] 欄位應包含 `Attachments` 陣列。
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* 為了您的方便，您可以 [!DNL Workfront Fusion] 應用程式提供專門的 [!UICONTROL 迭代器] 簡化設定的模組。 例如， [!UICONTROL 電子郵件] 應用程式包含特殊的 [!UICONTROL 迭代器] 模組 [!UICONTROL 電子郵件] > [!UICONTROL 迭代附件] 將產生與一般相同的結果 [!UICONTROL 迭代器] 模組。
>
>   ![](assets/specialized-iterators-350x135.jpg)


## 疑難排解：對應面板不會在 [!UICONTROL 迭代器] 模組

當 [!UICONTROL 迭代器] 模組沒有陣列專案結構的相關資訊，模組後面的對應面板如下 [!UICONTROL 迭代器] 模組只會顯示2個專案 [!UICONTROL 迭代器] 模組：`Total number of bundles` 和 `Bundle order position`：

![](assets/mapping-panel-doesnt-display-350x147.png)

這是因為每個模組都負責提供其輸出專案的相關資訊，以便這些專案能在後續模組的對應面板中正確顯示。 但是，在某些情況下，某些模組可能無法提供此資訊；例如， [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 或 [!UICONTROL Webhook] > [!UICONTROL 自訂Webhook] 遺失資料結構的模組。

解決方案是手動執行情境，讓模組瞭解其輸出的專案，以便能夠為以下模組提供資訊。

例如，如果您的 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 沒有資料結構的模組，如下所示：

![](assets/json-parse-json-350x285.png)

如果您將 [!UICONTROL 迭代器] 將模組對應至該模組，您將無法將模組的輸出對應至的設定面板中的陣列欄位。 [!UICONTROL 迭代器] 模組：

![](assets/connect-iterator-module-350x146.png)

若要解決此問題，請在情境編輯器中手動啟動情境。 之後您可以取消連結模組 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組，以防止流程繼續進行。 或者，您可以用滑鼠右鍵按一下 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組並選擇 **[!UICONTROL 僅執行此模組]** 從快顯選單中僅執行 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 模組。

當 [!UICONTROL JSON] > [!UICONTROL 剖析JSON] 執行時，它會學習它輸出的專案，並將此資訊提供給所有後續模組，包括疊代器模組。 疊代器設定中的對應面板接著會顯示專案：

![](assets/mapping-panel-displays-items-350x131.png)

此外，在之後連線的模組中的對應面板 [!UICONTROL 迭代器] 模組會顯示陣列專案中包含的專案：

![](assets/items-contained-in-array-350x156.png)

如果您在模組的對應面板中看不到某些專案，請執行此案例一次，讓所有模組都可以瞭解它們輸出的專案，並將此資訊提供給下列模組。
