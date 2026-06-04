---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 執行自訂動作
description: 執行自訂動作
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
TQID: https://experienceleague.adobe.com/y9RxzhalPQGx0BEMOtLVOAxwyh-OhQcxuARtBrJd8Yg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 191
ht-degree: 4%

---

# 執行自訂動作（尚未實作）

此端點可讓Adobe Workfront使用者（或自動化工作流程事件）在外部系統中執行動作。 /customAction端點接受「name」引數，此引數允許webhook提供者實作多個自訂操作。

webhook提供者會將actions包含在customActions下的/serviceInfo回應中，藉此向Workfront註冊自訂動作。 Workfront會在設定>檔案>自訂整合底下設定或重新整理webhook提供者時載入此清單。

使用者可以透過選擇「檔案動作」下的區段來觸發自訂動作

**URL**

GET /customAction

## 查詢參數

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
   <td> <p>名稱</p> </td> 
   <td> <p>指定要執行的動作型別的識別碼。 此值對應至/serviceInfo端點傳回的其中一個customAction值。</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>正在對其執行動作的Workfront檔案ID。</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> 正在對其執行動作的Workfront檔案版本ID。</td> 
  </tr> 
 </tbody> 
</table>

 

## 回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。 失敗時（即狀態= &quot;failure&quot;），Workfront會向使用者顯示提供的錯誤訊息。

**範例：**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

回應

```
{
status: "success"
}
```
