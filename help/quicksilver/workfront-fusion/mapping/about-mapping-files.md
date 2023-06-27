---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 關於對應檔案於 [!DNL Adobe Workfront Fusion]
description: 有些模組具有處理檔案的功能。 這些模組可以傳回要傳送以供進一步處理的輸出檔案，或要求將檔案傳遞給它們以供處理。 這些模組必須彼此對應，才能共同處理檔案。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 關於對應檔案於 [!DNL Adobe Workfront Fusion]

有些模組具有處理檔案的功能。 這些模組可以傳回要傳送以供進一步處理的輸出檔案，或要求將檔案傳遞給它們以供處理。 這些模組必須彼此對應，才能共同處理檔案。

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
  </tr>  </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 對應檔案

能夠處理檔案的模組需要兩則資訊：

* 檔案名稱
* 檔案內容（資料）

對應檔案時，您可在情境中選擇要從中取得資料的模組。 然後會自動對應檔案名稱和檔案內容。

>[!NOTE]
>
>如果您需要處理URL中的檔案，我們建議使用 `HTTP > Get a File` 模組，可從URL下載檔案，然後將檔案從 `HTTP > Get a File` 模組至情境中所需模組的欄位。

>[!INFO]
>
>**範例：** 此範例說明如何從下載檔案 [!DNL Adobe Workfront] 至 [!DNL Google Drive]. 此 [!DNL Workfront] 觸發器 [!UICONTROL 觀看記錄] 傳回每個檔案的詳細資訊，包括其名稱和ID。
>
>下一個模組， [!UICONTROL 下載檔案]，下載實際資料，以便上傳至Google Drive。
>
>若要將此資訊對應至 [!DNL Google Drive] 為了能夠上傳，您需要指定將從中對應資訊的來源檔案。 如果您選取 [!DNL Workfront] > [!UICONTROL 下載檔案] 來源檔案下的選項 [!DNL Workfront Fusion] 對應檔案名稱和檔案內容，使檔案來自 [!DNL Workfront] 上傳至指定的Google資料夾。
>
>![](assets/wf-download-document-350x605.png)
>
>不過，如果您想要重新命名檔案，但保留資料不變，您可以使用 [!UICONTROL 地圖] 分別對應檔案名稱和檔案內容的選項。 您可以輸入完整的檔案名稱，包括副檔名。 支援文字格式和二進位格式，例如像片、影片和PDF。
>
>![](assets/use-the-map-option-350x358.png)
