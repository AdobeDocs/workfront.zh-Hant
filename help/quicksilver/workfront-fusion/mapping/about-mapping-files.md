---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 關於在 [!DNL Adobe Workfront Fusion]
description: 有些模組可處理檔案。 這些模組可以返回要發送以供進一步處理的輸出檔案，或者要求將檔案傳遞給它們進行處理。 在這些模組可以一起處理檔案之前，它們必須相互映射。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 關於在 [!DNL Adobe Workfront Fusion]

有些模組可處理檔案。 這些模組可以返回要發送以供進一步處理的輸出檔案，或者要求將檔案傳遞給它們進行處理。 在這些模組可以一起處理檔案之前，它們必須相互映射。

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
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr>  </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 映射檔案

能夠處理檔案的模組需要兩個資訊：

* 檔案名
* 檔案內容（資料）

映射檔案時，在方案中選擇要從中獲取資料的模組。 然後，檔案名稱和檔案內容會依原樣自動對應。

>[!NOTE]
>
>若您需要從URL處理檔案，建議您使用 `HTTP > Get a File` 模組，從URL下載檔案，然後從 `HTTP > Get a File` 模組至您案例中所需模組的欄位。

>[!INFO]
>
>**範例：** 此範例說明如何從 [!DNL Adobe Workfront] to [!DNL Google Drive]. 此 [!DNL Workfront] 觸發 [!UICONTROL 監視記錄] 返回有關每個文檔的詳細資訊，包括其名稱和ID。
>
>下一個模組， [!UICONTROL 下載檔案]，會下載實際資料，以便上傳至Google Drive。
>
>將此資訊對應至 [!DNL Google Drive] 因此，您需要指定要從中映射資訊的源檔案，才能將其上載。 如果您選取 [!DNL Workfront] > [!UICONTROL 下載檔案] 選項， [!DNL Workfront Fusion] 映射檔案名和檔案內容，以便 [!DNL Workfront] 上傳至指定的Google資料夾。
>
>![](assets/wf-download-document-350x605.png)
>
>不過，如果您想重新命名檔案，但保留資料原樣，則可使用 [!UICONTROL 地圖] 選項，分別映射檔案名和檔案內容。 您可以輸入完整的檔案名稱，包括副檔名。 支援文字格式和二進位格式，例如像片、視訊和PDF。
>
>![](assets/use-the-map-option-350x358.png)
