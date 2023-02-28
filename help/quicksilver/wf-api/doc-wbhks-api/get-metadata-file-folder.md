---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 獲取檔案或資料夾的元資料
description: 獲取檔案或資料夾的元資料
author: Becky
feature: Workfront API
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 6%

---


# 獲取檔案或資料夾的元資料

傳回指定檔案或資料夾的中繼資料。

**URL**

GET/metadata?id=[文檔或資料夾ID]

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
   <td>id</td> 
   <td>檔案或資料夾的ID，由Webhook提供程式引用。 這與Adobe Workfront的檔案ID不同。 要獲取根目錄的元資料，請使用值「/」。
   <p>注意：ID的長度上限為255個字元。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 個回應

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
   <td> 檔案的大小（以位元組為單位）。 (可選)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>布林值</td> 
   <td> 指出此檔案或資料夾是否為已驗證的使用者唯讀。(可選) </td> 
  </tr> 
 </tbody> 
</table>

**範例：** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document"，<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z」，<br>大小："32554694"<br>}</pre>

>[!NOTE]
>
>錯誤處理應在所有API呼叫間保持一致。 如需詳細資訊，請參閱下方的「錯誤處理」一節。
