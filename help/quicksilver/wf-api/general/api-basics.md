---
content-type: api
navigation-topic: general-api
title: API 基本概念
description: API 基本概念
author: Becky
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 01f5970fc17f9390d48b00541c912d21ba77c0a4
workflow-type: tm+mt
source-wordcount: '4478'
ht-degree: 0%

---


# API 基本概念

Adobe Workfront API的目標是透過引入透過HTTP運作的REST風格架構，簡化與Workfront的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Workfront API採用的方法。

熟悉Workfront結構有助於了解可用於將資料從Workfront中提取以用於整合目的的資料庫關係。

## 限制與准則

為確保Workfront隨選系統效能一致，每個客戶最多只能有10個同時執行的API執行緒。 沙箱環境有相同的限制，讓客戶和合作夥伴在將程式碼發行至生產環境之前，能夠精確測試API呼叫。

針對生產、預覽和測試硬碟環境，一般使用者請求的URI長度上限為8892個位元組，因為這些請求是透過Workfront CDN(Akamai)路由。 此限制僅適用於透過CDN路由的URI。

>[!NOTE]
>
>此限制不適用於沙箱環境，因為沙箱環境不會透過CDN路由。

### 免責聲明

API的任何使用應先在Workfront測試版環境中測試，再在生產環境中執行。 如果任何客戶將API用於Workfront合理認為對隨選軟體造成負擔的程式（即該程式對其他客戶的軟體效能造成重大負面影響）,Workfront保留要求客戶停止該程式的權利。 如果客戶不遵守規定且問題持續存在，Workfront保留終止程式的權利。

## REST基本知識

本節提供如何與Workfront REST API互動的高階簡介，以遵循下列REST原則：

### 對象URI

系統中的每個對象都被指定一個唯一URI，由對象類型和ID組成。 以下示例顯示了描述三個唯一對象的URI:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

物件類型不區分大小寫，可以是縮寫的ObjCode（如proj）或替代物件名稱（專案）。

有關有效ObjCode的清單，請參見  [API Explorer](../../wf-api/general/api-explorer.md).

### 作業

通過將HTTP請求發送到其唯一URI來操作對象。 要執行的操作由HTTP方法指定。

標準HTTP方法對應於下列操作：

* **GET**  — 按ID檢索對象、按查詢搜索所有對象、運行報告或執行命名查詢
* **POST**  — 插入新對象
* **PUT**  — 編輯現有對象
* **DELETE**  — 刪除對象

為了解決用戶端不足或通訊協定長度限制的問題，可使用方法參數來覆寫HTTP行為。 例如，可以通過發佈以下URI來實施GET操作：
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET/attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 個回應

每個要求都會以JSON格式提供回應。 如果請求成功，回應會有資料屬性，如果有問題，則會有錯誤屬性。 例如，請求

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

傳回類似下列的JSON回應：


<pre>{<br>    "data":[<br>        {<br>            "percentComplete":0,<br>            "status":"CUR",<br>            "優先順序":2,<br>            "name":「全新專案」，<br>            "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>透過瀏覽器的位址列執行GET要求時，不需要將sessionID納入要求中。

已針對PUT、POST和DELETE要求新增特殊安全性。 導致寫入資料庫或從資料庫刪除的任何請求只能在 **sessionID=abc123** 包含在URI中。 下列範例顯示這如何尋找DELETE請求：
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET/attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### 驗證

API驗證每個請求，以確保用戶端有權檢視或修改請求的物件。

驗證是透過傳遞工作階段ID來執行，而此ID可透過下列方法之一提供：

#### 請求標題驗證

慣用的驗證方法是傳遞包含工作階段權杖、名為SessionID的要求標題。 這有安全防範的優點 [跨網站請求偽造(CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻擊，而不會為快取目的而干擾URI。

以下是請求標題的範例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### 請求參數驗證

您可以傳遞名為sessionID的請求參數來進行驗證，如下列範例所示： 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie式驗證

API使用的Cookie式驗證與Web UI用於系統的相同。 其中，如果用戶端使用Web UI登入Workfront，從相同瀏覽器發出的任何AJAX呼叫都會使用相同的驗證。

>[!NOTE]
>
>為了防止CSRF（跨站請求偽造）攻擊的可能性，此驗證方法僅適用於唯讀操作。

## 登入

>[!IMPORTANT]
Workfront不再建議使用 `/login` 端點或API金鑰。 請改為使用下列其中一種驗證方法：
* 使用JWT進行伺服器驗證
* 使用OAuth2進行使用者驗證
>
有關設定這些驗證方法的說明，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)
如需在Workfront中使用伺服器驗證的指示，請參閱 [使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md)
如需在Workfront中使用使用者驗證的指示，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
本節所述的程式僅適用於尚未上架到Adobe業務平台的組織。 如果貴組織已上線至Workfront Business Platform，便無法透過Workfront API登入Adobe。
有關根據貴組織是否已上架到AdobeBusiness Platform而有所不同的過程清單，請參見 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

使用有效的用戶名和密碼，可以使用以下請求獲取會話ID:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

這會設定Cookie以驗證未來請求，並傳回具有新建立之sessionID、登入使用者的userID和其他工作階段屬性的JSON回應。

>[!NOTE]
如果您有指定的API使用者也是管理員，Workfront強烈建議您使用API金鑰登入。

**產生API金鑰**

以該使用者身分登入系統時，您可以產生API金鑰，如下列範例所示：


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**擷取先前產生的API金鑰**

您也可以執行getApiKey，以擷取先前為特定使用者產生的API金鑰：


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

然後，您可以新增&quot;apiKey&quot;作為請求參數並加上此值，以取代sessionID或使用者名稱及密碼，借此使用此結果來驗證任何API呼叫。 從安全形度看，這是有益的。

以下請求是使用apiKey從專案擷取資料的範例：

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**使API金鑰失效**

如果apiKey值已洩露，您可以執行「clearApiKey」，使目前的API金鑰失效，如下列範例所示：

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

清除後，您可以再次執行getApiKey以產生新的API金鑰。

### 登出

當工作階段完成時，您可以使用下列要求將使用者登出，使得使用sessionID的任何進一步存取都無法進行。

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

要登出的sessionID可指定為Cookie、要求標題或要求參數。

若要登出使用者：

1. 導覽至您的登入畫面，但不登入。
1. 將URL變更為/attask/api/v15.0/project/search。\
   請注意，找不到頁面。
1. 取代 *搜尋* 使用login?username=admin&amp;password=user ，以替換您的使用者名稱和密碼 *管理員* 和*使用者\
   *此工作階段會以Cookie形式儲存在瀏覽器中，不需要在後續的每個GET要求中重列。

1. 將URL變更回 **/attask/api/v15.0/project/search**.
1. 請注意提供的回應。

執行PUT、POST和DELETE要求時，您必須一律包含登入後提供的sessionID。

## GET行為

使用HTTPGET方法來檢索對象或多個對象並運行報告。

### 檢索對象

您可以使用修飾詞和篩選器來增強對對象的搜索。

#### 使用對象ID檢索對象

如果您知道對象的ID，則可以通過訪問對象的唯一URI來檢索該對象。 例如，請求

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

傳回類似下列的回應：

<pre>{<br>    "percentComplete":0,<br>    "status":"CUR",<br>    "優先順序":2,<br>    "name":「全新專案」，<br>    "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


您可以指定id請求參數並提供以逗號分隔的ID清單，借此擷取相同請求中的多個物件，如下列範例所示：


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

請注意， /attask/api/v15.0/project?id=...要求與 `/attask/api/v15.0/project/...` 請求。

#### 使用URI檢索對象

如果要按ID以外的條件檢索對象，則可以搜索URI。

例如，您可以使用下列請求來傳回系統中所有專案的清單：

```
GET /attask/api/v15.0/project/search
```

您可以使用請求參數來指定篩選器，做為名稱值配對。 例如，下列範例顯示可尋找所有目前專案的請求：

```
GET /attask/api/v15.0/project/search?status=CUR
```

以下請求將查找所有尚未完成的任務以及分配給名為John的用戶的任務。

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 使用搜索修飾符

下表列出您可與Workfront API搭配使用的一些修飾元。

| **修飾詞** | **說明** | **範例** |
|---|---|---|
| eq | 返回狀態為已關閉的結果 | <pre>...status=cls&amp;status_Mod=eq..</pre> |
| ne | 傳回未處於已關閉狀態的結果 | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| get | 傳回百分比完成大於或等於50的結果 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | 傳回百分比完成小於或等於50的結果 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 返回說明為Null的結果 | <pre>...description_Mod=isnull..</pre> |
| notnull | 返回說明非空的結果 | <pre>...description_Mod=notnull...</pre> |
| 包含 | 傳回名稱包含「Workfront」的結果 | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| 介於 | 傳回過去7天內具有登入日期的結果 | <pre>...entryDate=$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
搜尋請求會區分大小寫。 如果您收到錯誤，請確定  **_Mod** 和 **範圍(_R)** 大小寫正確。

#### 使用OR陳述式

您可以新增包含「OR」的參數，以及指出篩選器或一系列篩選器等級的數字，借此增強搜尋。

OR陳述式只會傳回API呼叫中符合OR陳述式篩選條件的記錄。 篩選器不會隱含在OR陳述式層級中。

例如，如果您要篩選

* 名稱包含「Planning」或
* 名為「FixedAssets」AND的產品組合中的任務，指派給名稱包含「Steve」OR的人
* 具有名為「最終任務」的父任務的任務

然後搭配其多個OR陳述式使用下列API呼叫：
<pre>GET/attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>或(&amp;O):1:portfolio:name=FixedAssets<br>或(&amp;O):1:portfolio:name_Mod=eq<br>或(&amp;O):1:assignedTo:name=Steve<br>或(&amp;O):1:assignedTo:name_Mod=cicontains<br>或(&amp;O):2:parent:name=最終任務<br>或(&amp;O):2:parent:name_Mod=eq
</pre>

#### 使用篩選參數

將URL參數用於搜尋篩選器的一個潛在陷阱是，Workfront會先剖析特定參數，再檢查不同的驗證方法（例如使用者名稱、密碼、apiKey、Cookie）。 發生此情況時，不會將參數當作呼叫中的篩選器。 

若要避免此問題，您可以將這些值放入具有JSON格式的篩選參數中。 例如，如果您要篩選使用者名稱testuser，而非使用 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>在篩選器中傳遞URL參數，如下列範例所示：
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### 使用對應請求參數

依預設，從搜尋傳回的資料是JSON陣列。 根據您的使用案例，將結果作為依ID索引的JSON物件來取得可能會更有效率。 您可以使用對應請求參數來完成此操作。 例如，請求 
<pre>/attask/api/v15.0/task/search?map=true</pre>傳回依ID索引的回應，如下所示：
<pre>{<br>    "data":{<br>        "4c9a97db0000000f13ee4446b9aead9b":{<br>            "percentComplete":0,<br>            "status":"新",<br>            "name":"第一項任務",<br>            "ID":"4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber":1 <br>        },<br>        「4ca28ba600002024cd49e75bd43cf601」：{<br>            "percentComplete":0,<br>            "status":"INP:A",<br>            "name":第二項任務，<br>            "ID":"4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber":2 <br>        } <br>    } <br>}</pre>

#### 使用欄位請求參數

依預設，擷取物件只會傳回最常使用的欄位子集。

您可以使用欄位要求參數來指定傳回的特定欄位清單（以逗號分隔）。 例如，請求
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>傳回類似下列的回應：
<pre>{<br>    "優先順序":2,<br>    "name":"第一項任務",<br>    "ID":"4c7c08fa0000002ff924e298ee148df4",<br>    "planededStartDate":"2010-08-30T09":00:00:000-0600」 <br>}</pre>

>[!NOTE]
這些欄位名稱區分大小寫。

有關可能的欄位引用的清單，請參見  [API Explorer](../../wf-api/general/api-explorer.md)

#### 搜索嵌套對象

您可以搜尋巢狀物件。 依預設，傳回的巢狀物件僅包含名稱和ID。 例如，若要取得所有問題及其擁有者，請使用下列要求：
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>如需詳細資訊，您可以使用冒號語法要求巢狀欄位。 例如，下列請求會搜尋所有問題，以及擁有者的姓名、ID、標題和電話號碼
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>並傳回下列內容： 
<pre>{<br>    "name":"重要問題",<br>    "ID":"4c78285f00000908ea8cfd66e084939f",<br>    "owner":{<br>        "title":"運營專家",<br>        "phoneNumber":《555-1234》，<br>        "name":"管理員用戶",<br>        "ID":"4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### 擷取巢狀集合

您可以擷取物件的巢狀集合。 例如，若要取得包含所有工作的專案，請使用下列請求：
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>以下請求獲取任務分配：
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 搜尋多個巢狀欄位

預設情況下，僅返回每個任務的名稱和ID，但可以使用冒號語法指定其他嵌套欄位。 若要檢視相關物件或集合的所有可用欄位，只需在物件/集合參考上附加冒號和星號。
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### 擷取自訂資料

您可以使用首碼「DE：」擷取自訂資料欄位。 例如，若要要求專案中包含「CustomText」參數，請使用下列要求：
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>會返回
<pre>{<br>    "name":"自訂資料專案",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText":"任務b" <br>}</pre>您也可以要求parameterValues欄位，以擷取物件的所有自訂資料。 例如， 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>會傳回類似於下列的資料：
<pre>{<br>    "name":"自訂資料專案",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues:{ <br>        "DE:CustomText":"任務b", <br>        "DE:CustomNumber":1.4, <br>        "DE:CustomCheckBoxs":["first"、"second"、"third"] <br>    } <br>}</pre>

#### 使用命名查詢

某些對象類型具有命名的搜索，這些搜索通常執行，通過將查詢的名稱附加到對象類型URI的末尾即可使用。 例如，下列請求會擷取使用者目前被指派到的工作項目（工作和問題）:
<pre>/attask/api/v15.0/work/myWork</pre>命名查詢支援請求欄位參數以檢索其他欄位。 有些已命名的查詢也接受其他篩選器。 如需可允許的已命名查詢物件的清單，請參閱[API Explorer](../../wf-api/general/api-explorer.md)中該物件的「動作」標籤。

#### 使用計數篩選

您可以指定指定的搜尋要傳回的結果數。 這可讓伺服器更快處理請求並節省頻寬。 例如，請求
<pre>GET/attask/api/v15.0/project/count?status=CUR</pre>以下列格式傳回結果數：
<pre>{<br>    "count":3 <br>}</pre>與傳送完整物件相比，這樣的下載量會小得多。 篩選語法與搜尋命令相同。

### 請求報表

您可以執行報表請求，其中只需要某些欄位的匯總（以一或多個群組分組）。 如下列範例所示，報表語法與SOAP API的語法相同：
<pre>GET/attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>會傳回下列結果
<pre>{<br>    「第一個項目」：{ <br>        "sum_hours":15 <br>    }, <br>     「第二個項目」：{ <br>        "sum_hours":30 <br>    } <br>}</pre>新增$$ROLLUP=true參數，包括每個分組層的總計：
<pre>{<br>    「第一個項目」：{ <br>        "sum_hours":15 <br>    }, <br>    「第二個項目」：{ <br>        "sum_hours":30 <br>    }, <br>    "$$ROLLUP":{ <br>        "sum_hours":45 <br>    } <br>}</pre>

### 在API中排序查詢結果

如果您將下列項目附加至API呼叫，則可依任何欄位來排序結果：

&amp;entryDate_Sort=asc

例如，如果要按任務計畫起始日期排序，請刪除entryDate，並將其替換為planingedCompletionDate。

這適用於Workfront的大部分欄位。

### 考慮查詢限制

查詢對象時，應特別考慮相關對象的關係和搜索限制。 例如，如下表所示，專案的查詢最多可傳回2,000個專案。 這2,000個項目被視為「主要對象」。 如果查詢項目上的「任務」欄位，則「任務」欄位（即集合）將成為主對象「項目」的輔助對象。 「任務」欄位的查詢可以包含數千個項目任務。 總計，返回的對象（項目和任務）的合計數不能超過50,000個。

為確保最佳效能，下表顯示搜尋請求所受的限制。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>查詢結果</th> 
   <th>限制</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">預設結果數</td> 
   <td>100</td> 
   <td> 如果未在查詢篩選器中指定任何限制（即$LIMIT），則結果只能包含不超過100個主對象。 <br>請參閱 <a href="#using-paginated-responses" class="MCXref xref">使用編頁回應</a> 以取得如何覆寫此限制的說明。 </td> 
  </tr> 
  <tr> 
   <td>結果的最大數量</td> 
   <td>2,000</td> 
   <td>查詢篩選器（即$LIMIT）最多可傳回2000個結果。 如需詳細資訊，請參閱「已編頁的回應」。</td> 
  </tr> 
  <tr> 
   <td>最大欄位深度</td> 
   <td>4</td> 
   <td>在標識要顯示的欄位時，不能從要查詢的對象中移出超過四個級別。</td> 
  </tr> 
  <tr> 
   <td>最大對象數</td> 
   <td>50,000</td> 
   <td>結果集不能包含50000個主對象和次對象。</td> 
  </tr> 
  <tr> 
   <td>欄位數上限</td> 
   <td nowrap>1,000,000</td> 
   <td>當結果集小於50000對象時，您的結果最多可能包含1,000,000個欄位。</td> 
  </tr> 
  <tr> 
   <td>建立/更新的批次數量上限</td> 
   <td>100</td> 
   <td>批次建立或更新上限為100。</td> 
  </tr> 
 </tbody> 
</table>

### 使用編頁回應 {#using-paginated-responses}

要覆蓋「預設結果數」查詢限制並允許200個結果，您可以包括 `$$LIMIT=200` 篩選，如下列範例所示：
<pre>GET/attask/api/v15.0/project/search?$$LIMIT=200</pre>

為確保系統中其他租戶的可靠性和效能，每個查詢允許的最大結果限制為2000個對象。 嘗試指定較大限制會導致 `IllegalArgumentException` 錯誤訊息。 

因此，建議您考慮對大型資料集使用編頁回應。 若要指定應傳回的第一個結果，請新增 `$$FIRST` 篩選。 例如，下列請求會傳回查詢的結果201-250:
<pre>GET/attask/api/v15.0/project/search?$FIRST=200&amp;$LIMIT=50</pre>

請注意，在上例中， `$$FIRST=200` 返回第201個結果。 `$$FIRST=0` 會傳回第一個結果。 將$$FIRST值視為在傳回結果之前要略過的結果數，可能會有所幫助。

若要確定結果已正確編頁，請使用排序參數。 這可讓結果以相同順序傳回，因此分頁不會重複或略過結果。 例如，若要使用物件ID來排序，請使用 `ID_Sort=asc`.

### 建立存取規則

您可以建立存取規則，以決定誰可以存取物件。 以下是您可以設定的存取規則範例：

若要設定專案，使其只與ID為「abc123」的使用者共用，請使用下列請求：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules:[ {accessorID:'abc123',accessorObjCode:'USER',coreAction:'VIEW'} ] }</pre>或者，您也只能與新人員共用，並保留現有權限：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>要檢索現有訪問規則，請執行以下操作：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST行為

POST插入新對象。 語法與PUT相同，但有一些例外。 因為新物件尚未存在，它沒有ID。 因此，URI不包含ID。

### 建立物件

以下是建立新專案的要求範例：
<pre>POST/attask/api/v15.0/project?name=新專案</pre>回應包含新建立的專案及其新ID和任何其他指定欄位。

### 複製物件

某些物件支援複製。 對於這些對象類型，可以通過使用copySourceID參數發佈來建立新對象。 例如，下列請求會複製指定的專案，並為其提供新名稱：

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### 上傳檔案

您可以透過下列API URL上傳檔案：
<pre>POST/attask/api/v15.0/upload</pre>API預期內容類型為多部分/表單資料。 檔案的參數名稱必須為uploadedFile。 伺服器會傳回下列JSON資料：
<pre>{<br>    "handle":"4c7c08fa0000002ff924e298ee148df4"<br>}</pre>建立Workfront檔案時，您可以使用控點，並將貼文至下列URL:
<pre>POST/attask/api/v15.0/document?updates={<br>    名稱：aFileName,<br>    句柄：abc...123，（從檔案上傳處理）<br>    docObjCode:PROJ 、（或TASK 、 OPTASK等）<br>    objID:abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT行為

PUT用於更新現有對象。

PUT的回應與GET相同。 在這兩種情況下，伺服器都會在更新後傳回物件的新狀態。 用來變更GET要求回應的所有規則也可搭配PUT使用，例如指定要傳回的其他欄位、自訂資料等。

### 編輯對象

對象的更新始終由ID使用對象的唯一URI完成。 要更新的欄位會指定為請求參數。 例如，若要變更專案名稱，您可以傳送類似下列的要求：
<pre>PUT/attask/api/v15.0/project/4c7...?name=新項目名稱 <br>PUT/attask/api/v15.0/project?id=4c7...&amp;name=新項目名稱</pre>由於更新需要ID，如果伺服器上不存在物件，則此操作將失敗（不插入）。

### 指定JSON編輯

如下列範例所示，您可以使用更新要求參數來指定要使用JSON語法更新的欄位：
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{<br>     名稱："新項目名稱", <br>     狀態："CUR", <br>     ... <br>}</pre>

### 進行巢狀更新

某些物件有私人擁有的集合，可供更新。 例如，以下示例演示如何覆蓋給定任務的現有分配：
<pre>PUT/attask/api/v15.0/task/4c7...?更新= <br>{<br>    分配：[ <br>        { <br>            assignedToID:"2222...54d0, <br>            assignmentPercent:50.0 <br>        },{ <br>            roleID:「111...54d0」<br>        } <br>    ] <br>}</pre>

>[!NOTE]
雖然對頂層進行的更新是稀疏的，但對集合或巢狀物件的更新會完全取代現有的集合。 要在不影響對象的情況下編輯任務上的單個分配，請對分配使用PUT，而不是對任務使用。

下面的示例將項目設為公共服務台隊列。 請注意，現有隊列屬性將被替換。
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{ <br>    queueDef:{ <br>        isPublic:1 <br>    } <br>}</pre>

### 使用動作要求參數

有些物件支援除了簡單編輯以外可執行的其他動作。 您可以使用動作請求參數來指定這些動作。 例如，下列請求會重新計算指定專案的時間軸：
<pre>PUT/attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>或<br><br>PUT/attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### 移動對象

以下示範將任務從一個項目移動到另一個項目的語法：
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>以下提供每個動作類型的範例：(??)
<pre>PUT/attask/api/v15.0/project/1234/approveApproval<br><br>PUT/attask/api/v15.0/project/1234/calculateFinance<br><br>PUT/attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT/attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT/attask/api/v15.0/project/1234/recallApproval<br><br>PUT/attask/api/v15.0/project/1234/rejectApproval<br><br>PUT/attask/api/v15.0/task/1234/move<br><br>PUT/attask/api/v15.0/workitem/1234/markViewed</pre>只有移動操作需要標識附加屬性，以指定要移動工作項的項目。

以下是每個動作類型的範例： 
<pre>PUT/attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID:'abc123',accessorObjCode:'USER',coreAction:'VIEW'}]}</pre>

### 共用對象

下列範例示範與團隊共用專案的語法：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>編輯物件時，您可以執行類似下列範例的PUT並傳送更新，以取代物件上的所有存取規則：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]</pre>以下示例顯示了將任務從一個項目移動到另一個項目的語法：
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE行為

DELETE移除物件。 在每種情況下，URI都可能包含參數force=true ，以使伺服器刪除指定的資料及其受屬者。 在以下示例中，通過在URI上執行HTTPDELETE方法來刪除任務：
<pre>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## 大量更新

大量更新陳述式會在單一API呼叫中同時更新多個物件。 大量建立API呼叫的建置方式與一般更新呼叫類似，如下列範例所示：
<pre>PUT/attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>會產生類似下列的傳回：
<pre>資料：[{<br>    ID:"53ff8d3d003b438b57a8a784df38f6b3",<br>    名稱："Test_Project_1",<br>    objCode:"PROJ",<br>    percentComplete:0,<br>    planedCompletionDate:"2014-08-28T11":00:00:000-0400」，<br>    planedStartDate:"2014-08-28T11":00:00:000-0400」，<br>    優先順序：0,<br>    projectedCompletionDate:"2014-08-28T16":12:00:000-0400」，<br>    狀態："CUR"<br>},<br>{<br>    ID:"53ff8d49003b43a2562aa34eea3b6b10",<br>    名稱："Test_Project_2",<br>    objCode:"PROJ",<br>    percentComplete:0usi,<br>    planedCompletionDate:"2014-08-28T11":00:00:000-0400」，<br>    planedStartDate:"2014-08-28T11":00:00:000-0400」，<br>    優先順序：0,<br>    projectedCompletionDate:"2014-08-28T16":12:00:000-0400」，<br>    狀態："CUR"<br>}]</pre>您也可以執行類似下列的大量更新：
<pre>PUT/attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}&amp;apiKey=123axxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>會產生類似下列的傳回：
<pre>資料：[ {<br>     ID:"53ff8e15003b461d4560f7f65a440078",<br>     名稱："Test_Project_1_Edit",<br>     objCode:"PROJ",<br>     percentComplete:0,<br>     planedCompletionDate:"2014-08-28T11":00:00:000-0400」，<br>     planedStartDate:"2014-08-28T11":00:00:000-0400」，<br>     優先順序：0,<br>     projectedCompletionDate:"2014-08-28T16":16:00:000-0400」，<br>     狀態："CUR"<br>},<br>{<br>    ID:"53ff8e19003b46238a58d303608de502",<br>    名稱："Test_Project_2_Edit",<br>    objCode:"PROJ",<br>    percentComplete:0,<br>    planedCompletionDate:"2014-08-28T11":00:00:000-0400」，<br>    planedStartDate:"2014-08-28T11":00:00:000-0400」，<br>    優先順序：0,<br>    projectedCompletionDate:"2014-08-28T16":16:00:000-0400」，<br>    狀態："CUR"<br>}]</pre>如果您希望所有操作都在相同的交易中執行，請將"atomic=true"新增至批次API呼叫，作為請求參數。 這樣，如果任何操作失敗，則所有操作都將回退。

>[!NOTE]
原子批處理操作只能返回「成功：true」或錯誤。
