---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 封存模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將封存（例如壓縮檔案）連線至多個協力廠商應用程式和服務。 例如，您可以設定一個情境
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL 封存]模組

在[!DNL Adobe Workfront Fusion]情境中，您可以在情境中使用封存（例如壓縮檔案），讓您將其用於自動化或整合。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。 如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## [!UICONTROL 封存]模組及其欄位

當您設定[!UICONTROL 封存]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位之外，可能還會顯示其他[!UICONTROL 封存]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 擷取封存]](#extract-an-archive)
* [[!UICONTROL 建立封存]](#create-an-archive)
* [[!UICONTROL 膨脹]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL 擷取封存]

此動作模組會從封存中擷取您識別的檔案。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td> <p> 選取您要擷取的檔案。 此檔案可從先前的模組（例如[!DNL Workfront] &gt;[！UICONTROL下載檔案]模組）對應。</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**&#x200B;從定義的[!DNL Dropbox]資料夾中取得ZIP檔案（例如「封存」），使用[!UICONTROL 封存]模組擷取檔案，並將擷取的檔案以[!UICONTROL 電子郵件]或[!DNL Gmail]模組的附件形式傳送至所需的電子郵件地址。
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL 建立封存]

此彙總模組將所需的檔案新增至[!UICONTROL ZIP]或[!UICONTROL TAR]封存。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Source模組]</td> 
   <td> <p> 選取您要從中擷取檔案的模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL型別] </td> 
   <td> <p>選擇您要將檔案新增到[！UICONTROL ZIP]封存還是[！UICONTROL TAR]封存。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL註解]</td> 
   <td>輸入要新增到封存的註解。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Group by]</td> 
   <td> <p>定義要將彙總輸出分組依據的運算式。 此運算式可包含一或多個對應專案。 接著，彙總的資料會使用此運算式的值分隔成群組。 每個群組會輸出一個單獨的組合，內含索引鍵（運算式）和值（彙總文字）。 您可以在後續模組中使用該索引鍵作為篩選條件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL在空白彙總後停止處理]</td> 
   <td>選取此選項可在沒有結果時停止情境。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL封存名稱]</td> 
   <td> <p> 輸入已建立封存檔的名稱。 請勿新增副檔名。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**&#x200B;使用[!DNL Gmail] >[!UICONTROL 觀看電子郵件]模組觀看傳入電子郵件。 如果收到電子郵件，其附件會疊代為個別套件組合，然後封存至[!DNL ZIP]檔案並儲存至定義的Dropbox資料夾。
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 膨脹]

此轉換器模組會使用膨脹演演算法來解壓縮二進位資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料] </td> 
   <td> <p>使用膨脹函式，輸入或對應您要解壓縮的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflate]

此轉換器模組使用壓縮演演算法壓縮二進位資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料] </td> 
   <td> <p>使用deflate函式輸入或對應您要壓縮的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>
