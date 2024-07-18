---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Adobe Workfront Fusion CSV模組可讓您建立CSV檔案，以及從收到的文字值或檔案剖析CSV文字。
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---

# CSV

[!DNL Adobe Workfront Fusion] [!UICONTROL CSV]模組可讓您建立CSV檔案，並從收到的文字值或檔案剖析CSV文字。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## [!UICONTROL 建立CSV]

[!UICONTROL 建立CSV]彙總器可讓您從收到的文字值建立CSV文字。

如需彙總的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)中的[彙總模組。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL Source模組]</td>
        <td>選取您用來彙總所需欄位的模組。</td>
    </tr>
    <tr>
        <td>[！UICONTROL彙總欄位]</td>
        <td>從可用欄位清單中選取您要彙總的欄位。</td>
    </tr>
    <tr>
        <td>[！UICONTROL Include headers in the first row]</td>
        <td>選取此選項以在結果中包含標題。</td>
    </tr>
    <tr>
        <td>[！UICONTROL Group by]</td>
        <td>輸入篩選條件以將結果分組。 例如，輸入日期。</td>
    </tr>
    <tr>
        <td>[！UICONTROL在空白彙總後停止處理]</td>
        <td>選取此選項可在沒有結果時停止情境。</td>
    </tr>
</table>

## [!UICONTROL 建立CSV （進階）]

[!UICONTROL 建立CSV （進階）]彙總器可讓您從收到的文字值建立CSV文字。 它採用一種資料結構，定義所產生CSV檔案中的CSV欄。 定義後，欄會顯示為CSV模組設定中的欄位，並可對應至案例中稍後的模組。

如需彙總的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)中的[彙總模組。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td>選取您用來彙總所需欄位的應用程式模組。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料結構]</td> 
   <td> <p>選取資料結構，以您想要的方式彙總欄位。 定義資料結構後，您可以將專案對應至對應的欄位。</p> <p>如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">資料結構。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include headers in the first row] </td> 
   <td>選取此選項以在結果中包含標題。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Group by] </td> 
   <td>輸入篩選條件以將結果分組。 例如，輸入日期。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在空白彙總後停止處理] </td> 
   <td>選取此選項可在沒有結果時停止情境。 </td> 
  </tr> 
 </tbody> 
</table>


<p>假設您想要將Google聯絡人匯出至具有兩欄「全名」和「電子郵件」的CSV檔案。 [！UICONTROL Google Contacts] &gt;[！UICONTROL Get contacts from a group]模組的輸出套件組合具有以下結構。 電子郵件地址儲存在<code>[!UICONTROL Emails[]]</code>專案內，這是集合陣列，每個集合包含兩個專案： <code>Label</code>和<code>Email</code>。</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>如果您使用簡單[!DNL Create CSV]模組，則會提供對應至套件組合最上層專案的核取方塊清單。 如果您嘗試勾選<code>Full name</code>和<code>Emails</code>個專案，[！UICONTROL建立CSV]模組會產生以下輸出，可能不是您想要的：</p>
<p>"emails"，"fullName"</p>
<p>"[物件物件]"，"Shon Winer"</p>
<p>"[物件物件]"，"Lizeth Fulmore"</p>
<p>"[物件物件]"，"Hilario Gullatt"</p>
<p>"[物件物件]"，"Abby Eisenbarth"</p>
<p>由於專案<code>Full Name</code>屬於簡單型別Text，因此可以順利匯出。 但專案<code>Emails</code> （屬於複雜型別Array of Collections）會匯出為[object Object]，這是預設將Collections和Arrays轉換為文字的方式。 如需詳細資訊，請參閱<a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的專案資料型別</a>。</p>
<p>若要轉存<code>Emails[]</code>陣列之第一個集合的<code>Email </code>專案內容，必須採用[！UICONTROL建立CSV （進階）]模組。 此模組可讓您定義CSV檔案的個別欄，並將專案對應至這些欄，包括巢狀欄。</p>
<ol>
<li value="1">在情境中插入模組[！UICONTROL建立CSV （進階）]並開啟其設定。</li>
<li value="2">按一下[！UICONTROL資料結構]欄位旁的<strong>[！UICONTROL新增]</strong>按鈕，以建立新的資料結構。</li>
<li value="3"> <p>寫入資料結構的名稱，然後按一下<strong>[！UICONTROL新增專案]</strong>按鈕以新增個別欄。 如果您想要匯出兩欄：「全名」和「電子郵件」，則產生的「資料」結構會如下所示：</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>當您成功定義資料結構後，與每個個別欄對應的欄位應該會出現在[！UICONTROL建立CSV （進階）]模組的設定中，以便您對應專案。 從<code>[!UICONTROL Emails[]]</code>陣列取得第一個專案，並將其專案<code>Email </code>對應至欄位/欄電子郵件：</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>執行情境。 由於對應到欄「電子郵件」的專案<code>Emails[1]: Email</code>屬於簡單型別Text，因此它現在會正確匯出：</p> <p>"Full Name"，"Email"</p> <p>「Shon Winer」，「Shon@Winer.com」</p> <p>"Lizeth Fulmore"，"Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt"，"Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth"，"Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL 剖析CSV]

[!UICONTROL 剖析CSV]轉換器可讓您從收到的文字值或檔案剖析CSV文字。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄數]</td> 
   <td>指定CSV檔案中的欄數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL CSV包含標題]</td> 
   <td> <p>如果CSV文字的第一列包含標題，請選取此選項。</p> <p>注意：模組不會使用這些標頭來標示輸出中的欄。 相反，此欄位可確保輸出資料中不包含標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL delimiterType]</td> 
   <td> <p>選取CSV檔案的分隔符號。 分隔字元是指示個別值或欄位之間界限的文字字元。</p> 
    <ul> 
     <li>[！UICONTROL逗號]</li> 
     <li>[！UICONTROL索引標籤]</li> 
     <li> <p>[！UICONTROL其他]</p> <p>如果您選取[！UICONTROL其他]，請輸入CSV檔案用來分隔值的分隔字元。 您只能輸入一個字元。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL保留無引號欄位內的引號]</td> 
   <td>啟用此選項以保留引號。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL CSV]</td> 
   <td>輸入或對應您要剖析的CSV檔案。<p>注意： <p>如果您的資料為二進位格式（通常來自檔案），您必須使用'toString()'函式將二進位資料轉換為[！UICONTROL String]：</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
