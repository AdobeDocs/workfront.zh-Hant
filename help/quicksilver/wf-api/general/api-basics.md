---
content-type: api
navigation-topic: general-api
title: API 基本概念
description: API 基本概念
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 362a14c2c25e995d06a26b77ab51448b033bc2ac
workflow-type: tm+mt
source-wordcount: '4361'
ht-degree: 0%

---


# API 基本概念

Adobe Workfront API的目標是透過引入透過HTTP運作的REST-ful架構，簡化與Workfront的整合的建置。 本檔案假設您熟悉REST和JSON回應，並說明Workfront API所採取的方法。

熟悉Workfront結構描述有助於您瞭解可用來從Workfront中提取資料以進行整合的資料庫關係。

## 限制和准則

為確保一致的Workfront隨選系統效能，每個客戶限製為10個同時的API執行緒。 沙箱環境有相同的限制，可讓客戶和合作夥伴在將程式碼發佈到生產環境之前準確測試API呼叫。

在生產、預覽和測試磁碟環境中，一般使用者請求的URI長度上限為8892個位元組，因為它們是透過Workfront CDN (Akamai)路由傳送。 此限制僅適用於透過CDN路由的URI。

>[!NOTE]
>
>此限制不適用於沙箱環境，因為沙箱環境不會透過CDN路由。

### 免責宣告

任何使用API的情況都應先在Workfront測試版環境中進行測試，然後才能在生產環境中執行。 如果有任何客戶將API用于某項流程，而Workfront合理地認為該流程會對隨選軟體造成負擔（也就是說，該流程會對其他客戶的軟體效能造成重大負面影響），Workfront將保留請求客戶停止該流程的權利。 如果客戶沒有遵守規定，且問題仍然存在，Workfront保留終止程式的權利。

## REST基本概念

本節簡要介紹如何與下列REST原則的Workfront REST API互動：

### 物件URI

系統中的每個物件都會獲得一個獨一無二的URI，由物件型別和ID組成。 下列範例顯示描述三個唯一物件的URI：

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

物件型別不區分大小寫，可以是縮寫的ObjCode （例如proj）或替代物件名稱（專案）。

如需有效ObjCode的清單，請參閱  [API總管](../../wf-api/general/api-explorer.md).

### 營運

透過傳送HTTP請求至物件的唯一URI來控制物件。 要執行的作業會由HTTP方法指定。

標準HTTP方法會對應至下列作業：

* **GET**  — 依ID擷取物件、依查詢搜尋所有物件、執行報表或執行具名查詢
* **POST**  — 插入新物件
* **PUT**  — 編輯現有物件
* **DELETE**  — 刪除物件

為了解決使用者端缺陷或通訊協定長度限制，可以使用方法引數覆寫HTTP行為。 例如，可藉由張貼下列URI來實作GET作業：
<pre>GET/attask/api/v15.0/project？id=4c78...54d0&amp;method=get<br>GET/attask/api/v15.0/project/4c78...54d0？method=get</pre>

### 回應

每個要求都會有JSON格式的回應。 如果要求成功，回應會具有資料屬性，如果有問題，則會具有錯誤屬性。 例如，請求

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

會傳回類似下列的JSON回應：


<pre>{<br>    "data"： [<br>        {<br>            "percentComplete"： 0，<br>            "status"： "CUR"，<br>            "priority"： 2，<br>            "name"： "Brand New Project"，<br>            "ID"： "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>透過瀏覽器的位址列執行GET要求時，不需要將sessionID納入要求的一部分。

已針對PUT、POST和DELETE請求新增特殊安全性。 任何導致寫入資料庫或從資料庫刪除的要求只能在 **sessionID=abc123** 包含在URI中。 下列範例說明這會如何尋找DELETE請求：
<pre>GET/attask/api/v15.0/project？id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET/attask/api/v15.0/project/4c78...54d0？method=delete&amp;sessionID=abc123</pre>

### 驗證

API會驗證每個請求，以確保使用者端有權檢視或修改請求的物件。

透過傳入工作階段ID來執行驗證，該ID可使用以下方法之一指定：

#### 請求標頭驗證

首選的驗證方法是傳遞包含工作階段權杖的名為SessionID的請求標頭。 其優點是可以安全抵禦 [跨網站請求偽造(CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻擊且不干擾URI以進行快取。

以下是請求標頭的範例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### 要求引數驗證

您可以傳遞名為sessionID的請求引數來進行身分驗證，如下列範例所示： 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie型驗證

此API使用的是Web UI用於系統的相同基於Cookie的驗證。 其中，如果使用者端使用網頁UI登入Workfront，則從相同瀏覽器內進行的任何AJAX呼叫都會使用相同的驗證。

>[!NOTE]
>
>為了防止CSRF （跨網站請求偽造）攻擊的可能性，此驗證方法僅適用於唯讀操作。

## 登入

>[!IMPORTANT]
>
Workfront不再建議使用 `/login` 端點或API金鑰。 請改用下列其中一種驗證方法：
>
* 使用JWT進行伺服器驗證
* 使用OAuth2進行使用者驗證
>
如需設定這些驗證方法的說明，請參閱 [為Workfront整合建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
如需在Workfront中使用伺服器驗證的指示，請參閱 [使用JWT流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md)
>
如需在Workfront中使用使用者驗證的指示，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
本節所述的程式僅適用於尚未加入「Adobe業務平台」的組織。 如果您的組織已加入Adobe Business Platform，就無法透過Workfront API登入Workfront。
>
如需根據貴組織是否已加入Adobe Business Platform而有所差異的程式清單，請參閱 [平台型管理差異(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

使用有效的使用者名稱和密碼，您可以使用以下要求來取得工作階段ID：

```
POST /attask/api/v15.0/login?username=admin&password=user
```

這樣會設定Cookie以驗證未來的請求，並傳回JSON回應，其中包含新建立的sessionID、登入使用者的使用者ID以及其他工作階段屬性。

>[!NOTE]
>
如果您有同時身為管理員的指定API使用者，Workfront強烈建議您使用API金鑰來登入。

**產生API金鑰**

您可以以該使用者身分登入系統時產生API金鑰，如下列範例所示：


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**擷取先前產生的API金鑰**

您也可以執行getApiKey，擷取先前為特定使用者產生的API金鑰：


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

然後，您可以使用此結果，新增「apiKey」作為請求引數，取代工作階段ID或使用者名稱和密碼，以驗證任何API呼叫。 從安全性角度來看，這是有好處的。

以下請求為使用apiKey從專案擷取資料的範例：

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**使API金鑰失效**

如果apiKey值已洩漏，您可以執行「clearApiKey」，讓目前的API金鑰失效，如下列範例所示：

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

清除後，您可以再次執行getApiKey以產生新的API金鑰。

### 登出

工作階段完成時，您可以使用以下請求將使用者登出，防止任何使用sessionID的進一步存取。

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

要登出的sessionID可指定為Cookie、請求標頭或請求引數。

登出使用者：

1. 導覽至您的登入畫面，但不登入。
1. 將URL變更為/attask/api/v15.0/project/search。\
   請注意，找不到該頁面。
1. 取代單字 *搜尋* 使用login？username=admin&amp;password=user，將您的使用者名稱和密碼替換為 *管理員* 和*user\
   *此工作階段會以Cookie形式儲存在瀏覽器中，不需要在後續每個GET要求中重新陳述。

1. 將URL變更回 **/attask/api/v15.0/project/search**.
1. 請注意提供的回應。

執行PUT、POST和DELETE要求時，您必須一律包含登入後提供的sessionID。

## GET行為

使用HTTPGET方法擷取一或多個物件，並執行報表。

### 正在擷取物件

您可以使用修飾詞和篩選器來增強物件的搜尋。

#### 使用物件識別碼擷取物件

如果您知道物件的ID，可以存取物件的唯一URI來擷取該物件。 例如，請求

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

會傳回類似下列的回應：

<pre>{<br>    "percentComplete"： 0，<br>    "status"： "CUR"，<br>    "priority"： 2，<br>    "name"： "Brand New Project"，<br>    "ID"： "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


您可以指定id請求引數，並提供ID清單（以逗號分隔），在相同請求中擷取多個物件，如下列範例所示：


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

請注意/attask/api/v15.0/project？id=...要求與 `/attask/api/v15.0/project/...` 要求。

#### 使用URI擷取物件

如果您想要依據ID以外的條件擷取物件，則可搜尋URI。

例如，您可以使用以下請求來傳回系統中所有專案的清單：

```
GET /attask/api/v15.0/project/search
```

您可以使用要求引數做為名稱 — 值組來指定篩選器。 例如，下列範例顯示會尋找所有目前專案的要求：

```
GET /attask/api/v15.0/project/search?status=CUR
```

以下請求會尋找所有尚未完成的工作，以及指派給名為John的使用者的工作。

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 使用搜尋修飾元

下表列出您可以搭配Workfront API使用的一些修飾元。

| **修飾元** | **說明** | **範例** |
|---|---|---|
| eq | 傳回狀態為「已關閉」的結果 | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| 新 | 傳回不處於「已關閉」狀態的結果 | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | 傳回完成百分比大於或等於50的結果 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | 傳回完成百分比小於或等於50的結果 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 傳回說明為空的結果 | <pre>...description_Mod=isnull...</pre> |
| notnull | 傳回說明不是Null的結果 | <pre>...description_Mod=notnull...</pre> |
| 包含 | 傳回名稱包含「Workfront」的結果 | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| 介於 | 傳回其輸入日期在過去7天內的結果 | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
搜尋要求會區分大小寫。 如果收到錯誤，請確定  **修改(_M)** 和 **範圍(_R)** 大小寫正確。

#### 使用OR陳述式

您可以新增包含「OR」的引數，以及數字來指示篩選或一系列篩選的層級，藉此增強搜尋。

OR陳述式只會傳回API呼叫中符合OR陳述式篩選條件的記錄。 OR陳述式層級不會隱含篩選器。

例如，如果您要篩選

* 名稱包含「Planning」或
* 名為「FixedAssets」的投資組合中的任務，以及指派給名稱包含「Steve」OR之人員的任務
* 具有名為「最終任務」之父系任務的任務

然後搭配使用下列API呼叫的多個OR陳述式：
<pre>GET/attask/api/v15.0/task/search？name=Planning<br>&amp;name_Mod=contains<br>或(&amp;O):1:portfolio：name=FixedAssets<br>或(&amp;O):1:portfolio：name_Mod=eq<br>或(&amp;O):1:assignedTo：name=Steve<br>或(&amp;O):1:assignedTo：name_Mod=cicontains<br>或(&amp;O):2:parent：name=最終任務<br>或(&amp;O):2:parent：name_Mod=eq
</pre>

#### 使用篩選器引數

將URL引數用於搜尋篩選的一個潛在陷阱是Workfront會先剖析某些引數，再檢查是否有不同的驗證方法（即使用者名稱、密碼、apiKey、Cookie）。 發生此情況時，引數不會作為呼叫中的篩選器。 

若要避免此問題，您可以將這些值放入具有JSON格式的篩選引數中。 例如，如果您想篩選使用者名稱testuser，而不是使用 
<pre>/attask/api/v15.0/user/search？username=testuser@workfront.com</pre>在篩選器中傳遞URL引數，如下列範例所示：
<pre>/attask/api/v15.0/user/search？filters={"username"："testuser@workfront.com"}</pre>

#### 使用對應要求引數

依預設，從搜尋傳回的資料為JSON陣列。 根據您的使用案例，以JSON物件格式依ID編制索引可能更有效率。 使用對應要求引數即可完成這項操作。 例如，請求 
<pre>/attask/api/v15.0/task/search？map=true</pre>傳回依ID編制索引的回應，如下所示：
<pre>{<br>    "data"： {<br>        「4c9a97db0000000f13ee4446b9aead9b」： {<br>            "percentComplete"： 0，<br>            "status"： "NEW"，<br>            "name"： "first task"，<br>            "ID"： "4c9a97db0000000f13ee4446b9aead9b"，<br>            "taskNumber"： 1 <br>        }，<br>        "4ca28ba600002024cd49e75bd43cf601"： {<br>            "percentComplete"： 0，<br>            "status"： "INP：A"，<br>            "name"： "second task"，<br>            "ID"： "4ca28ba600002024cd49e75bd43cf601"，<br>            "taskNumber"：2 <br>        } <br>    } <br>}</pre>

#### 使用欄位請求引數

依預設，擷取物件只會傳回最常用的欄位子集。

您可以使用欄位請求引數，指定傳回之特定欄位的逗號分隔清單。 例如，請求
<pre>/attask/api/v15.0/task/search？fields=plannedStartDate，priority</pre>會傳回類似下列的回應：
<pre>{<br>    "priority"： 2，<br>    "name"： "first task"，<br>    "ID"： "4c7c08fa0000002ff924e298ee148df4"，<br>    "plannedStartDate"： "2010-08-30T09:00:00:000-0600英吋 <br>}</pre>

>[!NOTE]
>
這些欄位名稱會區分大小寫。

如需可能的欄位參考清單，請參閱  [API總管](../../wf-api/general/api-explorer.md)

#### 搜尋巢狀物件

您可以搜尋巢狀物件。 依預設，巢狀物件只傳回名稱和ID。 例如，若要與擁有者取得所有問題，請使用以下請求：
<pre>/attask/api/v15.0/issue/search？fields=owner</pre>如需詳細資訊，您可以使用冒號語法來要求巢狀欄位。 例如，以下請求會搜尋所有問題以及擁有者的名稱、ID、職稱和電話號碼
<pre>/attask/api/v15.0/issue/search？fields=owner：title，owner：phoneNumber</pre>並傳回下列專案： 
<pre>{<br>    "name"： "an important issue"，<br>    "ID"： "4c78285f00000908ea8cfd66e084939f"，<br>    "owner"： {<br>        "title"： "Operations Specialist"，<br>        "phoneNumber"： "555-1234"，<br>        "name"： "Admin User"，<br>        "ID"： "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### 正在擷取巢狀集合

您可以擷取巢狀物件集合。 例如，若要取得包含其所有任務的專案，請使用以下請求：
<pre>/attask/api/v15.0/project/search？fields=tasks</pre>以下請求會取得任務指派：
<pre>/attask/api/v15.0/task/search？fields=assignments</pre>

#### 搜尋多個巢狀欄位

依預設，僅會傳回每個工作的名稱和ID，但可以使用冒號語法指定其他巢狀欄位。 若要檢視相關物件或集合的所有可用欄位，只需在物件/集合參考中附加冒號和星號即可。
<pre>/attask/api/v15.0/task/search？fields=assignments：*</pre>

#### 擷取自訂資料

您可以使用前置詞「DE：」來擷取自訂資料欄位。 例如，若要使用名為「CustomText」的引數請求專案，請使用以下請求：
<pre>/attask/api/v15.0/project/search？fields=DE：CustomText</pre>會傳回
<pre>{<br>    "name"： "custom data project"，<br>    "ID"： "4c9a954f0000001afad0687d7b1b4e43"，<br>    "DE：CustomText"： "任務b" <br>}</pre>您也可以請求parameterValues欄位，擷取物件的所有自訂資料。 例如， 
<pre>/attask/api/v15.0/project/search？fields=parameterValues</pre>傳回類似資料如下：
<pre>{<br>    "name"： "custom data project"，<br>    "ID"： "4c9a954f0000001afad0687d7b1b4e43"，<br>    parameterValues： { <br>        "DE：CustomText"： "task b"， <br>        "DE：CustomNumber"： 1.4， <br>        "DE：CustomCheckBoxes"： ["first"， "second"， "third"] <br>    } <br>}</pre>

#### 使用具名查詢

某些物件型別已命名搜尋，通常會執行，而且可將查詢名稱附加至物件型別URI的結尾來使用。 例如，以下請求會擷取使用者目前被指派的工作專案（任務和問題）：
<pre>/attask/api/v15.0/work/myWork</pre>具名查詢支援請求欄位引數以擷取其他欄位。 某些具名查詢也接受其他篩選器。 如需物件中允許的命名查詢清單，請參閱[API總管](../../wf-api/general/api-explorer.md)中物件的「動作」標籤。

#### 使用 `Count`

您可以使用 `count` 以傳回符合您查詢的結果數目。 當您不需要結果中的資料時，這會很有用。 只傳回計數，伺服器就能更快速地處理請求，並節省頻寬。 例如，請求
<pre>GET/attask/api/v15.0/project/count？status=CUR</pre>傳回以下格式的結果數：
<pre>{<br>    "count"： 3 <br>}</pre>傳回計數比傳回完整物件的資料傳輸小得多。 語法與search指令相同。

### 請求報告

您可以執行報表請求，其中一個或多個分組只需要某些欄位的彙總。 如以下範例所示，報表語法與SOAP API的語法相同：
<pre>GET/attask/api/v15.0/hour/report？project：name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>會傳回下列結果
<pre>{<br>    「第一個專案」： { <br>        "sum_hours"：15個 <br>    }， <br>     「第二個專案」： { <br>        "sum_hours"：30 <br>    } <br>}</pre>新增$$ROLLUP=true引數會在每個群組層級包含總計：
<pre>{<br>    「第一個專案」： { <br>        "sum_hours"：15個 <br>    }， <br>    「第二個專案」： { <br>        "sum_hours"：30 <br>    }， <br>    "$$ROLLUP"： { <br>        "sum_hours"：45 <br>    } <br>}</pre>

### 排序API中的查詢結果

如果您將以下內容附加至API呼叫，則可以根據任何欄位來排序結果：

&amp;entryDate_Sort=asc

例如，如果您要依任務計劃開始日期排序，請移除entryDate並將其取代為plannedCompletionDate。

這適用於Workfront中的大部分欄位。

### 考慮查詢限制

查詢物件時，應特別注意相關物件的關係和搜尋限制。 例如，如下表所示，專案查詢最多可傳回2,000個專案。 這2,000個專案會視為「主要物件」。 如果您在專案上查詢「任務」欄位，則作為集合的「任務」欄位會成為主要物件「專案」的次要物件。 「任務」欄位的查詢可包含專案中的數千個任務。 傳回的物件（專案和任務）組合總數不能超過50,000個的上限。

為確保最佳效能，下表顯示對搜尋要求的限制。 

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
   <td> 如果在查詢篩選條件中未指定限制（即$$LIMIT），則結果可包含不超過100個主要物件。 <br>另請參閱 <a href="#using-paginated-responses" class="MCXref xref">使用分頁回應</a> 以取得如何覆寫此限制的指示。 </td> 
  </tr> 
  <tr> 
   <td>結果數量上限</td> 
   <td>2,000</td> 
   <td>查詢篩選器（即$$LIMIT）最多只能傳回2000個結果。 如需詳細資訊，請參閱「分頁回應」。</td> 
  </tr> 
  <tr> 
   <td>最大欄位深度</td> 
   <td>4</td> 
   <td>識別您要顯示的欄位時，您不可離開查詢的物件超過四個層級。</td> 
  </tr> 
  <tr> 
   <td>物件最大數量</td> 
   <td>50,000</td> 
   <td>結果集不能包含50000要和次要物件。</td> 
  </tr> 
  <tr> 
   <td>最大欄位數</td> 
   <td nowrap>1,000,000</td> 
   <td>當結果集少於50000個物件時，您的結果可能最多包含1,000,000個欄位。</td> 
  </tr> 
  <tr> 
   <td>批次建立/更新的最大數量</td> 
   <td>100</td> 
   <td>最大批次建立或更新限製為100。</td> 
  </tr> 
 </tbody> 
</table>

### 使用分頁回應 {#using-paginated-responses}

若要覆寫「預設結果數」查詢限制並允許200個結果，您可以包括 `$$LIMIT=200` 在查詢中篩選，如下列範例所示：
<pre>GET/attask/api/v15.0/project/search？$$LIMIT=200</pre>

為確保系統中其他租使用者的可靠性和效能，每個查詢允許的結果限制上限為2000個物件。 嘗試指定較大的限制將導致 `IllegalArgumentException` 錯誤訊息。 

因此，我們建議您針對大型資料集使用分頁回應。 若要指定應傳回的第一個結果，請新增 `$$FIRST` 篩選。 例如，下列要求會針對查詢傳回結果201-250：
<pre>GET/attask/api/v15.0/project/search？$$FIRST=200&amp;$$LIMIT=50</pre>

請注意，在上述範例中， `$$FIRST=200` 傳回第201個結果。 `$$FIRST=0` 會傳回第一個結果。 將$$FIRST值視為在傳回結果之前要略過的結果數可能會有所幫助。

為確保結果正確分頁，請使用排序引數。 如此可讓結果以相同順序傳回，因此分頁不會重複或略過結果。 例如，若要使用物件ID排序，請使用 `ID_Sort=asc`.

### 建立存取規則

您可以建立存取規則，以決定誰可以存取物件。 以下是您可以設定的存取規則範例：

若要設定專案，使其僅與ID為「abc123」的使用者共用，請使用以下請求：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx？method=put &amp;updates={ accessRules： [ {accessorID： 'abc123'， accessorObjCode： 'USER'， coreAction： 'VIEW'} ] }</pre>或者，若只要與新使用者共用，並保持現有許可權不變：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxx/share？method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>若要擷取現有的存取規則：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx？fields=accessRules：*</pre>

## POST行為

POST插入新物件。 語法與PUT相同，但有一些例外。 因為新物件尚未存在，所以它沒有ID。 因此，URI不包含ID。

### 建立物件

以下是建立新專案的請求範例：
<pre>POST/attask/api/v15.0/project？name=New Project</pre>回應包括新建立的專案及其新ID和任何其他指定欄位。

### 複製物件

有些物件支援複製。 對於這些物件型別，可以使用copySourceID引數張貼來建立新物件。 例如，以下請求會複製指定的專案，並賦予專案新名稱：

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### 正在上傳檔案

您可以透過下列API URL上傳檔案：
<pre>POST/attask/api/v15.0/upload</pre>API預期內容型別為多部分/表單資料。 檔案的引數名稱必須是uploadedFile。 伺服器會傳回下列JSON資料：
<pre>{<br>    "handle"： "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>建立Workfront檔案時，您可以使用控制代碼並張貼至下列URL：
<pre>POST/attask/api/v15.0/document？updates={<br>    名稱： aFileName，<br>    控制代碼： abc...123， （來自檔案上傳的控制代碼）<br>    docObjCode： PROJ （或TASK、OPTASK等）<br>    物件ID： abc...123，<br>    currentVersion：{version：v1.0，fileName：aFileName}<br>}</pre>

## PUT行為

PUT可用來更新現有的物件。

PUT的回應與GET相同。 在這兩種情況下，伺服器都會在更新後傳回物件的新狀態。 所有用於變更對GET請求的回應的規則也可與PUT搭配使用，例如指定要傳回的其他欄位、自訂資料等。

### 編輯物件

物件的更新一律會使用物件的唯一URI依ID完成。 要更新的欄位會指定為請求引數。 例如，若要變更專案名稱，您可以傳送類似下列的請求：
<pre>PUT/attask/api/v15.0/project/4c7...？name=新專案名稱 <br>PUT/attask/api/v15.0/project？id=4c7...&amp;name=新專案名稱</pre>由於更新需要ID，如果伺服器上不存在物件，此操作將失敗（不插入）。

### 指定JSON編輯

如以下範例所示，您可以使用更新請求引數，指定使用JSON語法要更新的欄位：
<pre>PUT/attask/api/v15.0/project/4c7...？更新= <br>{<br>     名稱：「新專案名稱」， <br>     狀態： "CUR"， <br>     ... <br>}</pre>

### 進行巢狀更新

有些物件擁有可以更新的私人擁有集合。 例如，下列範例示範如何覆寫指定任務的現有指派：
<pre>PUT/attask/api/v15.0/task/4c7...？更新= <br>{<br>    指定任務：[ <br>        { <br>            assignedToID： "2222...54d0， <br>            assignmentPercent： 50.0 <br>        }，{ <br>            roleID： "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
雖然對最上層所做的更新是稀疏的，但對集合或巢狀物件的更新會完全取代現有的集合。 若要編輯任務的單一工作分派而不影響物件，請在工作分派上使用PUT，而不是在任務上使用。

下列範例會將專案設為公開服務檯佇列。 請注意，現有的佇列屬性會被取代。
<pre>PUT/attask/api/v15.0/project/4c7...？更新= <br>{ <br>    queueDef： { <br>        isPublic： 1 <br>    } <br>}</pre>

### 使用動作要求引數

某些物件支援除了簡單編輯外可以執行的其他動作。 您可以使用動作要求引數指定這些動作。 例如，下列請求會重新計算指定專案的時間表：
<pre>PUT/attask/api/v15.0/project/4c7...？action=calculateTimeline<br><br>或<br><br>PUT/attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### 移動物件

以下示範將任務從一個專案移動到另一個專案的語法：
<pre>PUT/attask/api/v15.0/task/4c7.../move？projectID=5d8...</pre>每種動作型別的範例如下： (??)
<pre>PUT/attask/api/v15.0/project/1234/approveApproval<br><br>PUT/attask/api/v15.0/project/1234/calculateFinance<br><br>PUT/attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT/attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT/attask/api/v15.0/project/1234/recallApproval<br><br>PUT/attask/api/v15.0/project/1234/rejectApproval<br><br>PUT/attask/api/v15.0/task/1234/move<br><br>PUT/attask/api/v15.0/workitem/1234/markViewed</pre>只有移動動作需要識別其他屬性，以指定要移動工作專案的專案。

以下是每種動作型別的範例： 
<pre>PUT/attask/api/v15.0/project/1234？method=put&amp;updates={accessRules：[{accessorID： 'abc123'， accessorObjCode： 'USER'， coreAction： 'VIEW'}]}</pre>

### 共用物件

下列範例示範與團隊共用專案的語法：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx/share？accessorID=123abcxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>編輯物件時，您可以執行PUT並傳送類似以下範例的更新，以取代物件上的所有存取規則：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx？method=PUT&amp;updates={accessRules：[{accessorID：'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx'，accessorObjCode：'TEAMOB'，coreAction：'VIEW'}]</pre>下列範例顯示將任務從一個專案移動到另一個專案的語法：
<pre>PUT/attask/api/v15.0/task/4c7.../move？projectID=5d8...</pre>

## DELETE行為

DELETE會移除物件。 在任何情況下，URI都可以包含引數force=true ，以讓伺服器移除指定的資料及其相依專案。 在以下範例中，會藉由在URI上執行HTTPDELETE方法來刪除工作：
<pre>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task？id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0？force=true <br>DELETE/attask/api/v15.0/task？id=4c78821c0000d6fa8d5e52f07a1d54d0？force=true</pre>

## 大量更新

大量更新陳述式會在單一API呼叫中同時更新多個物件。 大量建立API呼叫的建置方式與一般更新呼叫類似，如下列範例所示：
<pre>PUT/attask/api/v15.0/proj？updates=[{"name"："Test_Project_1"}，{"name"："Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>會傳回類似下列的內容：
<pre>資料： [{<br>    ID： "53ff8d3d003b438b57a8a784df38f6b3"，<br>    名稱： "Test_Project_1"，<br>    物件代碼： "PROJ"，<br>    percentComplete： 0，<br>    plannedCompletionDate： "2014-08-28T11:00:00:000-0400英吋，<br>    plannedStartDate： "2014-08-28T11:00:00:000-0400英吋，<br>    優先順序： 0，<br>    projectedCompletionDate： "2014-08-28T16:12:00:000-0400英吋，<br>    狀態： "CUR"<br>}，<br>{<br>    ID： "53ff8d49003b43a2562aa34eea3b6b10"，<br>    名稱： "Test_Project_2"，<br>    物件代碼： "PROJ"，<br>    percentComplete： 0usi，<br>    plannedCompletionDate： "2014-08-28T11:00:00:000-0400英吋，<br>    plannedStartDate： "2014-08-28T11:00:00:000-0400英吋，<br>    優先順序： 0，<br>    projectedCompletionDate： "2014-08-28T16:12:00:000-0400英吋，<br>    狀態： "CUR"<br>}]</pre>您也可以進行類似下列的大量更新：
<pre>PUT/attask/api/v15.0/proj？Umethod=PUT&amp;updates=[{"ID"："123abcxxxxxxxxxxxxxxxxxxxxxxxxxx"，"name"："Test_Project_1_ Edit"}，{"ID"："123abcxxxxxxxxxxxxxxxxxxxxxxxxxx"，"name"："Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>會傳回類似下列的內容：
<pre>資料： [ {<br>     ID： "53ff8e15003b461d4560f7f65a440078"，<br>     名稱：「Test_Project_1_Edit」，<br>     物件代碼： "PROJ"，<br>     percentComplete： 0，<br>     plannedCompletionDate： "2014-08-28T11:00:00:000-0400英吋，<br>     plannedStartDate： "2014-08-28T11:00:00:000-0400英吋，<br>     優先順序： 0，<br>     projectedCompletionDate： "2014-08-28T16:16:00:000-0400英吋，<br>     狀態： "CUR"<br>}，<br>{<br>    ID： "53ff8e19003b46238a58d303608de502"，<br>    名稱：「Test_Project_2_Edit」，<br>    物件代碼： "PROJ"，<br>    percentComplete： 0，<br>    plannedCompletionDate： "2014-08-28T11:00:00:000-0400英吋，<br>    plannedStartDate： "2014-08-28T11:00:00:000-0400英吋，<br>    優先順序： 0，<br>    projectedCompletionDate： "2014-08-28T16:16:00:000-0400英吋，<br>    狀態： "CUR"<br>}]</pre>如果您希望所有作業都發生在相同交易中，請將"atomic=true"新增至批次API呼叫，作為請求引數。 如此一來，如果有任何作業失敗，所有作業都會回覆。

>[!NOTE]
>
原子批次作業只能傳回「success： true」或錯誤。
