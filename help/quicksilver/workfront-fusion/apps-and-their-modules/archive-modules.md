---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 封存模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將歸檔（如壓縮檔案）連接到多個第三方應用程式和服務。 例如，您可以設定案例，
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL 封存] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以在案例中使用封存（例如壓縮檔），讓您在自動化或整合中使用。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL 封存] 模組及其欄位

設定時 [!UICONTROL 封存] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!UICONTROL 封存] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 解壓縮封存]](#extract-an-archive)
* [[!UICONTROL 建立封存]](#create-an-archive)
* [[!UICONTROL 膨脹]](#inflate)
* [[!UICONTROL 平減]](#deflate)

## [!UICONTROL 解壓縮封存]

此動作模組會從封存中擷取您所識別的檔案。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td> <p> 選取要擷取的檔案。 此檔案可從先前的模組(例如 [!DNL Workfront] &gt;[!UICONTROL下載文檔]模組)。</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 從定義的 [!DNL Dropbox] 資料夾（例如封存），請使用擷取 [!UICONTROL 封存] 模組，並將擷取的檔案連同 [!UICONTROL 電子郵件] 或 [!DNL Gmail] 模組。
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL 建立封存]

此聚合器模組將所需檔案添加到 [!UICONTROL ZIP] 或 [!UICONTROL TAR] 封存。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源模組]</td> 
   <td> <p> 選取要從中擷取檔案的模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL類型] </td> 
   <td> <p>選擇要將檔案添加到[!UICONTROL ZIP]存檔或[!UICONTROL TAR]存檔。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注釋]</td> 
   <td>輸入要添加到存檔的注釋。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL組依據]</td> 
   <td> <p>定義要將匯總輸出分組的表達式。 此運算式可包含一或多個已對應項目。 然後，使用此運算式的值，將匯總的資料分組。 每個群組會以獨立套件的形式輸出，其中包含鍵值（評估的運算式）和值（匯總文字）。 您可以在後續模組中將索引鍵當作篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在空聚合後停止處理]</td> 
   <td>選取此選項，在沒有結果時停止方案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL存檔名]</td> 
   <td> <p> 輸入已建立存檔的名稱。 請勿新增擴充功能。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 使用 [!DNL Gmail] >[!UICONTROL 觀看電子郵件] 模組。 如果收到電子郵件，其附件會迭代到個別套件組合中，然後封存到 [!DNL ZIP] 檔案並儲存至定義的Dropbox資料夾。
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 膨脹]

該變壓器模組使用膨脹算法對二進位資料進行解壓縮。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料] </td> 
   <td> <p>使用膨脹函式輸入或映射要解壓縮的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 平減]

該變壓器模組使用放氣算法壓縮二進位資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料] </td> 
   <td> <p>使用平減函式輸入或映射要壓縮的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>
