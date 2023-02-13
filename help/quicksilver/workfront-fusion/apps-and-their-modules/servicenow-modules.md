---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: ServiceNow模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL ServiceNow]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# [!DNL ServiceNow] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL ServiceNow]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL ServiceNow] 模組，您必須 [!DNL ServiceNow] 帳戶。

## Connect [!DNL ServiceNow] to [!DNL Workfront Fusion]

為 [!DNL ServiceNow] 模組：

1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 框 [!DNL ServiceNow] 模組。
1. 輸入下列內容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL連接名]</p> </td> 
      <td>輸入新名稱 [!DNL ServiceNow] 連接</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL用戶名]</p> </td> 
      <td>輸入 [!DNL ServiceNow] 使用者名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL密碼]</p> </td> 
      <td>輸入ServiceNow密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL實例]</p> </td> 
      <td> <p>輸入 [!DNL ServiceNow] 帳戶無 <code>https://</code> (通常 <code>&lt;company>.service-now.com</code>)。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] 模組及其欄位

設定時 [!DNL ServiceNow] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL ServiceNow] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>如果在「[!UICONTROL 記錄類型]」欄位，載入自訂欄位可能需要一些時間。
>
>如果沒有自訂記錄，下拉式清單將會是空的。

* [[!UICONTROL 監看記錄]](#watch-records)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 停用使用者]](#deactivate-a-user)
* [[!UICONTROL 下載附件]](#download-an-attachment)
* [[!UICONTROL 上傳附件]](#upload-an-attachment)
* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 搜索記錄]](#search-for-records)

### [!UICONTROL 監看記錄]

建立或更新記錄時，此觸發模組會啟用案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表類型]</td> 
   <td>選擇要監視的表是自定義表還是標準表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇要監視的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示]</td> 
   <td>選取您要顯示的值類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td>選擇要監視新記錄還是更新記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL ServiceNow] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL ServiceNow] 模組。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL相對URL]</td> 
   <td> <p>在Web伺服器上輸入您要模組與之互動的地址。</p> <p>您可以輸入相對URL，這表示您不需要包含通訊協定(例如 <code>http://</code>)。 這向Web伺服器建議，正在伺服器上進行互動。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 讀取記錄]

此動作模組會讀取 [!DNL ServiceNow] 使用系統ID進行記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄系統ID]</td> 
   <td>輸入或對應唯一 [!DNL ServiceNow] 您要模組讀取的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表類型]</td> 
   <td>選擇要讀取的記錄是在自定義表還是標準表中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選取 [!DNL ServiceNow] 記錄您要模組讀取的內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示]</td> 
   <td>選取您要顯示的值類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 停用使用者]

此動作模組會停用使用者 [!DNL ServiceNow] 使用系統ID。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用戶系統ID]</td> 
   <td> 輸入或對應唯一 [!DNL ServiceNow] 您希望模組停用的使用者ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 下載附件]

此動作模組會下載 [!DNL ServiceNow] 記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附件系統ID]</td> 
   <td> 輸入或對應唯一 [!DNL ServiceNow] 您要模組下載的附件ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上傳附件]

此動作模組會將附件上傳至 [!DNL ServiceNow] 記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表名]</td> 
   <td>輸入或映射要上載附件的表的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系統ID]</td> 
   <td>輸入或對應唯一 [!DNL ServiceNow] 要上載附件的系統ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>輸入或映射附件的名稱</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案內容]</td> 
   <td>輸入或對應您要上傳的檔案 [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立記錄]

此動作模組會建立新 [!DNL ServiceNow] 記錄。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表類型]</td> 
   <td>選擇要在自定義表或標準表中建立記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選取 [!DNL ServiceNow] 記錄您要建立模組。 然後，您可以填寫此記錄類型的可用欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會建立新 [!DNL ServiceNow] 記錄。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄系統ID]</td> 
   <td>輸入或對應唯一 [!DNL ServiceNow] 要更新模組的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表類型]</td> 
   <td>選擇要更新的記錄是在自定義表還是標準表中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選取 [!DNL ServiceNow] 記錄您要更新模組。 然後，您可以填寫此記錄類型的可用欄位。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除事件或使用者。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇要刪除事件還是用戶。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系統ID]</td> 
   <td>輸入或對應唯一 [!DNL ServiceNow] 您要刪除模組的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索記錄]

此模組使用您選取的條件來搜尋記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將ServiceNow帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connect [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表類型]</td> 
   <td>選擇要搜索的表是自定義表還是標準表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇要搜索的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果集]</td> 
   <td>選擇是希望模組返回符合條件的所有記錄，還是僅返回第一個與其匹配的記錄。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄的最大計數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索類型]</td> 
   <td> <p>選擇要模組執行的搜索類型</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL高級查詢]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL搜索查詢]</p> <p>輸入自定義搜索查詢。 如需 [!DNL ServiceNow] 自訂搜尋查詢，請參閱 <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow查詢文檔</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL簡單]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL搜索條件]</p> <p>輸入要模組搜索的標準。 如需設定搜尋篩選器的詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">為Adobe Workfront Fusion中的案例新增篩選器</a>.</p> </li> 
       <li> <p>[!UICONTROL排序依據]</p> <p>指定您要模組依哪個欄位來排序結果，以及應以升序或降序排序結果。</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示]</td> 
   <td>選取您要顯示的值類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>
