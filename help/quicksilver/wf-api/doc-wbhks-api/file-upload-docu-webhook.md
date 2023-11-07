---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 透過Document Webhook上傳檔案
description: 透過Document Webhook上傳檔案
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 5%

---


# 透過Document Webhook上傳檔案

將檔案上傳至檔案儲存提供者是一個包含兩個步驟的程式，需要兩個不同的API端點。 Adobe Workfront會呼叫/uploadInit以開始上傳程式。 此端點會傳回檔案ID，然後在上傳檔案位元組時傳遞給/upload。 根據基礎檔案儲存系統，可能需要建立長度為零的檔案，然後稍後更新檔案的內容。

將檔案ID和檔案版本ID新增至本規格1.1版，可用來從Workfront擷取額外資訊。

**範例：** 如果檔案管理系統需要檔案的額外資訊，webhook實作程式碼可以使用檔案ID，透過Workfront的RESTful API擷取該資訊。 好的實務是，此資訊可能來自檔案上的自訂資料欄位，並包含任務、問題或專案。

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
   <td>Webhook提供者參照的父資料夾ID。</td> 
  </tr> 
  <tr> 
   <td>檔案名稱 </td> 
   <td>檔案的名稱</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront檔案ID （在1.1版中新增）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront檔案版本ID （在1.1版中新增） </td> 
  </tr> 
 </tbody> 
</table>

## 個回應

由/metadata端點定義的檔案中繼資料。 這包括提供者使用的檔案ID。

**範例:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT方法

將檔案的位元組上傳到webhook提供者。

**URL**

PUT/upload

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id  |  剛建立的檔案ID。 |


**要求內文**

檔案的原始內容位元組。

**回應**

```
{
result: "success"
}
```

或

```
{
result: "fail"
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
