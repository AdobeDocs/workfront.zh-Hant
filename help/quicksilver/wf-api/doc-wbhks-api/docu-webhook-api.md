---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 檔案Webhooks API
description: Adobe Workfront Document Webhooks定義了一組API端點，Workfront會透過這些端點向外部檔案提供者發出授權的API呼叫。 這可讓任何人為任何檔案儲存提供者建立中介外掛程式。
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '3649'
ht-degree: 2%

---


# 檔案Webhooks API

<!-- Audited: 5/2025 -->

Adobe Workfront Document Webhooks定義了一組API端點，Workfront會透過這些端點向外部檔案提供者發出授權的API呼叫。 這可讓任何人為任何檔案儲存提供者建立中介外掛程式。

webhook型整合的使用者體驗將與現有檔案整合類似，例如Google Drive、Box和Dropbox。 例如，Workfront使用者將能夠執行下列動作：

* 瀏覽外部檔案提供者的檔案夾結構
* 搜尋檔案
* 將檔案連結至Workfront
* 將檔案上傳到外部檔案提供者
* 檢視檔案的縮圖

## 參考實作

為協助快速開始開發新的Webhook實作，Workfront提供參考實作。 您可以在[https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app)找到此專案的程式碼。 此實作以Java為基礎，可讓Workfront在網路檔案系統上連線檔案。

## 註冊Webhook整合

Workfront管理員可透過導覽至Workfront中的「設定>檔案>自訂整合」，為其公司新增自訂webhook整合。 在「設定」的「自訂整合」頁面中，管理員可以檢視現有檔案Webhook整合的清單。 您可以在此頁面新增、編輯、啟用和停用整合。 若要新增整合，請按一下新增整合按鈕。

### 可用欄位

新增整合時，管理員會在下列欄位中輸入值：

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
   <td>姓名</td> 
   <td>此整合的名稱。</td> 
  </tr> 
  <tr> 
   <td>基底 API URL</td> 
   <td> <p>回撥API的位置。 呼叫外部系統時，Workfront會將端點名稱附加至此位址。 例如，如果管理員輸入基本API URL " https://www.mycompany.com/api/v1 "，Workfront將使用以下URL來取得檔案的中繼資料：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>要求引數</td> 
   <td> <p>附加至每個 API 呼叫的 querystring 的選用值。例如，access_type</p> </td> 
  </tr> 
  <tr> 
   <td>驗證類型</td> 
   <td>OAuth2或ApiKey。</td> 
  </tr> 
  <tr> 
   <td>驗證 URL</td> 
   <td> <p>（僅限OAuth2）用於使用者驗證的完整URL。 Workfront會在OAuth布建程式過程中，將使用者導覽至此位址。 <br><br>注意： Workfront會將"state"引數附加至查詢字串。 提供者必須透過將此附加至Workfront重新導向URI，將其傳回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>權杖端點 URL</td> 
   <td> <p>（僅限OAuth2）用於擷取OAuth2 Token的完整API URL。 這是由webhook提供者或外部檔案提供者所託管。</p> </td> 
  </tr> 
  <tr> 
   <td>用戶端 ID</td> 
   <td>（僅限OAuth2）此整合的OAuth2使用者端ID。</td> 
  </tr> 
  <tr> 
   <td>用戶端密碼</td> 
   <td> <p>（僅限OAuth2）此整合的OAuth2使用者端密碼。</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重新導向 URI</td> 
   <td> <p>（僅限OAuth2）這是唯讀欄位，由Workfront產生。 此值可用來向外部檔案提供者註冊此整合。 <br><br>注意：如上述驗證URL所述，提供者在執行重新導向時，必須將"state"引數及其值附加至querystring。</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>（僅限ApiKey）用來對webhook提供者進行授權的API呼叫。 API金鑰由webhook提供者發行。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 驗證

Workfront檔案webhook支援兩種不同的驗證形式： OAuth2和ApiKey。 在這兩種情況下，Workfront都會在進行API呼叫時在標題中傳遞驗證權杖。

### OAuth2

OAuth2可讓Workfront代表使用者向webhook提供者發出授權的API呼叫。 在執行此操作之前，使用者必須將其外部檔案提供者帳戶連結至Workfront，並授予Workfront存取權以代表其採取行動。 此握手程式只會針對每位使用者進行一次。 以下是運作方式：

1. 使用者開始將webhook整合連線至其帳戶。 目前，若要這麼做，請按一下新增檔案下拉式清單>新增服務>自訂整合名稱。
1. Workfront會將使用者導覽至驗證URL，這可能會提示使用者登入外部檔案提供者。 此頁面由webhook提供者或外部檔案管理系統託管。 Workfront這麼做時，會將「state」引數新增至驗證URL。 必須在下列步驟中，將相同的值附加至Workfront傳回URI，將此值傳回Workfront。
1. 登入外部系統後（或如果使用者已登入），使用者將被帶到「驗證」頁面，此頁面說明Workfront正在請求存取權，以代表使用者執行一組動作。
1. 如果使用者按一下「允許」按鈕，瀏覽器會重新導向至Workfront重新導向URI ，新增&quot;code=`<code>`&quot;至查詢字串。 根據OAuth2規格，此代號只會短暫有效。 查詢字串也必須具有下列專案： &quot;state=`<sent_by_workfront>`&quot;。
1. Workfront處理此要求，並使用授權代碼對權杖端點URL進行API呼叫。
1. 權杖端點URL會傳回重新整理權杖和存取權杖。
1. Workfront會儲存這些Token並完整布建此使用者的webhook整合。
1. 從現在開始，Workfront將能夠向webhook提供者發出授權的API呼叫。 進行這些呼叫時，Workfront會在HTTP請求標頭中傳送存取權杖，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果存取權杖已過期，Workfront將會呼叫權杖端點URL以擷取新的存取權杖，然後使用新的存取權杖再次嘗試授權API呼叫。

### ApiKey

使用ApiKey向webhook提供者發出授權API呼叫比OAuth2簡單得多。 進行API呼叫時，Workfront只會在HTTP請求標頭中傳遞ApiKey和Workfront使用者名稱：

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供者可以使用使用者名稱來套用使用者特定的許可權。 當兩個系統都使用單一登入(SSO)連線至LDAP時，這個方法最有效。

### 新增請求標頭（選用）

除了使用OAuth2 Token或ApiKey進行驗證外，Workfront還可以為每個API呼叫將預先定義的標題集傳送給webhook提供者。 Workfront管理員可在註冊或編輯Webook整合時進行此設定，如上節所述。

例如，這可用於基本驗證。 若要這麼做，Workfront管理員會在「自訂整合」對話方塊中新增下列「請求標題」資訊：

   授權基本QWxhZGRpbjpvcGVuIHNlc2FtZQ==

其中QWxhZGRpbjpvcGVuIHNlc2FtZQ==是「username：password」的base-64編碼字串。 請參閱基本驗證。 如果新增此專案，Workfront除了其他請求標頭外，還會在HTTP請求標頭中傳遞此專案：

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API規格

以下是webhook提供者應該實作的API清單，以便檔案webhook運作。

### 取得OAuth2 Token （僅需要OAuth2驗證）

傳回已驗證使用者的OAuth2重新整理權杖和存取權杖。 當使用者布建檔案提供者時，就會叫用一次。 進行後續呼叫以取得更新的存取Token。

HTTP要求POST /any/url

URL可設定，並與自訂整合設定頁面上的權杖端點URL值相對應。

**查詢引數**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>姓名</th> 
   <th>必要</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>是</td> 
   <td> <p>值包括「authorization_code」或「refresh_token」。 指定的值表示將傳遞至此API呼叫的兩個引數之一： code或refresh_token。</p> </td> 
  </tr> 
  <tr> 
   <td>程式碼</td> 
   <td>根據</td> 
   <td> <p>使用者按一下「授予」按鈕後就會傳送至Workfront的授權代碼。 僅當授權型別為「authorization_code」時才需要此項。 授權碼應為短期，通常在10分鐘或更短時間內到期。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>根據</td> 
   <td> <p>只有在進行後續呼叫以擷取新的access_token時才需要此專案，因為先前的access_token已過期。 傳送此值時，請將grant_type引數設為"refresh_token"。</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>是</td> 
   <td>在Workfront中針對此自訂整合設定的使用者端ID。</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>是</td> 
   <td> Workfront中針對此自訂整合設定的使用者端密碼。</td> 
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
   <th>姓名</th> 
   <th>型別 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>字串</td> 
   <td> <p>代號，用來代表使用者進行授權的API呼叫。 此專案應該會過期，以防止未經授權的API呼叫。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>字串</td> 
   <td> <p>長效權杖，用於透過呼叫此API方法擷取新的access_token。</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>長</td> 
   <td>  <p>（選用） access_token過期前的時間（以秒為單位），通常為3,600。</p></td> 
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

### 取得檔案或資料夾的中繼資料

傳回指定檔案或資料夾的中繼資料。

**URL**

GET /metadata？id=[檔案或資料夾識別碼]

**查詢引數**

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
   <td>  <p>檔案或資料夾的ID，由webhook提供者參照。 這與Workfront的檔案ID不同。 若要取得根目錄的中繼資料，請使用值'/'。</p><p>注意：ID的長度上限為255個字元。</p></td> 
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
   <th>型別 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>標題 </td> 
   <td>字串 </td> 
   <td>檔案或資料夾的名稱。</td> 
  </tr> 
  <tr> 
   <td>種類 </td> 
   <td>字串 </td> 
   <td>指定此專案是檔案還是資料夾（'file'或'folder'）。</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>字串 </td> 
   <td>檔案或資料夾的識別碼。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>字串 </td> 
   <td> <p>使用者在瀏覽器視窗中檢視檔案時所使用的URL路徑。 URL可由檔案提供者或原生外部儲存提供者來託管。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>字串 </td> 
   <td> <p>使用者在瀏覽器視窗中下載檔案時使用的URL路徑。 URL可由檔案提供者或原生外部儲存提供者來託管。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>字串 </td> 
   <td>（選用）檔案的MIME型別。</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>字串 </td> 
   <td>上次修改此檔案的時間（格式為RFC 3339時間戳記）。</td> 
  </tr> 
  <tr> 
   <td>大小</td> 
   <td>長</td> 
   <td>（選用）檔案大小（位元組）。</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>布林值</td> 
   <td><p> （選擇性）指出此檔案或資料夾對於已驗證的使用者是否為唯讀。</p><p> </p></td> 
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
>所有API呼叫的錯誤處理都應保持一致。 如需詳細資訊，請參閱下文的錯誤處理一節。

### 取得資料夾中的專案清單

傳回指定資料夾之檔案和資料夾的中繼資料。

**URL**

GET /files

**查詢引數**

| 名稱  | 說明 |
|---|---|
| parentId  | 資料夾識別碼。 若要取得根目錄的中繼資料，請使用值&#39;/&#39;。 |

{style="table-layout:auto"}

檔案Webhooks API目前不支援分頁。

**回應**

包含檔案和資料夾清單的JSON。 每個專案的中繼資料與/metadata端點傳回的中繼資料相同。

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

### 進行搜尋

傳回搜尋傳回之檔案和資料夾的中繼資料。 這可作為全文檢索搜尋或一般資料庫查詢來實施。 當使用者從外部檔案瀏覽器執行搜尋時，Workfront會呼叫/search端點。

**URL**

GET /search

**查詢引數**

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
   <td>搜尋字詞或片語。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（選用）執行搜尋的來源資料夾ID。 <br><br>注意：這是Workfront中未來功能的預留位置。 目前Workfront不會傳遞此引數。 </p> </td> 
  </tr> 
  </tbody> 
</table>

檔案Webhooks API目前不支援分頁。

 

**回應**

JSON，其中包含符合查詢的檔案和資料夾的中繼資料清單。 構成「符合」的專案由webhook提供者決定。 理想情況下，應該執行全文檢索或檔案名稱式搜尋。

**範例：** `https://www.acme.com/api/search?query=test-query`

**回應**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### 取得檔案的內容

傳回檔案的原始位元組。

**URL**

GET /下載

**查詢引數**

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
   <td> 檔案識別碼。</td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

檔案的原始位元組。

**範例：** `https://www.acme.com/api/download?id=123456`

### 取得檔案的縮圖

傳回檔案的原始縮圖位元組。

**URL**

GET /thumbnail

**查詢引數**

| 名稱  | 說明 |
|---|---|
| id  | 檔案識別碼。 |
| 大小  | 縮圖的寬度。 |

{style="table-layout:auto"}

 

**回應**

原始縮圖位元組。

**範例：** `https://www.acme.com/api/thumbnail?id=123456`

### 上傳檔案 — 第1部分，共2部分

將檔案上傳至檔案儲存提供者是一個兩步驟的程式，需要2個獨立的API端點。 Workfront會呼叫/uploadInit以開始上傳程式。 此端點會傳回檔案ID，然後在上傳檔案位元組時傳遞給/upload。 根據基礎檔案儲存系統，可能需要建立長度為零的檔案，然後稍後更新檔案的內容。

將檔案ID和檔案版本ID新增至本規格1.1版，可用來從Workfront擷取額外資訊。 例如，如果檔案管理系統想要關於檔案的額外資訊，webhook實作程式碼可以使用檔案ID來使用Workfront的RESTful API擷取該資訊。 好的實務是，此資訊可能來自檔案及其包含任務、問題或專案的自訂資料欄位。

**URL**

POST /uploadInit

**查詢引數**

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
   <td>Webhook提供者參照的父資料夾ID。</td> 
  </tr> 
  <tr> 
   <td>檔案名稱 </td> 
   <td>檔案的名稱。</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront檔案ID （在1.1版中新增）。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront檔案版本ID （在1.1版中新增）。</td> 
  </tr> 
 </tbody> 
</table>

 

**回應**

由/metadata端點定義的檔案中繼資料。

**範例：** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**回應**

`[file_metadata]`包含檔案提供者使用的新檔案識別碼。

### 上傳檔案 — 第2部分（共2部分）

將檔案的位元組上傳到webhook提供者。

**URL**

PUT /upload

**查詢引數**

| 名稱  | 說明 |
|---|---|
| id  |  剛建立的檔案ID。 |


 

**要求內文**

檔案的原始內容位元組。

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

**範例：** `https://www.acme.com/api/upload?id=1234` *[包含在更新資料流中的檔案位元組]*

**回應**

```
{
"result":"success"
}
```

### 取得服務的相關資訊 

（發行日期 — 待定）傳回服務的相關資訊，例如特性與功能。 Workfront將使用此資訊在Workfront中自訂使用者介面。 例如，如果webhook實作包含一些自訂動作，JSON應在JSON中列出這些動作。 之後，使用者就可以從Workfront叫用這些動作。

**URL**

GET /serviceInfo

查詢參數

無。 此外，對此端點的呼叫不應需要驗證。

**回應**

包含此服務相關資訊的JSON。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>姓名</th> 
   <th>型別 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>字串 </td> 
   <td>此服務實作的webhook版本。 這是列在此規格頂端的版本編號。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字串 </td> 
   <td>此服務的內部版本號碼。 此數字由webhook服務提供者決定，僅供參考。<br><br></td> 
  </tr> 
  <tr> 
   <td>發佈者 </td> 
   <td>字串 </td> 
   <td>提供webhook實作的公司名稱。</td> 
  </tr> 
  <tr> 
   <td>availableendpoints</td> 
   <td>字串 </td> 
   <td>包含此服務實作之API端點的清單。 這可用來確保Workfront中的使用者介面反映webhook提供者所提供的功能。 清單中的每個專案都必須包含端點的名稱（例如「search」）。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>字串</td> 
   <td>  <p>包含此Webhook實作的自訂作業清單。 每個清單專案都包含名稱和顯示名稱。 顯示名稱會顯示在Workfront的「檔案動作」下拉式清單中。 按一下下拉式清單中的專案時，將會呼叫/customAction端點，以叫用webhook中的動作。</p></td> 
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

POST /createFolder

**查詢引數**

| 名稱  | 說明 |
|---|---|
| parentId  | 應在其中建立資料夾的資料夾ID。 |
| 名稱  | 新資料夾的名稱。 |

{style="table-layout:auto"}

 

**回應**

新建立資料夾的中繼資料，如/metadata端點所定義。

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

### 刪除檔案或資料夾

（發行日期 — 待定）刪除外部系統中具有特定ID的檔案或資料夾。 刪除資料夾也會刪除其內容。

URL

PUT /delete

**查詢引數**

| 名稱  | 說明 |
|---|---|
| documentId  | 要刪除的檔案識別碼。 |
| folderId  | 要刪除的資料夾ID。 |

{style="table-layout:auto"}

回應：指出成功或失敗的JSON字串，如底下「錯誤處理」區段中所指定。

**範例：** PUT https://www.acme.com/api/delete id=1234

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


### 重新命名檔案或資料夾

（發行日期 — 待定）重新命名外部系統中具有特定ID的檔案或資料夾。

URL

PUT /rename

**查詢引數**

| 名稱  | 說明 |
|---|---|
| id | 要重新命名的檔案或資料夾ID。 |
| 名稱  | 檔案或資料夾的新名稱。 |

{style="table-layout:auto"}

 

回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。

**範例：**

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

（發行日期 — 待定）此端點會允許Workfront使用者（或可能是自動化工作流程事件）在外部系統中執行動作。 /customAction端點接受「name」引數，此引數允許webhook提供者實作多個自訂操作。

webhook提供者會將actions包含在customActions下的/serviceInfo回應中，藉此向Workfront註冊自訂動作。 Workfront會在設定>檔案>自訂整合底下設定或重新整理webhook提供者時載入此清單。\
![執行自訂動作](assets/mceclip0-350x262.png)

使用者可透過選取「檔案動作」下的區段來觸發自訂動作。\
![觸發自訂動作](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**查詢引數**

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
   <td><p>指定要執行的動作型別的識別碼。 此值對應至/serviceInfo端點傳回的其中一個customAction值。</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>正在對其執行動作的Workfront檔案ID。</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td>正在對其執行動作的Workfront檔案版本ID。</td>
  </tr>
 </tbody>
</table>

 

**回應**

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。 失敗時（即狀態= &quot;failure&quot;），Workfront會向使用者顯示提供的錯誤訊息。

**範例：** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

回應

```
{
"status": "success" 
}
```


## 錯誤處理

處理API請求時可能會出現問題。 所有API端點的處理方式都應保持一致。 發生錯誤時，webhook提供者會執行下列動作：

* 在回應標頭中包含錯誤代碼。 錯誤碼包括：

   * 403 — 禁止。 指出要求權杖遺失或無效，或是與權杖關聯的認證無權存取指定的資源。 對於以OAuth為基礎的webhook提供者，Workfront將嘗試擷取新的存取權杖。
   * 404 — 找不到。 表示指定的檔案或資料夾不存在。
   * 500 — 內部伺服器錯誤。 任何其他型別的錯誤。

* 使用以下格式說明回應本文中的錯誤：


```
{
"status": "error"
"error": "Sample error message" 
}
```


## 測試中

若要驗證檔案webhook實作是否正常運作，請執行以下測試。 這些是透過Workfront網頁介面的手動測試，並間接點選webhook實施的端點。

### 先決條件

若要執行這些測試，您將需要下列專案：

* 已啟用進階檔案管理(ADM)的Workfront帳戶。
* 此帳戶的Workfront使用者，擁有系統管理員許可權。
* Workfront可存取其HTTP端點的檔案Webhook例項。

這些測試也假設您已經在Workfront中的「設定>檔案>自訂整合」下註冊了Document Webhook例項。

### 測試1：為使用者布建Document Webhook服務

測試以OAuth為基礎的Webhook提供者的驗證URL和權杖端點URL。

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 按一下「新增檔案」下拉式清單，並在「新增服務」下選取您的Document Webhook服務。
1. （僅限OAuth服務）完成上一步驟後，您會在快顯視窗中看到服務的OAuth2驗證頁面載入載入內容。 （注意：系統可能會提示您先登入服務。） 在驗證頁面中，按一下「信任」或「允許」按鈕，授予Workfront使用者帳戶的存取權。
1. 確認您的服務已新增至新增檔案下拉式清單。 如果一開始沒有看見，請嘗試重新整理瀏覽器。

### 測試2：將檔案連結至Workfront測試下列端點： /files、/metadata

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 在新增檔案下選擇您的檔案Webhook服務。
1. 從強制回應視窗中，導覽至資料夾結構。
1. 確認您能夠正確導覽資料夾結構。
1. 選取檔案並將其連結至Workfront。

### 測試3：導覽至內容管理系統中的檔案

測試下列端點： /metadata （尤其是viewLink）。

1. 將檔案連結至Workfront。
1. 選取檔案並按一下「開啟」連結。
1. 確認檔案會在新標籤中開啟。

### 測試4：導覽至內容管理系統中的檔案（含登入）

測試下列端點： /metadata （尤其是viewLink）。

1. 確保您已登出內容管理系統。
1. 將檔案連結至Workfront。
1. 選取檔案並按一下「開啟」連結。
1. 確認內容管理系統的登入畫面會在新標籤中載入。
1. 登入並確認您已進入檔案。

### 測試5：從內容管理系統下載檔案

測試以下端點： /metadata （尤其是downloadLink）。

1. 將檔案連結至Workfront。
1. 選取檔案並按一下下載連結。
1. 確認下載開始。

### 測試6：搜尋內容

測試下列端點： /search

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 在新增檔案下選擇您的檔案Webhook服務。
1. 從強制回應視窗中，執行搜尋。
1. 確認搜尋結果是否正確。

### 測試7：將檔案從Workfront傳送至內容管理系統

測試下列端點： /files、/uploadInit、/upload

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 從您的電腦上傳檔案至Workfront。
1. 前往檔案詳細資訊頁面。
1. 從「檔案動作」下拉式清單中，選取「傳送至……」下的「檔案Webhook」服務。
1. 前往所需的目的地資料夾，然後按一下「儲存」按鈕。
1. 確認檔案已上傳至內容管理系統中的正確位置。

### 測試8：在Workfront中檢視縮圖

測試下列端點： /thumbnail

1. 將檔案連結至Workfront。
1. 選取清單中的文件。
1. 確認縮圖出現在右側面板中。

### 測試9：取得內容位元組

測試下列端點： /download

1. 將檔案連結至Workfront。
1. 前往檔案詳細資訊頁面。
1. 透過選取檔案動作>傳送至…… > Workfront，將檔案傳送至Workfront。 這會在Workfront中建立新的檔案版本。
1. 按一下「下載」連結，從Workfront下載檔案。

### 測試10：重新整理存取權杖（僅限OAuth2 Webhook提供者）

測試下列端點：權杖端點URL

1. 為使用者布建Document Webhook服務。
1. 等候使用者的存取權杖逾時或在外部系統中手動讓使用者存取權杖失效。
1. 在Workfront中重新整理存取Token。 例如，您可以將檔案連結至Workfront來執行此操作。 如果您能夠導覽至並連結檔案，您將知道存取權杖已成功重新整理。

>[!NOTE]
>
>目前，傳送至……不適用於連結的檔案。 Workfront將新增此專案。 您可以使用REST使用者端(例如Postman)手動點選端點來測試/download端點。 或者，也可以透過產生數位校樣來測試/download端點。 若要啟用，數位校訂，請聯絡Workfront。

## 版本

* 1.0版（發行日期 — 2015年5月）

   * 初始規格

* 1.1版（發行日期 — 2015年6月）

   * 更新/uploadInit — 新增documentId和documentVersionId

* 1.2版（發行日期 — 2015年10月）

   * 新增/createFolder

