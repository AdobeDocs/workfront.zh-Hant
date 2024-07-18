---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe Workfront Fusion]中的專案資料型別'
description: 您的 [!DNL Adobe Workfront Fusion] 案例可以包含套件組合中下列專案的型別。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的專案資料型別

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
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 專案資料型別

可在束中包含下列專案型別。

如需哪些型別的專案[!DNL Workfront Fusion]允許彼此之間轉換的資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md)中鍵入強制。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>文字</p> </td> 
   <td> <p>最常見的專案型別。 對於某些文字專案，[!DNL Adobe Workfront Fusion]會檢查是否符合允許的最大或最小長度，或專案是否執行格式驗證（電子郵件、URL或檔案名稱）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>數字</p> </td> 
   <td> <p>對於某些數值專案，[!DNL Workfront Fusion]可能會驗證指定範圍（最小或最大允許值）的輸入。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>布林值（是/否）</p> </td> 
   <td> <p>此型別用於只有兩個可能值的專案：true或false。 </p> <p>設定模組時，布林值型別可能會以兩種不同的形式出現：</p> 
    <ul> 
     <li> <p>如果欄位是必填欄位且必須填寫，則會顯示必填核取方塊。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>可保留空白的選用欄位會顯示為選取方塊，允許選取三個值： <code>Yes</code>、<code>No</code>和<code>Not defined</code> （預設）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>如果您需要將值對應到其他模組的專案，可以按一下<strong>[！UICONTROL Map]</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日期</p> </td> 
   <td> <p>日期是以ISO 8601日期格式輸入，例如<code>2015-09-18T11:58Z</code>。 您可以在設定檔設定中變更時區，如<a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中變更設定檔設定中所述。 </p> <p>如果您按一下需要日期的欄位，模組設定中會顯示快顯行事曆。 某些專案不需要時間。</p> <p>日期專案的值會使用您在設定檔中選取的當地和網頁時區來格式化。 您可以將滑鼠懸停在專案上，以顯示日期專案值的ISO 8601版本。</p> <p>注意：如果ISO值未顯示，則專案可能是文字，而不是日期。</p> <p>時間以<code>hours:minutes:seconds</code>格式輸入，例如<code>14:03:52</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>緩衝區（二進位資料）</p> </td> 
   <td> <p>檔案內容通常會以緩衝型別內容（影像內容、視訊檔案等）傳送。 在某些情況下，文字資料會包含在此型別中（例如文字檔）。 [!DNL Workfront Fusion]能夠自動將二進位程式碼中的文字資料轉換成文字，並將文字轉換成二進位程式碼中的文字資料。 如需詳細資訊，請參閱<a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">關於[！UICONTROL Adobe Workfront Fusion]</a>中的對應檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>集合</p> </td> 
   <td> <p>集合是由多個子專案組成的專案。 電子郵件訊息中的「寄件者」專案是集合的範例：它包含寄件者名稱（文字型別）和寄件者電子郵件地址（文字型別）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>選取（功能表）</p> </td> 
   <td> <p>當您依照<a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中設定模組的設定中所述設定模組設定時，您可以從相同型別的數個專案中選取。 例如，[!DNL Dropbox]模組設定中的資料夾選取功能表。 </p> <p>設定模組時，選取功能表可以兩種形式出現：</p> <p> <p>如果可以選取多個專案，則會顯示數個包含核取方塊的專案。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>如果只有一個選項可行，便會顯示下拉式功能表。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>如果您需要對應另一個模組的專案，請使用<strong>對應</strong>按鈕。 此按鈕會開啟文字欄位，而非選取功能表。 如需詳細資訊，請參閱<a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中將資訊從一個模組對應到另一個模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>陣列</p> </td> 
   <td> <p>您可以使用陣列型別來處理相同型別的多個值，包括集合。 [！UICONTROL Email]模組就是一個範例：它們會傳回一系列附件，而每個附件都包含名稱、內容、大小等。 如需詳細資訊，請參閱<a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中對應陣列。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>驗證</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 可能會對每種型別的專案執行驗證。 如果專案未通過驗證，則模組會因為資料錯誤而停止處理。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">錯誤處理。 </p> </td> 
  </tr> 
 </tbody> 
</table>
