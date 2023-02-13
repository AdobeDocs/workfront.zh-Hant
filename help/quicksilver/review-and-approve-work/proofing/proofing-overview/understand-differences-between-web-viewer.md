---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Web校對查看器與Desktop Pooting Viewer之間的差異概述
description: Adobe Workfront提供兩種不同的校對檢視器 — 「編輯我」。
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 2%

---

# Web校對查看器與Desktop Pooting Viewer之間的差異概述

Adobe Workfront提供兩種不同的校對檢視器：

* **Web校對查看器：** 主要用於校對靜態和視訊檔案。 在Google Chrome、Firefox或Safari中執行。
* **案頭校對查看器：** 專為校對互動式檔案以及視訊和靜態檔案而設計。 在工作站上以獨立應用程式的形式執行。 如需詳細資訊，請參閱 [了解案頭打樣檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* 如果您的組織因安全原因而無法使用案頭測試檢視器應用程式，則Workfront管理員可以設定您的系統，讓您可以在網頁測試檢視器中，檢閱ZIP封存檔案內隨附的互動式內容。 如需詳細資訊，請參閱  [在網頁校對檢視器中設定互動式內容校對](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

下列清單可協助您了解哪些校對檢視器可用來校樣特定類型的內容：

* **互動式網頁內容 — URL**:如果您使用URL建立網頁內容校樣，並且想要以互動方式校樣內容，則必須使用案頭校樣檢視器。
* **互動式網頁內容 — ZIP檔案**:如果您使用ZIP檔案建立網頁內容校樣，則可以使用Web校樣檢視器（有某些限制）或案頭校樣檢視器。 如需使用網頁校對檢視器進行互動式內容的相關限制資訊，請參閱 [在網頁校對檢視器中設定互動式內容校對](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **靜態和視訊內容**:如果您建立包含靜態內容的校樣，則可以使用Web校樣檢視器或案頭校樣檢視器。

## 靜態校樣

| **功能** | **網頁校對檢視器** | **案頭校對檢視器** |
|---|---|---|
| 開啟靜態校樣 | ✓ | ✓&#42; |
| 單一、雜誌和連續檢視 | ✓ | ✓&#42; |
| 平移 | ✓ | ✓&#42; |
| 縮放 | ✓ | ✓&#42; |
| 旋轉 | ✓ | ✓&#42; |
| 測量工具 | ✓（設定自訂大小的區域） | ✓&#42; |
| 縮圖檢視 | ✓ | ✓&#42; |
| 靜態校樣導覽器 | ✓ | ✓&#42; |
| 文檔搜索 | ✓ | ✓&#42; |
| 在多個頁面上張貼留言 | ✓（適用於所有檢視） | ✓&#42; （適用於所有檢視） |
| 高級靜態校樣快捷方式 | ✓(有關詳細資訊，請參閱 [校對檢視器中的鍵盤快速鍵](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;(如需詳細資訊，請參閱 [校對檢視器中的鍵盤快速鍵](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style=&quot;table-layout:auto&quot;}

&#42; 只有在您的Workfront管理員已將案頭校對檢視器設定為所有校樣的預設檢視器時，才能使用此功能。

## 影片校樣

| **功能**  | **網頁校對檢視器** | **案頭校對檢視器** |
|---|---|---|
| 開啟視訊校樣 | ✓ | ✓&#42; |
| 緩衝 | ✓ | ✓&#42; |
| 使用時間檢閱 | ✓ | ✓&#42; |
| 使用框架或時間碼進行審閱 | ✓ | ✓&#42; |
| 更快或更慢地審核 | ✓ | ✓&#42; |
| 音量調節 | ✓ | ✓&#42;  |
| 全螢幕模式 | ✓ | ✓&#42;  |
| 範圍注釋 | ✓ | ✓&#42;  |
| 重複播放視訊校樣（視訊自動完成和開始） | ✓ | ✓&#42;  |
| 進階視訊快速鍵 | ✓(有關詳細資訊，請參閱 [校對檢視器中的鍵盤快速鍵](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style=&quot;table-layout:auto&quot;}

&#42; 只有將案頭校對檢視器設定為所有校樣的預設檢視器時，此功能才有效。

## 互動式校樣

| **功能**  | **網頁校對檢視器** | **案頭校對檢視器** |
|---|---|---|
| 開啟從ZIP檔案中套件內容建立的互動式校樣 | ✓ | ✓（建議） |
| 開啟從URL建立的互動式校樣 | 不支援 | ✓ |
| 以各種螢幕大小檢視互動式校樣（從ZIP檔案中隨附的內容建立） | ✓ | ✓ |
| 檢視各種裝置的互動式校樣（從ZIP檔案中隨附的內容建立） | 不支援 | ✓ |
| 檢查不安全(HTTP)網站 | 不支援 | ✓ |
| 查看受iFrame保護的站點（在iFrame中受到保護的站點，以防被查看） | 不支援 | ✓ |

{style=&quot;table-layout:auto&quot;}

## 註解

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>網頁校對檢視器 </th> 
   <th>案頭校對檢視器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>添加、刪除和編輯注釋</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>新增和刪除回覆</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>矩形、箭頭、線、手繪和突出顯示標籤工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>折線工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>裁切遮色片標籤工具</p> </td> 
   <td>不支援</td> 
   <td>不支援</td> 
  </tr> 
  <tr> 
   <td> <p>文本選擇標籤工具</p> </td> 
   <td>✓僅靜態校樣</td> 
   <td>✓僅靜態校樣</td> 
  </tr> 
  <tr> 
   <td> <p>更改標籤顏色</p> </td> 
   <td>✓（32種可用顏色） </td> 
   <td>✓（32種可用顏色） </td> 
  </tr> 
  <tr> 
   <td> <p>更改標注不透明度</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>更改標籤厚度</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>剪下、複製和貼上標籤</p> </td> 
   <td> 不支援</td> 
   <td> 不支援</td> 
  </tr> 
  <tr> 
   <td> <p>撤消和重做上次操作</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>重複標籤</p> </td> 
   <td> 不支援</td> 
   <td> 不支援</td> 
  </tr> 
  <tr> 
   <td>將動作設定為註解</td> 
   <td>✓（設定動作後，就會立即在註解上顯示動作）</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>將標籤顏色設定為預設</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>解決注釋</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>鎖定注釋</p> </td> 
   <td>不支援</td> 
   <td> 不支援</td> 
  </tr> 
  <tr> 
   <td> <p>標籤使用者</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>繼續注釋</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>以精簡版檢視檢視註解清單</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>以標準、完整或單一檢視檢視註解清單</p> </td> 
   <td>未來計畫</td> 
   <td>未來計畫</td> 
  </tr> 
  <tr> 
   <td> <p>搜索注釋</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>按用戶篩選注釋</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>依使用者篩選留言和回覆</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>排序注釋</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>註解自動更新</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 決策

| 功能 | 網頁校對檢視器 | 案頭校對檢視器 |
|---|---|---|
| 做出決策 | ✓ | ✓ |
| 自訂決策 | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

## 比較校訂

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>網頁校對檢視器 </th> 
   <th>案頭校對檢視器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>比較不同版本的校樣</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>比較個別校樣</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## 校樣操作

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>網頁校對檢視器 </th> 
   <th>案頭校對檢視器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>變更校樣版本 </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>建立新版本</td> 
   <td> <p>僅適用於Workfront Proof(在Workfront內進行校對時預計於未來使用)<br></p> </td> 
   <td>僅適用於Workfront Proof(在Workfront內進行校對時預計於未來使用)</td> 
  </tr> 
  <tr> 
   <td>查看校樣詳細資訊 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>檢閱校樣工作流程</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>編輯工作流程階段</td> 
   <td>不支援</td> 
   <td>不支援</td> 
  </tr> 
  <tr> 
   <td>共用校樣</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>獲取團隊URL</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>變更電子郵件通知</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>下載原始檔案</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>鎖定和解鎖校樣和階段</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>打印校樣摘要</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>刪除校樣</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>管理相同資料夾中的校樣</td> 
   <td><strong>僅適用於Workfront Proof</strong> </td> 
   <td><strong>僅適用於Workfront Proof</strong> </td> 
  </tr> 
  <tr> 
   <td>品牌推廣（自訂標誌）</td> 
   <td>✓</td> 
   <td> ✓<br>(Workfront Logo on launch page) </td> 
  </tr> 
  <tr> 
   <td>自訂連結(僅限Workfront校樣)</td> 
   <td>不支援</td> 
   <td> 不支援 </td> 
  </tr> 
  <tr> 
   <td>基本整合(僅限Workfront Proof) </td> 
   <td>預計將來</td> 
   <td>預計將來</td> 
  </tr> 
  <tr> 
   <td>存在指示器 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>校樣自動更新（權限變更和新版本）</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## 微型檢視器

| **功能**  | **網頁校對檢視器**  | **案頭校對檢視器** |
|---|---|---|
| 內嵌程式碼 | 預計未來供靜態和原生視訊校樣使用 | 不支援  |

{style=&quot;table-layout:auto&quot;}

## 翻譯

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>功能</strong> </th> 
   <th><strong>網頁校對檢視器</strong> </th> 
   <th><strong>案頭校對檢視器</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>支援英語以外的語言</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
