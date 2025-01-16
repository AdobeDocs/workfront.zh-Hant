---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 關於在 [!DNL Adobe Workfront Fusion]中對應檔案
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# 關於在[!DNL Adobe Workfront Fusion]中對應檔案

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [在模組之間對應檔案](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

有些模組有能力處理檔案。 這些模組可以傳回要傳送以供進一步處理的輸出檔案，或要求將檔案傳遞給它們以供處理。 這些模組必須彼此對應，才能共同處理檔案。

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
  </tr>  </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 對應檔案

能夠處理檔案的模組需要兩則資訊：

* 檔案名稱
* 檔案內容（資料）

對應檔案時，您可以選擇情境中要從中取得資料的模組。 然後檔案名稱和檔案內容會自動對應。

>[!NOTE]
>
>如果您需要處理來自URL的檔案，我們建議使用`HTTP > Get a File`模組從URL下載檔案，然後將檔案從`HTTP > Get a File`模組對應到您案例中所需模組的欄位。

>[!INFO]
>
>**範例：**&#x200B;此範例說明如何從[!DNL Adobe Workfront]下載檔案至[!DNL Google Drive]。 [!DNL Workfront]觸發器[!UICONTROL 觀看記錄]傳回每個檔案的詳細資訊，包括其名稱和ID。
>
>下一個模組[!UICONTROL 下載檔案]會下載實際資料，以便上傳至Google磁碟機。
>
>若要將此資訊對應至[!DNL Google Drive]以便上傳，您必須指定將從中對應資訊的來源檔案。 如果您選取來源檔案下的[!DNL Workfront] > [!UICONTROL 下載檔案]選項，[!DNL Workfront Fusion]會對映檔案名稱和檔案內容，以便將[!DNL Workfront]中的檔案上傳到指定的Google資料夾。
>
>![](assets/wf-download-document-350x605.png)
>
>但是，如果您想要重新命名檔案，但保留資料不變，則可以使用[!UICONTROL 對應]選項來分別對應檔案名稱和檔案內容。 您可以輸入完整的檔案名稱，包括副檔名。 支援文字格式和二進位格式，例如像片、影片和PDF。
>
>![](assets/use-the-map-option-350x358.png)
