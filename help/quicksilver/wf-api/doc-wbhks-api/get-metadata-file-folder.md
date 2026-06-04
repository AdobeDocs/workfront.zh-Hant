---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得檔案或資料夾的中繼資料
description: 取得檔案或資料夾的中繼資料
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
TQID: https://experienceleague.adobe.com/H04UQeyhGw-FdXDwaRZs5PSXnN-YErVptHWn-78INYo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 8%

---

# 取得檔案或資料夾的中繼資料

傳回指定檔案或資料夾的中繼資料。

**URL**

取得/metadata？id=[檔案或資料夾識別碼]

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
   <td>檔案或資料夾的ID，由webhook提供者參照。這與Adobe Workfront的檔案ID不同。若要取得根目錄的中繼資料，請使用值'/'。
   <p>注意：ID的長度上限為255個字元。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 回應

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
   <td>標題 </td> 
   <td>字串 </td> 
   <td>檔案或資料夾的名稱</td> 
  </tr> 
  <tr> 
   <td>種類 </td> 
   <td>字串 </td> 
   <td>指定此專案是檔案還是資料夾（'file'或'folder'）</td> 
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
   <td>檔案的MIME型別。 (可選)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>字串 </td> 
   <td>上次修改此檔案的時間（格式為RFC 3339時間戳記）</td> 
  </tr> 
  <tr> 
   <td>大小</td> 
   <td>長</td> 
   <td> 檔案大小（位元組）。 (可選)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>布林值</td> 
   <td> 指出此檔案或資料夾對已驗證的使用者是否為唯讀。（選擇性） </td> 
  </tr> 
 </tbody> 
</table>

**範例：** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title："My Document"，<br>kind："file"<br>id"："12345"，<br>viewLink："https://www.acme.com/viewDocument?id=12345"，<br>downloadLink："https://www.acme.com/downloadDocument?id=12345"，<br>mimeType："image/png"，<br>dateModified："20140605T17:39:45.251Z"，<br>size："32554694"<br>}</pre>

>[!NOTE]
>
>所有API呼叫的錯誤處理都應保持一致。 如需詳細資訊，請參閱下方的「錯誤處理」一節。
