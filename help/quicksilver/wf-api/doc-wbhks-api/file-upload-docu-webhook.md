---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 透過檔案Webhook上傳檔案
description: 透過檔案Webhook上傳檔案
author: Becky
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# 透過檔案Webhook上傳檔案

將檔案上傳至檔案儲存提供者是兩步驟程式，需要兩個不同的API端點。 Adobe Workfront借由呼叫/uploadInit來開始上傳程式。 此端點會傳回檔案ID，然後在上傳檔案位元組時傳遞至/upload。 根據基礎文檔儲存系統，可能需要建立一個零長度的文檔，然後稍後更新該文檔的內容。

新增至此規格的1.1版，檔案ID和檔案版本ID可用來擷取來自Workfront的額外資訊。

**範例：** 如果檔案管理系統需要有關該檔案的額外資訊，Webhook實作程式碼可使用檔案ID，使用Workfront的RESTful API來擷取該資訊。 此資訊可能來自檔案上的自訂資料欄位，且包含任務、問題或專案，此為最佳作法。

## POST方法

**URL**

POST/uploadInit

### 查詢參數

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
   <td>Workfront檔案版本ID（在1.1版中新增） </td> 
  </tr> 
 </tbody> 
</table>

## 個回應

檔案的元資料，由/metadata端點定義。 這包括提供者使用的檔案ID。

**範例:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT方法

將文檔的位元組上載到Webhook提供程式。

**URL**

PUT/上傳

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id  |  剛建立的文檔ID。 |


**要求內文**

文檔的原始內容位元組。

**回應**

```
{
result: “success”
}
```

或

```
{
result: “fail”
}
```

**範例**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

回應

```
{
result:"success"
}
```
