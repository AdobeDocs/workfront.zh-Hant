---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 中的專案資料型別 [!DNL Adobe Workfront Fusion]
description: 您的 [!DNL Adobe Workfront Fusion] 案例可以包含套件組合中下列專案的型別。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 中的專案資料型別 [!DNL Adobe Workfront Fusion]

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
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 專案資料型別

您可以在組合中包含下列專案型別。

有關哪些專案型別的資訊 [!DNL Workfront Fusion] 允許彼此之間的轉換，請參閱 [輸入強制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>文字</p> </td> 
   <td> <p>最常見的專案型別。 對於某些文字專案， [!DNL Adobe Workfront Fusion] 檢查是否符合允許的最大或最小長度，或專案是否執行格式驗證（電子郵件、URL或檔案名稱）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>數量</p> </td> 
   <td> <p>對於某些數值專案， [!DNL Workfront Fusion] 可驗證指定範圍（允許的最小值或最大值）的輸入。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>布林值（是/否）</p> </td> 
   <td> <p>此型別僅用於具有兩個可能值的專案：true或false。 </p> <p>設定模組時，布林值型別可能會以兩種不同的形式出現：</p> 
    <ul> 
     <li> <p>如果欄位為必填欄位且必須填寫，則會顯示必填核取方塊。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>可留空的可選欄位會顯示為選取方塊，以便在三個值中進行選取： <code>Yes</code>， <code>No</code>、和 <code>Not defined</code> （預設）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>您可以按一下 <strong>[！UICONTROL Map]</strong> 如果您需要將值對應至另一個模組的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日期</p> </td> 
   <td> <p>日期以ISO 8601日期格式輸入，例如， <code>2015-09-18T11:58Z</code>. 您可以在設定檔設定中變更時區，如中所述 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">變更中的設定檔設定 [!DNL Adobe Workfront Fusion]</a>. </p> <p>如果您按一下需要日期的欄位，模組設定中會顯示快顯行事曆。 某些專案不需要時間。</p> <p>日期專案的值會使用您在設定檔中選取的本機與網頁時區來格式化。 您可以將滑鼠懸停在專案上，以顯示日期專案值的ISO 8601版本。</p> <p>注意：如果ISO值未顯示，則專案可能是文字，而不是日期。</p> <p>時間輸入於 <code>hours:minutes:seconds</code> 格式，例如，<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>緩衝區（二進位資料）</p> </td> 
   <td> <p>檔案內容通常會以緩衝型別內容（影像內容、視訊檔案等）傳送。 在某些情況下，文字資料會包含在此型別中（例如文字檔）。 [!DNL Workfront Fusion] 能夠自動將二進位程式碼中的文字資料轉換為文字，並將文字轉換為二進位程式碼中的文字資料。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">關於[！UICONTROL Adobe Workfront Fusion]中的對應檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>集合</p> </td> 
   <td> <p>集合是由多個子專案組成的專案。 電子郵件訊息中的寄件者專案是集合的範例：它包含寄件者名稱（文字型別）和寄件者電子郵件地址（文字型別）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>選取（功能表）</p> </td> 
   <td> <p>當您依照中所述配置模組設定時 <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">在中設定模組的設定 [!DNL Adobe Workfront Fusion]</a>，您可以從相同型別的多個專案中選取。 例如，設定中的資料夾選取功能表 [!DNL Dropbox] 模組。 </p> <p>設定模組時，選取功能表可以兩種形式出現：</p> <p> <p>如果可以選取多個專案，則會顯示數個包含核取方塊的專案。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>如果只有一個選項，下拉式功能表就會顯示。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>如果您需要從另一個模組對應專案，請使用 <strong>地圖</strong> 按鈕。 此按鈕會開啟文字欄位，而不是選取功能表。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>陣列</p> </td> 
   <td> <p>您可以使用陣列型別來處理相同型別的多個值，包括集合。 [！UICONTROL Email]模組就是一個範例：這類模組會傳回一系列附件，而每個附件都包含名稱、內容、大小等。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">將陣列對應 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>驗證</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 可能會對每種型別的專案執行驗證。 如果專案未通過驗證，模組會因為資料錯誤而停止處理。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">中的處理錯誤 [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
