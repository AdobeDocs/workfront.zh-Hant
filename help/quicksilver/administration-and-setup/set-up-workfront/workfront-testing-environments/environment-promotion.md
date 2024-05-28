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
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 96ff148ff9a05242d9ce900047d5e7d1de3f0388
workflow-type: tm+mt
source-wordcount: '1829'
ht-degree: 2%

---

# 移動物件 [!DNL Workfront] 使用環境 [!DNL Workfront] 環境升級API

「環境升級」功能的目的是提供與組態相關的物件從一個環境移動到另一個環境的功能。 您可以使用本文所述的Workfront API來移動這些物件。

如需使用Workfront應用程式在環境之間移動物件的相關指示，請參閱：

* [建立或編輯環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [安裝環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


<!-- add access req for GA-->

## 先決條件

「建立促銷活動套件」端點會假設您已設定來源環境。 此API呼叫需要手動建立 [!DNL Workfront] 物件程式碼和物件GUID。 此地圖的特定結構如下所述。

## 環境推進的支援物件

「環境升級」功能的目的是提供與組態相關的物件從一個環境移動到另一個環境的功能。 不支援移動異動物件的功能（只有少數例外）。

如需可升級物件及其包含的可升級子物件的清單，請參閱 [環境推進的支援物件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) 在文章中 [在Workfront環境之間移動物件的概觀](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## 驗證

API會驗證每個請求，以確保使用者端有權檢視或修改請求的物件。

透過傳入工作階段ID或API金鑰來執行驗證，金鑰可使用以下方法提供：

### 請求標頭驗證

首選的驗證方法是傳遞包含工作階段權杖的名為SessionID的請求標頭。 其優點是可以安全抵禦 [跨網站請求偽造(CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻擊且不干擾URI以進行快取。

以下是請求標頭的範例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## api端點

* [建立套件](#create-a-package)
* [取得封裝清單](#get-a-list-of-packages)
* [依ID取得套件](#get-a-package-by-id)
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
>每個專案也包含 `entities` 集合。 這預期 `ID` 欄位。 它也可以接受選填的 `name` 屬性，以便於瞭解 `ID` 表示。
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
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
    "name": "Agency Onboarding - 2023-06-06",
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

#### 回應

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 內文

_空白_

#### 回應

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
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;! — 檢查上面的「狀態」 — 是否新增？—>

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
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 內文

_空白_

#### 回應

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
1. 狀態（含值驗證的字串）

如需可用狀態的詳細說明，請參閱 [環境升級狀態](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) 在文章中 [在Workfront環境之間移動物件的概觀](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### 標頭

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
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

#### 回應

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 內文

_空白_

#### 回應

```
200
```

```
Deleted
```

### 執行預先執行

>[!IMPORTANT]
>
>您必須先執行此預先執行，才能執行安裝。 執行安裝時，會使用由此呼叫產生的ID。

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
   <td><p>在目標環境中找到對應的記錄時，該動作會設為USEEXISTING並且 <code>targetId</code> 也會擷取至 <code>translationmap</code>.</p><p>此動作設定於 <code>translationmap</code> 提供給 <code>/install</code> 端點，安裝服務將不會建立記錄。 但是，它會使用 <code>targetId</code> 包含在對應專案中，用於可能參照此記錄的其他物件。</p><p>例如，在部署套件的目標環境中可能會找到「預設群組」。 不可能有兩個「預設群組」記錄，所以安裝服務將在任何其他物件建立動作中使用現有群組的GUID，這些動作包括對「預設群組」的參照，例如專案、表單或與此群組相關的任何其他實體。</p><p><b>注意：</b> <ul><li><p>指派USEEXISTING動作時，不會修改目標環境中的現有記錄。 </p><p>例如，如果在建立套件的來源沙箱中「預設群組」的說明已變更，並且目標環境中的說明值不同，則在使用此專案安裝後，值將維持不變 <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>覆寫</td> 
   <td><p>系統不會自動設定此動作。</p><p>此動作提供更新目標環境中存在的物件的功能。 它提供在執行之前手動覆寫指派的CREATE或USEEXISTING動作的功能 <code>/install</code> 呼叫。<ul><li>使用者可以更新測試環境中的物件，然後使用OVERWRITING動作更新目標環境中的該物件。</p></li><li><p>如果使用者一開始安裝一個推進封裝，而日後新（或更新的）封裝包含對初始封裝中物件的變更，則使用者可以使用「覆寫」來取代（覆寫）先前安裝的物件。 </p></li><ul></td> 
  </tr> 
  <tr> 
   <td>忽略</td> 
   <td><p>系統不會自動設定此動作。</p><p>它提供在執行之前手動覆寫指派的CREATE或USEEXISTING動作的功能 <code>/install</code> 呼叫。</p><p><b>附註： </b><ul><li><p>如果原本設定為CREATE的記錄設定為IGNORE，則任何子記錄也應設定為IGNORE。</p><p>例如，如果範本記錄已使用CREATE動作對應，而安裝使用者希望將其從部署中排除，他們可以將範本的動作設定為IGNORE。</p><p>在此情況下，如果安裝使用者未將範本任務、範本任務指派、範本任務前置任務、佇列定義、佇列主題、路由規則等也設定為IGNORE，則部署會導致安裝嘗試失敗。</p></li><li><p>如果原本設定為USEEXISTING的記錄設定為IGNORE，安裝過程中可能會產生一些不良影響。</p><p>例如，如果「群組」記錄是以USEEXISTING動作對應，而安裝使用者將動作變更為IGNORE，則對於需要群組的物件（例如，如果沒有指派群組，Project就無法存在），系統預設群組將被指派給該專案。</p></li><li><p>如果原本設定為USEEXISTING的記錄設為CREATE，則在安裝過程中可能會產生一些不良影響，因為許多Workfront實體都有唯一名稱限制。</p><p>例如，如果以USEEXISTING動作對應「Default Group」記錄，而安裝使用者將動作變更為CREATE，因為已經有「Default Group」，所以安裝嘗試將無法完成所有步驟。 群組名稱必須是唯一的。</p><p>某些實體沒有唯一名稱限制。 對於這些物件，進行此變更將會產生兩個名稱相同的記錄。 例如，範本、專案、檢視、篩選器、群組、報告和儀表板不需要唯一名稱限制。 最佳做法是為這些記錄指定唯一的名稱，但不會強制執行。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

目前不支援更新 `action` 在此服務的alpha功能中。 允許更新的選項 `action` 是我們正在研究的專案。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### 標頭

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{}
```

#### 回應

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>執行安裝所需的ID為 `id` 欄位。 在此範例中， `id` 欄位在頂端的第三個位置，其值開頭為 `c0bc79bd`.

### 執行安裝

>[!IMPORTANT]
>
>您必須先執行預先執行，才能執行安裝。 執行安裝時，您會使用預先執行所產生的ID。
>
>如果在執行預先執行後，對目的地環境（套件將部署到的環境）進行了任何變更，我們建議再次執行預先執行。 如果您未再次執行預先執行，您的執行可能無法正確完成，或是安裝可能失敗。
>
>如需有關執行預先執行的指示，請參閱 [執行預先執行](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

此呼叫會起始促銷活動套件安裝到POSTURL中識別之目標環境的嘗試。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### 標頭

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 內文

```json
{
}
```

#### 回應

```
202
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### 標頭

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 內文

_空白_

#### 回應

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
        "status": "INSTALLED",
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
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 內文

_空白_

#### 回應

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
    "status": "INSTALLED",
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
