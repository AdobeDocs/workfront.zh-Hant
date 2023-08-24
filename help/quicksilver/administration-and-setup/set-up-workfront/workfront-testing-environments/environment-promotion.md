---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 將物件從一個環境移動到另一個環境
description: 「環境升級」功能的目的是提供與組態相關的物件從一個環境移動到另一個環境的功能。 不支援移動異動物件的功能（只有少數例外）。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 5d3c8e3626dabf88394bd6b3c2dd48e6168b56c4
workflow-type: tm+mt
source-wordcount: '2325'
ht-degree: 2%

---

# 將物件從其中移動 [!DNL Workfront] 環境至另一個環境

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 計劃</td> 
   <td> <p>Enterprise、Prime或Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 授權</p> </td> 
   <td> <p>[！UICONTROL計畫] </p> <p>您必須是 [!DNL Workfront] 管理員。 有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">物件許可權</p> </td> 
   <td> <p>全部</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支援套件</td> 
   <td> <p>[！UICONTROL Plus]、[！UICONTROL Preferred]或[！UICONTROL Enterprise]</p> <p>標準支援套件無法存取「自訂重新整理沙箱」，但可存取「預覽沙箱」。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

「建立促銷活動套件」端點會假設您已設定來源環境。 此API呼叫需要手動建立 [!DNL Workfront] 物件程式碼和物件GUID。 此地圖的特定結構如下所述。

## 環境推進的支援物件

「環境升級」功能的目的是提供與組態相關的物件從一個環境移動到另一個環境的功能。 不支援移動異動物件的功能（只有少數例外）。

* [工作物件](#work-objects)
* [報表物件](#reporting-objects)
* [自訂資料物件](#custom-data-objects)
* [組織物件](#organization-objects)
* [其他組態物件](#other-configuration-objects)


### 工作物件

| 可升級的物件 | 包含的可升級子物件 |
| --- | --- |
| 專案（專案） | 專案<br>任務<br>指定任務<br>前置任務<br>公司<br>覆寫率<br>群組<br>角色<br>團隊<br>核准流程<br>核准路徑<br>核准步驟<br>步驟核准者<br>排程<br>非工作日<br>佇列定義<br>佇列主題群組<br>佇列主題<br>路由規則<br>里程碑路徑<br>里程碑<br>小時型別<br>資源集區<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |
| 範本(TMPL) | 範本<br>範本任務<br>範本任務指派<br>範本任務前置任務<br>公司<br>覆寫率<br>群組<br>角色<br>團隊<br>核准流程<br>核准路徑<br>核准步驟<br>步驟核准者<br>排程<br>非工作日<br>佇列定義<br>佇列主題群組<br>佇列主題<br>路由規則<br>里程碑路徑<br>里程碑<br>小時型別<br>資源集區<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |

### 報表物件

| 可升級的物件 | 包含的可升級子物件 |
| --- | --- |
| 版面配置範本(UITMPL) | 版面配置範本<br>儀表板<br>行事曆<br>行事曆區段<br>外部頁面<br>報告<br>篩選<br>分組<br>檢視<br>引數 |
| 控制面板(PTLTAB) | 儀表板<br>行事曆<br>行事曆區段<br>外部頁面<br>報告<br>篩選<br>分組<br>檢視<br>引數 |
| 行事曆(CALEND) | 行事曆<br>行事曆區段 |
| 外部頁面(EXTSEC) | 外部頁面 |
| 報告(PTLSEC) | 報告<br>篩選<br>分組<br>檢視<br>引數 |
| 篩選器(UIFT) | 篩選<br>引數 |
| 分組(UIGB) | 分組<br>引數 |
| 檢視(UIVW) | 檢視<br>引數 |

### 自訂資料物件

| 可升級的物件 | 包含的可升級子物件 |
| --- | --- |
| 類別(CTGY) | 類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯<br>群組 |
| 引數（引數） | 引數<br>引數選項 |
| 引數群組(PGRP) | 參數群組 |

### 組織物件

| 可升級的物件 | 包含的可升級子物件 |
| --- | --- |
| 群組（群組） | 群組 <br>子群組（最多5個層級）<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |
| 角色(ROLE) | 角色 |
| 團隊（團隊） | 團隊<br>群組 |
| 公司(CMPY) | 公司<br>覆寫率<br>類別<br>類別引數<br>引數<br>引數群組<br>引數 <br>類別顯示邏輯<br>群組 |
| Portfolio（連線埠） | Portfolio<br>計畫<br>群組<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |
| 方案(PRGM) | 計畫<br>Portfolio<br>群組<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |

### 其他組態物件

| 可升級的物件 | 包含的可升級子物件 |
| --- | --- |
| 核准程式(ARVPRC) | 核准流程<br>核准路徑<br>核准步驟<br>步驟核准者<br>角色<br>團隊<br>群組 |
| 時程表(SCHED) | 排程<br>非工作日<br>群組 |
| 里程碑路徑(MPATH) | 里程碑路徑<br>里程碑 |
| 週期性時程表(TSPRO) | 週期性時程表<br>小時型別 |
| 小時型別（小時） | 時數類型 |
| 費用型別(EXPTYP) | 費用類型 |
| 風險型別(RSKTYP) | 風險類型 |
| 資源集區(RSPL) | 資源集區 |

## 驗證

API會驗證每個請求，以確保使用者端有權檢視或修改請求的物件。

透過傳入工作階段ID或API金鑰來執行驗證，該金鑰可使用以下方法之一提供：

### 請求標頭驗證

首選的驗證方法是傳遞包含工作階段權杖的名為SessionID的請求標頭。 其優點是可以安全抵禦 [跨網站請求偽造(CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻擊且不干擾URI以進行快取。

以下是請求標頭的範例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## api端點

* [建立套件](#create-a-package)
* [取得封裝清單](#get-a-list-of-packages)
* [依ID取得套件](#get-a-package-by-id)
* [取得套件的設定定義](#get-a-packages-configuration-definition)
* [取代封裝詳細資料和定義](#replace-package-details-and-definition)
* [更新封裝的特定屬性](#update-specific-properties-of-a-package)
* [刪除套裝](#delete-a-package)
* [執行預先執行](#execute-a-pre-run)
* [執行安裝](#execute-an-installation)
* [取得特定套件的安裝清單](#get-a-list-of-installations-for-a-specific-package)
* [取得安裝的安裝詳細資料](#get-the-installation-details-for-an-installation)

### 建立套件

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會執行多步驟流程。

第一個步驟會建立狀態為「組裝」的空白促銷活動套件。

第二個步驟使用 `objectCollections` POST主體中提供的陣列，用於從Workfront組合請求的記錄。 視要求的記錄數和Workfront設定而定，此步驟可能需要幾分鐘的時間才能完成。 在此程式結束時，空白的促銷活動套件會以更新 `packageEntities` 且狀態會自動設為「草稿」。


>[!NOTE]
>
>記下結構 `objectCollections`  陣列。
>
>陣列中的每個專案都包含 `objCode` 與Workfront API Explorer中記錄之物件程式碼對應的金鑰。
>
>每個專案也包含 `entities` 集合。 這預期 `ID` 和 `name` 金鑰將會出現。
>
>對於中請求的允許物件程式碼清單 `objectCollections` 清單，請參閱 [環境推進的支援物件](#supported-objects-for-environment-promotion) 一節。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### 個回應

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### 取得封裝清單

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會傳回屬於客戶的促銷套件未篩選清單。

回應將包含從客戶的任何沙箱、預覽或Workfront的生產執行個體建立的所有套件。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

### 依ID取得套件

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會傳回請求的促銷活動套件的詳細資料。

無論促銷活動套件的原始來源為何，都可透過任何環境進行請求。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 取得套件的設定定義

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### 取代封裝詳細資料和定義

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會取代促銷活動套件的所有內容。

該請求需要提供所有可編輯的欄位。

可編輯的屬性包括：

1. 名稱（字串）
1. 說明（字串）
1. 來源（含URL驗證的字串）
1. 狀態（含值驗證的字串）
1. 版本（整數）
1. packageEntities （集合）

狀態選項包括：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>組裝</td> 
   <td><p>組裝物件時，會自動指定此狀態。</p><p>客戶無法直接設定此狀態。</p></td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td><p>此狀態會在元件流程結束時或建立空推進封裝時指派。</p><p>客戶可以將促銷套件移回此狀態。</p><p>處於此狀態時，升級套件無法安裝在任何環境中。</p></td> 
  </tr> 
  <tr> 
   <td>測試</td> 
   <td><p>此狀態可讓促銷活動套件安裝在任何預覽或自訂重新整理沙箱中。 處於此狀態時，無法在生產環境中安裝套件。</p></td> 
  </tr> 
  <tr> 
   <td>作用中</td> 
   <td><p>此狀態可讓促銷活動套件安裝在任何環境中，包括生產環境。</p><p>當封裝狀態設定為ACTIVE時， <code>publishedAt</code> 日期會自動設定為請求目前的時間戳記。</p></td> 
  </tr> 
  <tr> 
   <td>已停用</td> 
   <td><p>此狀態將用於隱藏先前使用的促銷活動套件，這些套件日後不會安裝至任何環境。</p><p>當套件處於此狀態時，無法將其安裝在任何環境中。</p><p>當封裝狀態設定為DISABLED時， <code>retiredAt</code> 日期會自動設定為請求目前的時間戳記。</p><p>建議您使用此狀態，而不要使用<code>DELETE /package</code> 端點，因為它是可擷取的，而且會保留使用此套件進行的任何部署的安裝歷史記錄。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLY_FAILED</td> 
   <td><p>如果ASSEMBLY階段失敗，則推進封裝會自動處於此狀態。</p><p>若要將封裝返回ASSEMBLING階段，您必須再次觸發提取程式。</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### 個回應

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 更新封裝的特定屬性

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會更新PATCH內文中提供的促銷活動套件的任何內容。

可編輯的屬性包括：

1. 名稱（字串）
1. 說明（字串）
1. 來源（含URL驗證的字串）
1. 狀態（含值驗證的字串）
1. 版本（整數）
1. packageEntities （集合）

   或

   objectCollections （陣列）

提供 `packageEntities` 會以提供的組態定義更新促銷活動套件。

提供 `objectCollections` 將會起始重新擷取作業 `source` 和促銷活動套件相關聯的環境。 此 `source` 欄位必須提供當 `objectCollections` 已提供。

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
    "status": "ACTIVE"
}
```

#### 個回應

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 刪除套裝

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會刪除促銷活動套件記錄。 這個動作是不可逆的。

>[!NOTE]
>
>建議不要刪除促銷活動套件，而是將套件的狀態變更為「已停用」。 這樣可擷取套件，並保留其部署位置的安裝歷史記錄。

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```
Deleted
```

### 執行預先執行

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會比較封裝定義與URL中識別的目標環境。

結果會產生JSON內文，用來識別是否可在目標環境中找到推進物件。

針對每個推進物件，執行下列任一項作業 `actions`  將會設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td><p>在目標環境中找不到對應的記錄時，動作會設為CREATE。</p><p>此動作設定於 <code>translationmap</code> 提供給 <code>/install</code> 端點，安裝服務將建立記錄。</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>在目標環境中找到對應的記錄時，該動作會設為USEEXISTING並且 <code>targetId</code> 也會擷取至 <code>translationmap</code>.</p><p>此動作設定於 <code>translationmap</code> 提供給 <code>/install</code> 端點，安裝服務將不會建立記錄。 但是，它會使用 <code>targetId</code> 包含在對應專案中，用於可能參照此記錄的其他物件。</p><p>例如，在部署套件的目標環境中可能會找到「預設群組」。 不可能有兩個「預設群組」記錄，所以安裝服務將在任何其他物件建立動作中使用現有群組的GUID，這些動作包括對「預設群組」的參照，例如專案、表單或與此群組相關的任何其他實體。</p><p><b>備註:</b> <ul><li><p>指派USEEXISTING動作時，不會修改目標環境中的現有記錄。 </p><p>例如，如果在建立套件的來源沙箱中「預設群組」的說明已變更，並且目標環境中的說明值不同，則在使用此專案安裝後，值將維持不變 <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>忽略</td> 
   <td><p>系統不會自動設定此動作。</p><p>它提供在執行之前手動覆寫指派的CREATE或USEEXISTING動作的功能 <code>/install</code> 呼叫。</p><p><b>附註: </b><ul><li><p>如果原本設定為CREATE的記錄設定為IGNORE，則任何子記錄也應設定為IGNORE。</p><p>例如，如果範本記錄已使用CREATE動作對應，而安裝使用者希望將其從部署中排除，他們可以將範本的動作設定為IGNORE。</p><p>在此情況下，如果安裝使用者未將範本任務、範本任務指派、範本任務前置任務、佇列定義、佇列主題、路由規則等也設定為IGNORE，則部署會導致安裝嘗試失敗。</p></li><li><p>如果原本設定為USEEXISTING的記錄設定為IGNORE，安裝過程中可能會產生一些不良影響。</p><p>例如，如果「群組」記錄是以USEEXISTING動作對應，而安裝使用者將動作變更為IGNORE，則對於需要群組的物件（例如，如果沒有指派群組，Project就無法存在），系統預設群組將被指派給該專案。</p></li><li><p>如果原本設定為USEEXISTING的記錄設為CREATE，則在安裝過程中可能會產生一些不良影響，因為許多Workfront實體都有唯一名稱限制。</p><p>例如，如果以USEEXISTING動作對應「Default Group」記錄，而安裝使用者將動作變更為CREATE，因為已經有「Default Group」，所以安裝嘗試將無法完成所有步驟。 群組名稱必須是唯一的。</p><p>某些實體沒有唯一名稱限制。 對於這些物件，進行此變更將會產生兩個名稱相同的記錄。 例如，範本、專案、檢視、篩選器、群組、報告和儀表板不需要唯一名稱限制。 最佳做法是為這些記錄指定唯一的名稱，但不會強制執行。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

目前不支援更新 `action` 在此服務的alpha功能中。 允許更新的選項 `action` 是我們正在研究的專案。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/translationmap
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{}
```

#### 個回應

```
200
```

```json
{}
```

### 執行安裝

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會起始促銷活動套件安裝到POSTURL中識別之目標環境的嘗試。

#### 選項

如果 `translationmap` POST內文中未提供，處理將自動起始 `/translationmap` 呼叫。 此 `translationmap` 傳回的內容將依原樣使用，且沒有機會進行檢閱或調整。

如果 `translationmap` POST內文中提供，安裝程式將使用提供的對應。 這可讓安裝使用者在執行安裝嘗試之前，檢閱並視需要進行調整。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/install
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
}
```

#### 個回應

```
200
```


```json
{}
```

### 取得特定套件的安裝清單

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

結果包括部署該套件的所有環境中的安裝事件。 不限於發出要求之環境的安裝。 這可讓您識別哪些環境已收到此套件。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### 取得安裝的安裝詳細資料

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫將傳回最後 `translationMap` 由安裝服務針對特定安裝所產生。

每筆記錄會說明規定的內容 `action` 以及該動作是否成功。

對於具有CREATE的記錄 `action` 此 `targetId` 欄位將使用目標系統中新建立記錄的值來設定。 此外， `installationStatus` 欄位將設為INSTALLED。

對於具有USEEXISTING的記錄 `action` 此 `targetId` 欄位也會設定，而 `installationStatus` 欄位將設為REGISTERED。 這表示對應程式已完成，且安裝服務確認已評估記錄，且沒有可執行的動作。

如果記錄有CREATE `action` 但無法成功建立記錄，則 `installationStatus` 將會設定為FAILED ，並且還會提供失敗的原因。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### 標頭

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### 內文

_空白_

#### 個回應

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->