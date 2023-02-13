---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 影像模組
description: Adobe Workfront Fusion Image模組允許您獲取有關特定影像（尺寸、類型等）的資訊、將影像轉換為其他檔案格式，並直接更改影像的大小。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# 影像模組

[!DNL Adobe Workfront Fusion] [!UICONTROL 影像] 模組可讓您取得特定影像（尺寸、類型等）的相關資訊、將影像轉換為其他檔案格式，以及直接變更影像的大小。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 影像] 模組及其欄位

設定此模組時，會顯示下列欄位。 模組中的粗體標題表示必填欄位。

* [[!UICONTROL 調整大小]](#resize)
* [[!UICONTROL 轉換格式]](#convert-a-format)
* [[!UICONTROL 擷取中繼資料]](#extract-metadata)

### [!UICONTROL 調整大小]

此變壓器模組會根據您指定的准則來變更影像的高度和寬度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>選擇要轉換的影像源。 您可以選取上一個模組的輸出，或對應資料檔案和檔案名稱。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料]</td> 
   <td>映射要轉換的檔案。 如果您在[!UICONTROL源檔案]欄位中選擇了[!UICONTROL映射]，則此欄位可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>輸入轉換檔案的名稱。 如果您在[!UICONTROL源檔案]欄位中選擇了[!UICONTROL映射]，則此欄位可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL我想]</td> 
   <td>選擇是要保持高寬比，還是將尺寸更改為指定的高寬。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根據]</td> 
   <td> <p>選取要如何讓模組判斷影像的新大小。 如果您在「我想要」欄位中選取要維持高度寬度比，則會顯示此欄位。 根據此欄位中的選取項目，會顯示其他欄位。</p> 
    <ul> 
     <li> <p>[!UICONTROL最大寬度]</p> <p>將影像縮小為您指定的寬度。 高度會自動計算。</p> </li> 
     <li> <p>[!UICONTROL最大高度]</p> <p>將影像縮小到您指定的高度。 會自動計算寬度。</p> </li> 
     <li> <p>[!UICONTROL最大高度或寬度]</p> <p>縮小影像的高度和寬度不會超過您指定的值。 由於此選項會維持高寬比，因此其中一個尺寸可能小於指定尺寸。 例如，如果高度和寬度均指定為40,400x300影像會縮小為40x30。</p> </li> 
     <li> <p>[!UICONTROL最小寬度]</p> <p>將影像放大到您指定的寬度。 高度會自動計算。</p> </li> 
     <li> <p>[!UICONTROL最低高度]</p> <p>將影像放大到您指定的高度。 會自動計算寬度。</p> </li> 
     <li> <p>[!UICONTROL最低高度或寬度]</p> <p>放大影像的方式為其高度和寬度不小於指定的值。 由於此選項會維持高寬比，因此其中一個尺寸可能大於指定尺寸。 例如，如果高度和寬度均指定為300，則40x30影像將放大為400X300。</p> </li> 
     <li> <p>[!UICONTROL百分比]</p> <p>根據您指定的值以百分比變更影像大小。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL寬度]</td> 
   <td>以像素輸入或映射調整後影像的所需寬度。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL高度]</td> 
   <td>以像素輸入或映射調整後影像的所需高度。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 轉換格式]

該變壓器模組更改影像檔案的格式。 此模組相容以下格式：

* PNG
* JPG
* GIF
* BMP

源檔案和輸出必須採用以下格式之一。 例如， [!UICONTROL 影像] >[!UICONTROL 轉換格式] 模組可將PNG檔案轉換為BMP檔案，或將BMP轉換為JPG。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>選擇要轉換的影像源。 您可以選取上一個模組的輸出，或對應資料檔案和檔案名稱。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料]</td> 
   <td>映射要轉換的檔案。 如果您在[!UICONTROL源檔案]欄位中選擇了[!UICONTROL映射]，則此欄位可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>輸入轉換檔案的名稱。 如果您在[!UICONTROL源檔案]欄位中選擇了[!UICONTROL映射]，則此欄位可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出格式]</td> 
   <td>選擇要模組將源檔案轉換為的格式。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 擷取中繼資料]

該變壓器模組返回有關模組的基本資訊。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>選擇要轉換的影像源。 您可以選取上一個模組的輸出，或對應資料檔案和檔案名稱。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料]</td> 
   <td>映射要轉換的檔案。 如果您在[!UICONTROL源檔案]欄位中選擇了映射，則此欄位可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>輸入轉換檔案的名稱。 如果您在[!UICONTROL源檔案]欄位中選擇了映射，則此欄位可用。</td> 
  </tr> 
 </tbody> 
</table>

## 可能的問題

### 動作因錯誤而終止

有三種情況下，動作可能會因錯誤而終止：

* 收到的資料不是JPG/GIF/PNG/BMP格式
* 變更影像尺寸時已超出最大寬度/高度限制。 影像大小不得超過3840像素寬度和2160像素高
* 更改影像的尺寸或格式時已超出影像的最大允許大小。
