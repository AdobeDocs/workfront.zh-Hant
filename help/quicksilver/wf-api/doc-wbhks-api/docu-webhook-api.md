---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文檔Webhook API
description: 文檔Webhook API
author: John
feature: Workfront API
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: a2f340122b22ccc57af1afffd82093e458219648
workflow-type: tm+mt
source-wordcount: '3661'
ht-degree: 3%

---


# 文檔Webhook API

Adobe Workfront Document Webhook定義了一組API端點，Workfront會透過此端點向外部檔案提供者發出授權API呼叫。 這可讓任何人為任何檔案儲存提供者建立中間件外掛程式。

網頁連結型整合的使用者體驗將類似於現有的檔案整合，例如Google Drive、Box和Dropbox。 例如，Workfront使用者將能執行下列動作：

* 導航外部文檔提供程式的資料夾結構
* 搜尋檔案
* 將檔案連結至Workfront
* 將檔案上傳到外部文檔提供程式
* 查看文檔的縮略圖

## 參考實作

為協助快速開發新Webhook實作，Workfront提供參考實作。 此項目的程式碼位於 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). 此實作以Java為基礎，可讓Workfront連線網路檔案系統上的檔案。

## 註冊Webhook整合

Workfront管理員可導覽至Workfront中的「設定>檔案>自訂整合」 ，為公司新增自訂網頁連結整合。 從「設定」的「自訂整合」頁面，管理員可以檢視現有檔案Webhook整合的清單。 您可以從本頁面新增、編輯、啟用和停用整合。 若要新增整合，請按一下「新增整合」按鈕。

### 可用欄位

新增整合時，管理員將輸入下列欄位的值：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>名稱</td> 
   <td>此整合的名稱。</td> 
  </tr> 
  <tr> 
   <td>基本 API URL</td> 
   <td> <p>回呼API的位置。 呼叫外部系統時，Workfront只會將端點名稱附加至此位址。 例如，如果管理員輸入了基本API URL " https://www.mycompany.com/api/v1 ",Workfront會使用下列URL來取得檔案的中繼資料：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>要求參數</td> 
   <td> <p>附加至每個 API 呼叫的 querystring 的選用值。例如，access_type</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>驗證類型</td> 
   <td>OAuth2或ApiKey</td> 
  </tr> 
  <tr> 
   <td>驗證 URL</td> 
   <td> <p>（僅限OAuth2）用於使用者驗證的完整URL。 Workfront會在OAuth布建程式中，將使用者導覽至此位址。 注意：Workfront會將「state」參數附加至查詢字串。 提供者必須將此檔案附加至Workfront重新導向URI，以將此檔案傳回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>權杖端點 URL</td> 
   <td> <p>（僅限OAuth2）用來擷取OAuth2代號的完整API URL。 這是由Webhook提供者或外部檔案提供者托管</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>用戶端 ID</td> 
   <td>（僅限OAuth2）此整合的OAuth2用戶端ID</td> 
  </tr> 
  <tr> 
   <td>用戶端密碼</td> 
   <td> <p>（僅限OAuth2）此整合的OAuth2用戶端密碼</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重新導向 URI</td> 
   <td>  <p>（僅限OAuth2）此為唯讀欄位，由Workfront產生。 此值可用來與外部檔案提供者註冊此整合。 注意：如上所述，驗證URL的提供者在執行重新導向時，必須將「state」參數及其值附加至查詢字串。</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>（僅限ApiKey）用於向Webhook提供者發出授權API呼叫。 由Webhook提供者發出的API金鑰。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 驗證

Workfront document webhook支援兩種不同的驗證形式：OAuth2和ApiKey。 在這兩種情況下，Workfront會在進行API呼叫時，在標題中傳遞驗證Token。

### OAuth2

OAuth2可讓Workfront代表使用者向網頁連結提供者發出授權API呼叫。 在執行此動作之前，使用者必須將其外部檔案提供者帳戶連線至Workfront，並授與Workfront

有權代表他們採取行動。 此握手過程僅對每個用戶進行一次。 其運作方式如下：

1. 使用者開始將Webhook整合連線至其帳戶。 目前，您可以按一下「新增檔案」下拉式清單>「新增服務」>「自訂整合名稱」來完成此作業。
1. Workfront會導覽使用者驗證URL，這可能會提示使用者登入外部檔案提供者。 此頁由Webhook提供程式或外部文檔管理系統托管。 這麼做時，Workfront會將「state」參數新增至驗證URL。 您必須在下列步驟中，將相同的值附加至Workfront傳回URI，以將此值傳回Workfront。
1. 登入外部系統後（或如果使用者已登入），會將使用者帶入「驗證」頁面，說明Workfront正在代表使用者要求存取以執行一組動作。
1. 如果使用者按一下「允許」按鈕，瀏覽器會重新導向至Workfront重新導向URI ，並新增「code=`<code>`&quot;到查詢字串。 根據OAuth2規格，此代號是短期的。 查詢字串也必須具備下列項目： &quot;state=`<sent_by_workfront>`」。
1. Workfront會處理此要求，並使用授權程式碼對Token端點URL進行API呼叫。
1. Token端點URL會傳回重新整理Token和存取Token。
1. Workfront會儲存這些代號，並為此使用者完全布建webhook整合。
1. 此後，Workfront將能夠向Webhook提供者發出授權API呼叫。 進行這些呼叫時，Workfront會在HTTP要求標題中傳送存取權杖，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果存取權杖已過期，Workfront會呼叫權杖端點URL以擷取新的存取權杖，然後使用新的存取權杖再次嘗試授權API呼叫。

### ApiKey

使用ApiKey向網頁連結提供者發出授權API呼叫比OAuth2簡單得多。 發出API呼叫時，Workfront只會在HTTP要求標題中傳遞ApiKey和Workfront使用者名稱：

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供者可使用使用者名稱來套用使用者專屬權限。 當兩個系統都使用單一登入(SSO)連接到LDAP時，這種方法效果最佳。

### 新增請求標題（選用）

除了使用OAuth2代號或ApiKey進行驗證外，Workfront還可針對每個API呼叫，將一組預先定義的標題傳送至網頁連結提供者。 如上節所述，Workfront管理員可在註冊或編輯Webook整合時設定此設定。 請參閱註冊Webhook整合。

例如，這可用於基本驗證。 為此，Workfront管理員會在「自訂整合」對話方塊中新增下列「請求標題」資訊：

   授權基本QWxhZGRpbjpvcGVuIHNlc2FtZQ==

其中QWxhZGRpbjpvcGVuIHNlc2FtZQ==是由「username:password」編碼的base-64字串。 請參閱基本驗證。 新增此項目後，除了其他請求標題外，Workfront還會在HTTP請求標題中傳遞此項目：

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API規格

以下為Webhook提供者應實作的API清單，以便檔案Webhook運作。

### 取得OAuth2代號（僅需OAuth2驗證）

傳回已驗證使用者的OAuth2重新整理Token和存取Token。 當用戶設定文檔提供程式時，將調用一次。 會進行後續呼叫，以取得更新的存取權杖。

HTTP要求POST/any/url

此URL是可設定的，並對應至自訂整合設定頁面上的Token端點URL值。

**查詢參數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱</th> 
   <th>必要</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>是</td> 
   <td> <p>值包括「authorization_code」或「refresh_token」。 指定的值會指出這兩個參數中的哪個將傳遞至此API呼叫：code或refresh_token。</p> </td> 
  </tr> 
  <tr> 
   <td>代碼</td> 
   <td>dessions</td> 
   <td> <p>在使用者按一下「授權」按鈕後，授權程式碼即傳送至Workfront。 只有當授權類型為「authorization_code」時，才需要此選項。 授權代碼應為短期，通常在10分鐘或更短時間內到期。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>dessions</td> 
   <td> <p>只有在後續呼叫以擷取新access_token時，才需要這個選項，因為先前的access_token已過期。 傳送此值時，請將grant_type參數設為「refresh_token」。</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>是</td> 
   <td>在Workfront中針對此自訂整合設定的用戶端ID。</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>是</td> 
   <td> Workfront中針對此自訂整合設定的用戶端密碼。</td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱</th> 
   <th>類型 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>字串</td> 
   <td> <p>代表使用者進行授權API呼叫的代號。 此過期時間應該會防止未授權的API呼叫。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>字串</td> 
   <td> <p>一種長期的Token，可透過呼叫此API方法來擷取新的access_token。</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>（選用）access_token過期的時間（以秒為單位），通常為3,600。</p></td> 
  </tr> 
 </tbody> 
</table>

 

**範例**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**回應**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### 獲取檔案或資料夾的元資料

傳回指定檔案或資料夾的中繼資料。

**URL**

GET/metadata?id=[文檔或資料夾ID]

**查詢參數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>檔案或資料夾的ID，由Webhook提供程式引用。 這與Workfront的檔案ID不同。 要獲取根目錄的元資料，請使用值「/」。</p><p>注意：ID的長度上限為255個字元。</p></td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>類型 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>字串 </td> 
   <td>文檔或資料夾的名稱</td> 
  </tr> 
  <tr> 
   <td>fy </td> 
   <td>字串 </td> 
   <td>指定此項目是檔案還是資料夾（「file」還是「folder」）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>字串 </td> 
   <td>檔案或資料夾的ID。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>字串 </td> 
   <td> <p>用戶在瀏覽器窗口中查看文檔的URL路徑。 URL可由檔案提供者或本機外部儲存提供者托管。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>字串 </td> 
   <td> <p>用戶在瀏覽器窗口中下載文檔的URL路徑。 URL可由檔案提供者或本機外部儲存提供者托管。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>字串 </td> 
   <td>檔案的MIME類型。 (可選)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>字串 </td> 
   <td>上次修改此檔案的時間（格式化的RFC 3339時間戳）</td> 
  </tr> 
  <tr> 
   <td>大小</td> 
   <td>長</td> 
   <td>  檔案的大小（以位元組為單位）。 (可選)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>布林值</td> 
   <td>  <p> 指出此檔案或資料夾是否為已驗證的使用者唯讀。(可選)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**範例：** `https://www.acme.com/api/metadata?id=12345`

**回應**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>錯誤處理應在所有API呼叫間保持一致。 如需詳細資訊，請參閱下方的「錯誤處理」一節。

### 取得資料夾中的項目清單

返回給定資料夾的檔案和資料夾的元資料。

**URL**

GET/檔案

**查詢參數**

| 名稱  | 說明 |
|---|---|
| parentId  | 資料夾ID。 要獲取根目錄的元資料，請使用值「/」。 |

{style=&quot;table-layout:auto&quot;}

Document Webhooks API目前不支援分頁。

**回應**

JSON包含檔案和資料夾清單。 每個項的元資料與/metadata端點返回的元資料相同。

**範例：** `https://www.acme.com/api/files?parentId=123456`

**回應**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### 搜尋

返回從搜索返回的檔案和資料夾的元資料。 這可以作為全文搜索或作為常規資料庫查詢來實現。 當使用者從外部檔案瀏覽器執行搜尋時，Workfront會呼叫/search端點。

**URL**

GET/搜尋

**查詢參數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>查詢</td> 
   <td>搜尋詞或片語。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（可選）執行搜尋的資料夾ID。 注意：這是Workfront未來功能的預留位置。 目前，Workfront未傳遞此參數。 </p> </td> 
  </tr> 
  </tbody> 
</table>

Document Webhooks API目前不支援分頁。

 

**回應**

JSON包含符合查詢之檔案和資料夾的中繼資料清單。 「符合」的構成由Webhook提供者決定。 理想情況下，它應該進行全文搜索。 執行檔案名稱型搜尋也是可行的。

**範例：** `https://www.acme.com/api/search?query=test-query`

**回應**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### 獲取文檔的內容

返回文檔的原始位元組

**URL**

GET/下載

**查詢參數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> 文檔ID。</td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

文檔的原始位元組。

**範例：** `https://www.acme.com/api/download?id=123456`

### 獲取文檔的縮略圖

傳回檔案的原始縮圖位元組。

**URL**

GET/縮圖

**查詢參數**

| 名稱  | 說明 |
|---|---|
| id  | 文檔ID。 |
| 大小  |  縮圖的寬度 |

{style=&quot;table-layout:auto&quot;}

 

**回應**

原始縮圖位元組。

**範例：** `https://www.acme.com/api/thumbnail?id=123456`

### 上傳檔案 — 第1部分（共2部分）

將檔案上傳至檔案儲存提供者是兩步驟程式，需要兩個不同的API端點。 Workfront借由呼叫/uploadInit來開始上傳程式。 此端點會傳回檔案ID，然後在上傳檔案位元組時傳遞至/upload。 根據基礎文檔儲存系統，可能需要建立一個零長度的文檔，然後稍後更新文檔的內容。

新增至此規格的1.1版，檔案ID和檔案版本ID可用來擷取來自Workfront的額外資訊。 例如，如果文檔管理系統需要有關該文檔的額外資訊，Webhook實施代碼可以使用文檔ID來使用Workfront的RESTful API檢索該資訊。 此資訊可能來自檔案上的自訂資料欄位，且包含任務、問題或專案，此為最佳作法。

**URL**

POST/uploadInit

**查詢參數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>上層資料夾ID，由Webhook提供者參考。</td> 
  </tr> 
  <tr> 
   <td>檔案名 </td> 
   <td>文檔的名稱</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront檔案ID（在1.1版中新增）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront檔案版本ID（在1.1版中新增）</td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

檔案的元資料，由/metadata端點定義。

**範例：** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**回應**

`[file_metadata]` 包括文檔提供程式使用的新文檔ID。

### 上傳檔案 — 第2部分（共2部分）

將文檔的位元組上載到Webhook提供程式。

**URL**

PUT/上傳

**查詢參數**

| 名稱  | 說明 |
|---|---|
| id  |  剛建立的文檔ID。 |


 

**要求內文**

文檔的原始內容位元組。

**回應**

```
{
"result": "success"
}
```

或

```
{
"result": "fail"
}
```

**範例：** `https://www.acme.com/api/upload?id=1234` *[更新流中包含的文檔位元組]*

**回應**

```
{
"result":"success"
}
```

### 取得服務的相關資訊 

（發行日期 — TBD）傳回服務的相關資訊，例如功能。 Workfront將使用此資訊來自訂Workfront中的使用者介面。 例如，如果網頁連結實作包含某些自訂動作，JSON應在JSON中列出這些操作。 接著，使用者便能從Workfront叫用這些動作。

**URL**

GET/serviceInfo

查詢參數

無. 此外，對此端點的呼叫不應需要驗證。

**回應**

包含此服務相關資訊的JSON

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱</th> 
   <th>類型 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>字串 </td> 
   <td>由此服務實作的WebHook版本。 這是此規格頂部列出的版本號。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字串 </td> 
   <td>此服務的內部版本號。 此編號由Webhook服務提供商確定，僅用於資訊用途。<br><br></td> 
  </tr> 
  <tr> 
   <td>發佈者 </td> 
   <td>字串 </td> 
   <td>提供Webhook實作的公司名稱。</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>字串 </td> 
   <td>包含此服務實作之API端點的清單。 這可用來確保Workfront中的使用者介面反映Webhook提供者提供的功能。 清單中的每個項目都必須包含端點名稱（例如「search」）。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>字串</td> 
   <td>  <p>包含由此Webhook實作的自訂操作的清單。 每個清單項目都包含名稱和顯示名稱。 顯示名稱會顯示在Workfront的「檔案動作」下拉式清單中。 按一下下拉式清單中的項目，會呼叫/customAction端點來叫用Webhook中的動作。</p></td> 
  </tr> 
 </tbody> 
</table>

**範例：** https://www.acme.com/api/serviceInfo

**傳回**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### 建立資料夾

（在1.2版中新增）在指定目錄中建立資料夾。
URL

POST/createFolder

**查詢參數**

| 名稱  | 說明 |
|---|---|
| parentId  | 應在其中建立資料夾的資料夾ID |
| 名稱  | 新資料夾的名稱 |

{style=&quot;table-layout:auto&quot;}

 

**回應**

新建立資料夾的元資料，由/metadata端點定義。

**範例：** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

傳回

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### 刪除文檔或資料夾

（發行日期 — TBD）刪除外部系統中具有指定ID的文檔或資料夾。 刪除資料夾也會刪除其內容。

URL

PUT/刪除

**查詢參數**

| 名稱  | 說明 |
|---|---|
| documentId  | 要刪除的文檔ID |
| folderId  |  要刪除的資料夾ID |

{style=&quot;table-layout:auto&quot;}

回應指出成功或失敗的JSON字串，如下方的錯誤處理一節所指定。

**範例：** PUThttps://www.acme.com/api/delete id=1234

傳回

```
{
"status": "success" 
}
```

傳回

```
{
"status": "failure", "error": "File not found"
}
```


### 更名文檔或資料夾

（發行日期 — 待定）使用外部系統中的指定ID重新命名檔案或資料夾。

URL

PUT/重新命名

**查詢參數**

| 名稱  | 說明 |
|---|---|
| id | 要更名的文檔或資料夾ID |
| 名稱  | 文檔或資料夾的新名稱 |

{style=&quot;table-layout:auto&quot;}

 

個回應

表示成功或失敗的JSON字串，如下方的錯誤處理一節中所指定。

**範例:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### 執行自訂動作

（發行日期 — 待定）此端點可讓Workfront使用者（或自動化工作流程事件）在外部系統中執行動作。 /customAction端點接受「name」參數，該參數允許Webhook提供程式實施多個自定義操作。

Webhook提供者會將動作納入customActions下的/serviceInfo回應中，以向Workfront註冊自訂動作。 Workfront在「設定>檔案>自訂整合」下設定或重新整理網頁連結提供者時，會載入此清單。\
![](assets/mceclip0-350x262.png)

使用者可以選取「檔案動作」下方的區段，以觸發自訂動作\
![](assets/mceclip1-350x95.png)

**URL**

GET/customAction

**查詢參數**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>名稱 </th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>名稱</p></td>
   <td><p>指定要執行之動作類型的識別碼。 此值對應於/serviceInfo端點返回的一個customAction值。</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>正在為其執行操作的工作流文檔ID。</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> 正在執行操作的Workfront文檔版本ID。</td>
  </tr>
 </tbody>
</table>

 

**回應**

表示成功或失敗的JSON字串，如下方的錯誤處理一節中所指定。 失敗時（即狀態= &quot;failure&quot;）,Workfront會向使用者顯示提供的錯誤訊息。

**範例：** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

回應

```
{
"status": "success" 
}
```


## 錯誤處理

處理API請求時可能會產生問題。 這應在所有API端點間以一致的方式處理。 發生錯誤時，Webhook提供程式會執行下列操作：

* 在回應標題中加入錯誤碼。 錯誤代碼包括：

   * 403 — 禁止。 指出要求Token遺失或無效，或與Token相關聯的認證無權存取指定的資源。 針對OAuth型網頁連結提供者，Workfront會嘗試擷取新的存取權杖。
   * 404 — 找不到。 指示指定的檔案或資料夾不存在。
   * 500 — 內部伺服器錯誤。 任何其他類型的錯誤。

* 使用下列格式說明回應內文中的錯誤：


```
{
"status": "error"
"error": "Sample error message" 
}
```


## 測試

若要驗證您的檔案WebHook實作是否正確運作，請執行下列測試。 這些是手動測試，會透過Workfront Web介面間接點擊您Webhook實作的端點。

### 必要條件

若要執行這些測試，您需要下列項目：

* 已啟用進階檔案管理(ADM)的Workfront帳戶
* 具有系統管理員權限之此帳戶的Workfront使用者
* Document Webhook例項，其HTTP端點可供Workfront存取

這些測試也假設您已在Workfront的「設定>檔案>自訂整合」下註冊Document Webhook例項。

### 測試1:為用戶提供文檔Webhook服務

測試OAuth型Webhook提供者的驗證URL和Token端點URL。

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 按一下「添加文檔」下拉清單，並在「添加服務」下選擇「文檔Webhook服務」。
1. （僅限OAuth服務）完成上一個步驟後，您會在快顯視窗中看到服務的OAuth2驗證頁面載入。 (注意：系統可能會提示您先登錄服務。) 在驗證頁面中，按一下信任或允許按鈕，授予Workfront對使用者帳戶的存取權。
1. 確認您的服務已新增至新增檔案下拉式清單。 如果您一開始沒有看到，請嘗試重新整理瀏覽器。

### 測試2:將檔案連結至Workfront測試下列端點：/files, /metadata

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 在「添加文檔」下選擇「文檔Webhook」服務。
1. 在強制回應視窗中，導覽資料夾結構。
1. 驗證是否能正確導覽資料夾結構。
1. 選取檔案並將其連結至Workfront

### 測試3:導覽至內容管理系統中的檔案

測試下列端點：/metadata（尤其是viewLink）

1. 將檔案連結至Workfront
1. 選擇文檔，然後按一下「開啟」(Open)連結。
1. 驗證文檔是否在新頁簽中開啟。

### 測試4:導覽至內容管理系統中的檔案（含登入）

測試下列端點：/metadata（尤其是viewLink）

1. 確保您已登出內容管理系統。
1. 將檔案連結至Workfront。
1. 選擇文檔，然後按一下「開啟」(Open)連結。
1. 驗證內容管理系統的登錄螢幕是否在新頁簽中載入。
1. 登入並確認您已被帶入檔案

### 測試5:從內容管理系統下載文檔

測試下列端點：/metadata（尤其是downloadLink）

1. 將檔案連結至Workfront。
1. 選擇文檔，然後按一下「下載」連結。
1. 確認下載開始。

### 測試6:搜尋內容

測試下列端點：/search

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 在「添加文檔」下選擇「文檔Webhook」服務。
1. 在強制回應視窗中執行搜尋。
1. 驗證搜索結果是否正確。

### 測試7:將檔案從Workfront傳送至內容管理系統

測試下列端點：/files, /uploadInit, /upload

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 從電腦上傳檔案至Workfront
1. 轉到文檔詳細資訊頁
1. 在「文檔操作」下拉清單中，在「發送到……」下選擇「文檔Webhook服務」
1. 前往所需的目的地資料夾，然後按一下「儲存」按鈕。
1. 驗證文檔已上載到內容管理系統中的正確位置。

### 測試8:在Workfront中檢視縮圖

測試下列端點：/thumbnail

1. 將檔案連結至Workfront。
1. 在清單中選擇文檔。
1. 確認縮圖出現在右側面板中。

### 測試9:取得內容位元組

測試下列端點：/download

1. 將檔案連結至Workfront。
1. 轉到文檔詳細資訊頁。
1. 選擇「文檔操作」>「發送到……」>「Workfront」，將文檔發送到Workfront。 這會在Workfront中建立新的檔案版本。
1. 按一下「下載」連結，從Workfront下載檔案。

### 測試10:重新整理存取權杖（僅限OAuth2網頁連結提供者）

測試下列端點：代號端點URL

1. 為用戶提供文檔Webhook服務
1. 讓使用者的存取權杖失效，方法是1)等待它逾時，或2)在外部系統中手動使它失效。
1. 在Workfront中重新整理存取權杖。 例如，您可以將檔案連結至Workfront，即可完成此操作。 如果您能夠導覽至並連結檔案，則會知道存取權杖已成功重新整理。

>[!NOTE]
>
>目前，「發送對象……」不適用於連結的文檔。 這將由Workfront新增。 您可以使用REST用戶端(例如Postman)手動點擊端點，以測試/download端點。 或者，可通過生成數字校樣來測試/download端點。 若要啟用數位校對功能，請聯絡Workfront。

## 版本

* 1.0版（發行日期 — 2015年5月）

   * 初始規格

* 版本1.1（發行日期 — 2015年6月）

   * 更新/uploadInit — 新增documentId和documentVersionId

* 版本1.2（發行日期 — 2015年10月）

   * 新增/createFolder

