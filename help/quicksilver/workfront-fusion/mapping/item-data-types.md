---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 中的項目資料類型 [!DNL Adobe Workfront Fusion]
description: 您的 [!DNL Adobe Workfront Fusion] 方案可以包含套件中下列項目的類型。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 中的項目資料類型 [!DNL Adobe Workfront Fusion]

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
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 項目資料類型

您可以在套件中包含下列項目類型。

有關項目類型的資訊 [!DNL Workfront Fusion] 允許彼此轉換，請參閱 [中的強制類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>文字</p> </td> 
   <td> <p>最常見的項目類型。 對於某些文本項， [!DNL Adobe Workfront Fusion] 檢查是否滿足允許的最大長度或最小長度，或項目是否執行格式驗證（電子郵件、URL或檔案名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>數量</p> </td> 
   <td> <p>對於某些數值項， [!DNL Workfront Fusion] 可驗證指定範圍的輸入（允許的最小值或最大值）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>布林值（是/否）</p> </td> 
   <td> <p>此類型適用於只有兩個可能值的項目：true或false。 </p> <p>設定模組時，布林值類型可以以兩種不同的形式出現：</p> 
    <ul> 
     <li> <p>如果欄位為必填欄位且必須填入，則會顯示強制核取方塊。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>可留空的可選欄位會顯示為選取方塊，以允許在三個值中選取： <code>Yes</code>, <code>No</code>，和 <code>Not defined</code> （預設）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>您可以按一下 <strong>[!UICONTROL地圖]</strong> 如果您需要將值對應至其他模組中的項目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日期</p> </td> 
   <td> <p>日期以ISO 8601日期格式輸入，例如 <code>2015-09-18T11:58Z</code>. 您可以變更設定檔設定中的時區，如 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>. </p> <p>如果按一下需要日期的欄位，模組設定中會顯示快顯日曆。 某些項目不需要時間。</p> <p>日期項目的值會使用設定檔中選取的本機和網頁時區來格式化。 您可以將滑鼠暫留在項目上，以顯示日期項目值的ISO 8601版本。</p> <p>注意：如果未顯示ISO值，則項目可能是文字，而非日期。</p> <p>在 <code>hours:minutes:seconds</code> 格式，例如<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>緩衝（二進位資料）</p> </td> 
   <td> <p>檔案內容通常會以緩衝類型內容（影像內容、視訊檔案等）的形式傳送。 在某些情況下，文字資料會包含在此類型中（例如，文字檔案）。 [!DNL Workfront Fusion] 能夠自動將二進位代碼中的文本資料轉換為二進位代碼中的文本和文本資料。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">關於[!UICONTROL Adobe Workfront Fusion]中的對應檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>集合</p> </td> 
   <td> <p>集合是由多個子項組成的項目。 電子郵件中的寄件者項目是集合的範例：它包含寄件者名稱（文字類型）和寄件者電子郵件地址（文字類型）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>選擇（菜單）</p> </td> 
   <td> <p>如下所述配置模組設定時： <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>，您可以從數個相同類型的項目中選取。 例如， [!DNL Dropbox] 模組。 </p> <p>設定模組時，選取功能表可以以兩種形式顯示：</p> <p> <p>如果可以進行多個選取，則會顯示多個包含核取方塊的項目。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>如果只能有一個選項，則會顯示下拉式功能表。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>如果您需要從其他模組對應項目，請使用 <strong>地圖</strong> 按鈕。 此按鈕會開啟一個文本欄位，而不是選擇菜單。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>陣列</p> </td> 
   <td> <p>您可以使用陣列類型來處理相同類型的數個值，包括集合。 例如， [!UICONTROL電子郵件]模組：它們會傳回一連串附件，而每個附件都包含名稱、內容、大小等。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">在中映射陣列 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>驗證</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 可能會對每種類型的項目執行驗證。 如果項目未通過驗證，則模組將因資料錯誤而停止處理。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">中的錯誤處理 [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
