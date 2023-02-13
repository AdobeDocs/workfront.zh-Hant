---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 執行自訂動作
description: 執行自訂動作
author: John
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# 執行自訂動作（尚未實作）

此端點可讓Adobe Workfront使用者（或自動化工作流程事件）在外部系統中執行動作。 /customAction端點接受「name」參數，該參數允許Webhook提供程式實施多個自定義操作。

Webhook提供者會將動作納入customActions下的/serviceInfo回應中，以向Workfront註冊自訂動作。 Workfront在「設定>檔案>自訂整合」下設定或重新整理網頁連結提供者時，會載入此清單。

使用者可以選取「檔案動作」下方的區段，以觸發自訂動作

**URL**

GET/customAction

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
   <td> <p>指定要執行之動作類型的識別碼。 此值對應於/serviceInfo端點返回的一個customAction值。</p> </td> 
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

 

## 個回應

表示成功或失敗的JSON字串，如下方的錯誤處理一節中所指定。 失敗時（即狀態= &quot;failure&quot;）,Workfront會向使用者顯示提供的錯誤訊息。

**範例:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

回應

```
{
status: “success”
}
```
