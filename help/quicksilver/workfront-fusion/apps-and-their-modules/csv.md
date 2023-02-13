---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Adobe Workfront Fusion CSV模組可讓您建立CSV檔案，並從收到的文字值或檔案剖析CSV文字。
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

此 [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] 模組可讓您建立CSV檔案，並從收到的文字值或檔案剖析CSV文字。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 建立CSV]

此 [!UICONTROL 建立CSV] 匯總器可讓您從收到的文字值建立CSV文字。

如需匯總器的詳細資訊，請參閱 [中的匯總模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL源模組]</td>
        <td>選取您用來匯總所需欄位的模組。</td>
    </tr>
    <tr>
        <td>[!UICONTROL聚合欄位]</td>
        <td>從可用欄位清單中選取要匯總的欄位。</td>
    </tr>
    <tr>
        <td>[!UICONTROL在第一行中包含標題]</td>
        <td>選取此選項，將標題納入結果中。</td>
    </tr>
    <tr>
        <td>[!UICONTROL組依據]</td>
        <td>輸入要對結果進行分組的篩選器。 例如，輸入日期。</td>
    </tr>
    <tr>
        <td>[!UICONTROL在空聚合後停止處理]</td>
        <td>選取此選項，在沒有結果時停止方案。</td>
    </tr>
</table>

## [!UICONTROL 建立CSV（進階）]

此 [!UICONTROL 建立CSV（進階）] 匯總器可讓您從收到的文字值建立CSV文字。 它採用資料結構，定義產生的CSV檔案中的CSV欄。 定義欄後，欄會在CSV模組設定中顯示為欄位，且可在案例中對應至稍後的模組。

如需匯總器的詳細資訊，請參閱 [中的匯總模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td>選取您用來匯總所需欄位的應用程式模組。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料結構]</td> 
   <td> <p>選取資料結構，以您想要的方式匯總欄位。 定義資料結構後，您可以將項目對應至對應的欄位。</p> <p>如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">中的資料結構 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在第一行中包含標題] </td> 
   <td>選取此選項，將標題納入結果中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL組依據] </td> 
   <td>輸入要對結果進行分組的篩選器。 例如，輸入日期。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在空聚合後停止處理] </td> 
   <td>選取此選項，在沒有結果時停止方案。 </td> 
  </tr> 
 </tbody> 
</table>


<p>假設您要將Google連絡人匯出為CSV檔案，其中包含「全名」和「電子郵件」兩欄。 來自[!UICONTROL Google Contacts] &gt;[!UICONTROL從組獲取聯繫人]模組的輸出套件具有以下結構。 電子郵件地址會儲存在 <code>[!UICONTROL Emails[]]</code> 項目，即集合的陣列，每個集合包含兩個項目： <code>Label</code> 和 <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>如果你用 [!DNL Create CSV] 模組中，會提供與套件頂層項目對應的核取方塊清單。 如果您嘗試勾選 <code>Full name</code> 和 <code>Emails</code> 項目，則[!UICONTROL建立CSV]模組會產生下列輸出，而這可能不是您想要的：</p>
<p>"emails","fullName"</p>
<p>"[object]","Shon Winer"</p>
<p>"[object]","Lizeth Fulmore"</p>
<p>"[object]","Hilario Gullatt"</p>
<p>"[對象]","Abby Eisenbarth"</p>
<p>由於項目 <code>Full Name</code> 是簡單類型的Text，則匯出後即可。 但是這個 <code>Emails</code>，屬於複雜類型集合陣列，會匯出為[object Object]，這是預設情況下集合和陣列轉換為文字的方式。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的項目資料類型</a>.</p>
<p>若要匯出 <code>Email </code>第一個集合的項目 <code>Emails[]</code> 陣列，則必須採用[!UICONTROL建立CSV（進階）]模組。 模組可讓您定義CSV檔案的個別欄，並將項目對應至這些欄，包括巢狀欄。</p>
<ol>
<li value="1">在案例中插入模組[!UICONTROL Create CSV(advanced)]並開啟其設定。</li>
<li value="2">按一下 <strong>[!UICONTROL添加]</strong> 按鈕（位於[!UICONTROL資料結構]欄位旁）以建立新資料結構。</li>
<li value="3"> <p>寫入資料結構的名稱，然後按一下 <strong>[!UICONTROL添加項]</strong> 按鈕以新增個別欄。 如果要匯出兩欄：「全名」和「電子郵件」，產生的資料結構如下所示：</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>成功定義資料結構後，每個欄對應的欄位應會顯示在[!UICONTROL建立CSV（進階）]模組的設定中，以便您對應項目。 取用 <code>[!UICONTROL Emails[]]</code> 陣列和映射其項目 <code>Email </code>至欄位/欄電子郵件：</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>執行情境。 由於項目 <code>Emails[1]: Email</code> 對應至「電子郵件」欄是簡單類型「文字」，現在可正確匯出：</p> <p>"全名"、"電子郵件"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL 剖析CSV]

此 [!UICONTROL 剖析CSV] 「轉換器」可讓您從收到的文字值或檔案中剖析CSV文字。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL列數]</td> 
   <td>指定CSV檔案中的欄數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV包含標題]</td> 
   <td> <p>如果CSV文字的第一列包含標題，請選取此選項。</p> <p>注意：模組不會使用這些標題來標籤輸出中的欄。 相反地，此欄位可確保輸出資料中不包含標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>選取CSV檔案的分隔字元。 分隔字元是指出個別值或欄位之間界限的文字字元。</p> 
    <ul> 
     <li>[!UICONTROL逗號]</li> 
     <li>[!UICONTROL頁簽]</li> 
     <li> <p>[!UICONTROL其他]</p> <p>如果選擇[!UICONTROL其他]，請輸入CSV檔案用於分隔值的分隔字元。 您必須只輸入一個字元。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在無引號欄位內保留引號]</td> 
   <td>啟用此選項可保留引號。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>輸入或對應您要剖析的CSV檔案。<p>備註: <p>如果您的資料是二進位格式（通常來自檔案），則必須使用'toString()'函式將二進位資料轉換為[!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
