---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: ServiceNow模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用 [!DNL ServiceNow]的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 0%

---

# [!DNL ServiceNow]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL ServiceNow]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL ServiceNow]模組，您必須有[!DNL ServiceNow]帳戶。

## ServiceNow API資訊

ServiceNow聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>https://{{connection.instance}}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.5.13</td> 
  </tr>
 </tbody> 
 </table>

## 將[!DNL ServiceNow]連線至[!DNL Workfront Fusion]

若要為您的[!DNL ServiceNow]模組建立連線：

1. 當您開始設定第一個[!DNL ServiceNow]模組時，請按一下[!UICONTROL 連線]方塊旁的&#x200B;**[!UICONTROL 新增]**。
1. 輸入下列內容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td>輸入新[!DNL ServiceNow]連線的名稱</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL使用者名稱]</p> </td> 
      <td>輸入您的[!DNL ServiceNow]使用者名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL密碼]</p> </td> 
      <td>輸入您的ServiceNow密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL執行個體]</p> </td> 
      <td> <p>輸入沒有<code>https://</code>的[!DNL ServiceNow]帳戶位址（通常是<code>&lt;company>.service-now.com</code>）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow]模組及其欄位

當您設定[!DNL ServiceNow]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL ServiceNow]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>如果在&quot;[!UICONTROL 記錄型別]&quot;欄位中選取自訂記錄，則載入自訂欄位可能需要一些時間。
>
>如果沒有自訂記錄，下拉式清單將是空的。

* [[!UICONTROL 觀看記錄]](#watch-records)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 停用使用者]](#deactivate-a-user)
* [[!UICONTROL 下載附件]](#download-an-attachment)
* [[!UICONTROL 上傳附件]](#upload-an-attachment)
* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 搜尋記錄]](#search-for-records)

### [!UICONTROL 觀看記錄]

建立或更新記錄時，此觸發模組會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表型別]</td> 
   <td>選取您要觀察的表格是自訂表格還是標準表格。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要觀看的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示]</td> 
   <td>選取您要顯示的值型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>選取您要監視新記錄或更新的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對[!DNL ServiceNow] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL ServiceNow]模組無法完成的資料流程自動化。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL相對URL]</td> 
   <td> <p>在網頁伺服器上輸入您希望模組與之互動的位址。</p> <p>您可以輸入相對URL，這表示您不必在開頭包含通訊協定（例如<code>http://</code>）。 這會向網頁伺服器提示互動正在伺服器上發生。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 讀取記錄]

此動作模組使用系統ID讀取[!DNL ServiceNow]記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄系統ID]</td> 
   <td>輸入或對應您要模組讀取之記錄的唯一[!DNL ServiceNow]識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表型別]</td> 
   <td>選取您要讀取的記錄是在自訂表格中還是在標準表格中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您希望模組讀取的[!DNL ServiceNow]記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示]</td> 
   <td>選取您要顯示的值型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 停用使用者]

此動作模組使用系統ID在[!DNL ServiceNow]中停用使用者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者系統識別碼]</td> 
   <td> 輸入或對應您要停用模組之使用者的唯一[!DNL ServiceNow]識別碼。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 下載附件]

此動作模組會下載[!DNL ServiceNow]記錄中的附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附件系統ID]</td> 
   <td> 輸入或對應您要模組下載之附件的唯一[!DNL ServiceNow]識別碼。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上傳附件]

此動作模組會將附件上傳至[!DNL ServiceNow]記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表名稱]</td> 
   <td>輸入或對應您要上傳附件的表格名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL系統ID]</td> 
   <td>輸入或對應您要上傳附件之系統的唯一[!DNL ServiceNow] ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td>輸入或對應附件的名稱</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案內容]</td> 
   <td>輸入或對應您要上傳的檔案至[!DNL ServiceNow]。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立記錄]

此動作模組會建立新的[!DNL ServiceNow]記錄。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表型別]</td> 
   <td>選取您要在自訂表格或標準表格中建立記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要模組建立的[!DNL ServiceNow]記錄型別。 然後，您可以填寫此記錄型別的可用欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會建立新的[!DNL ServiceNow]記錄。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄系統ID]</td> 
   <td>輸入或對應您要模組更新的記錄的唯一[!DNL ServiceNow]識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表型別]</td> 
   <td>選取要更新的記錄是在自訂表格中還是在標準表格中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您希望模組更新的[!DNL ServiceNow]記錄型別。 然後，您可以填寫此記錄型別的可用欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除事件或使用者。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要刪除事件或使用者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL系統ID]</td> 
   <td>輸入或對應您要模組刪除之記錄的唯一[!DNL ServiceNow]識別碼。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋記錄]

此模組會使用您選取的條件來搜尋記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將ServiceNow帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">將[!DNL ServiceNow]連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料表型別]</td> 
   <td>選取您要搜尋的表格是自訂表格還是標準表格。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要搜尋的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果集]</td> 
   <td>選取您希望模組傳回符合條件的所有記錄，還是隻傳回符合條件的第一筆記錄。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋型別]</td> 
   <td> <p>選取您希望模組執行的搜尋型別</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL進階查詢]</strong> </p> 
      <ul> 
       <li> <p>[！UICONTROL搜尋查詢]</p> <p>輸入自訂搜尋查詢。 如需[!DNL ServiceNow]自訂搜尋查詢的相關資訊，請參閱<a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow查詢檔案</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[！UICONTROL搜尋條件]</p> <p>輸入您希望模組搜尋的條件。 如需設定搜尋篩選的詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">將篩選新增至Adobe Workfront Fusion中的案例</a>。</p> </li> 
       <li> <p>[！UICONTROL排序依據]</p> <p>指出您希望模組排序結果的欄位，以及應依遞增或遞減排序。</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示]</td> 
   <td>選取您要顯示的值型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>
