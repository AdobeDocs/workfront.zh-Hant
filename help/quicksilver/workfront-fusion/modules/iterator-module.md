---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的疊代器模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的[!UICONTROL 迭代器]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [疊代器模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!UICONTROL Iterator]模組是一種特殊的模組，可將陣列轉換為一系列組合。 每個陣列專案都會以個別的套件組合輸出。

如需詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)和[在Adobe Workfront Fusion中對應陣列](../../workfront-fusion/mapping/map-an-array.md)。

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
   <td>您的組織必須購買Adobe Workfront Fusion以及Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL 迭代器]模組組態

您設定的[!UICONTROL 疊代器]模組，與設定任何其他模組相同。 [!UICONTROL 陣列]欄位包含要轉換或分割為個別套裝的陣列。

![](assets/set-up-iterator-350x190.jpg)

如需詳細資訊，請參閱[在Adobe Workfront Fusion中設定模組的設定](../../workfront-fusion/modules/configure-a-modules-settings.md)。

>[!INFO]
>
>**範例：**
>
>* 以下案例顯示如何擷取含有附件的電子郵件，並將附件儲存為所選[!DNL Dropbox]資料夾中的單一檔案。
>
>   電子郵件可以包含一系列附件。 第一個模組之後插入的[!UICONTROL 疊代器]模組可讓您分別處理每個附件。 [!UICONTROL 迭代器]模組將附件陣列分割成單一組合。 然後，會將每個附有一個附件的套件一次儲存在選取的[!DNL Dropbox]資料夾中。 [!UICONTROL Iterator]模組設定如上所示： [!UICONTROL 陣列]欄位應該包含`Attachments`陣列。
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* 為方便起見，許多[!DNL Workfront Fusion]應用程式以簡化的設定，提供專門的[!UICONTROL 迭代器]模組。 例如，[!UICONTROL 電子郵件]應用程式包含特殊的[!UICONTROL 迭代器]模組[!UICONTROL 電子郵件] > [!UICONTROL 迭代附件]，將產生與一般[!UICONTROL 迭代器]模組相同的結果。
>
>   ![](assets/specialized-iterators-350x135.jpg)


## 疑難排解：對應面板不會在[!UICONTROL 迭代器]模組下顯示可對應專案

當[!UICONTROL 疊代器]模組沒有陣列專案的結構資訊時，[!UICONTROL 疊代器]模組之後的模組中的對應面板只會顯示[!UICONTROL 疊代器]模組下的2個專案：`Total number of bundles`和`Bundle order position`：

![](assets/mapping-panel-doesnt-display-350x147.png)

這是因為每個模組都負責提供其輸出專案的相關資訊，以便這些專案能在後續模組的對應面板中正確顯示。 但是，在某些情況下，數個模組可能無法提供此資訊；例如，[!UICONTROL JSON] > [!UICONTROL 剖析JSON]或[!UICONTROL Webhook] > [!UICONTROL 自訂Webhook]模組缺少資料結構。

解決方案是手動執行情境，讓模組瞭解其輸出的專案，以便提供資訊給下列模組。

例如，如果您有不具資料結構的[!UICONTROL JSON] > [!UICONTROL 剖析JSON]模組，如下所示：

![](assets/json-parse-json-350x285.png)

接著，如果您將[!UICONTROL 疊代器]模組連線至該模組，則無法將模組的輸出對應至[!UICONTROL 疊代器]模組的設定面板中的Array欄位：

![](assets/connect-iterator-module-350x146.png)

若要解決此問題，請在情境編輯器中手動啟動情境。 您可以在[!UICONTROL JSON] > [!UICONTROL 剖析JSON]模組之後取消連結模組，以防止流程繼續進行。 或者，您可以用滑鼠右鍵按一下[!UICONTROL JSON] > [!UICONTROL 剖析JSON]模組，然後從內容功能表中選擇&#x200B;**[!UICONTROL 僅執行此模組]**&#x200B;以僅執行[!UICONTROL JSON] > [!UICONTROL 剖析JSON]模組。

當[!UICONTROL JSON] > [!UICONTROL 剖析JSON]執行時，它會學習它輸出的專案，並將此資訊提供給所有後續模組，包括疊代器模組。 接著迭代器設定中的對應面板會顯示專案：

![](assets/mapping-panel-displays-items-350x131.png)

此外，在[!UICONTROL 疊代器]模組之後連線的模組中的對應面板會顯示陣列專案中包含的專案：

![](assets/items-contained-in-array-350x156.png)

如果您在模組的對應面板中看不到某些專案，請執行一次情境，讓所有模組都可以瞭解其輸出的專案，並將此資訊提供給下列模組。
