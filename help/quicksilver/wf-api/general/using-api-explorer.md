---
content-type: api
navigation-topic: general-api
title: 使用API總管
description: 使用API總管
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---


# 使用API總管

使用Adobe Workfront核心API時，API Explorer是舊版參考工具，可編錄支援的資源、引數和變數之間的關係。

## 存取API Explorer：

1. 使用網頁瀏覽器導覽至[API總管](https://developer.adobe.com/workfront/api-explorer/)\
   ![瀏覽至API總管](assets/mceclip1-350x149.png)

1. 在API Explorer的右上角，選取所需的Workfront **API Version**，預設會自動選取最新版本
1. **篩選器**&#x200B;欄位可用來篩選依名稱列出的物件，並將截斷顯示的物件清單：

   ![API總管欄位](assets/mceclip2-350x147.png)

   * **欄位**：指定物件中的可用欄位。
   * **參考**：指定物件的可用參考變數。 參照是變數的別名。 初始化後，參照可與變數名稱互換使用。 參考使用初始化的記憶體。
   * **集合**：物件的可用集合。 集合是代表物件與資源之間一對多關係的變數。
   * **搜尋**：物件的可用搜尋資源。 搜尋結果會根據API要求中搜尋資源所指定的查詢引數而定。
   * **動作**：物件支援的動作。 動作可以是針對資源或一組資源執行的簡單或複雜程式。 指定的動作也可能影響相關資源。

1. 開啟標籤，然後按一下「物件ID」以檢視適用的變數。\
   ![檢視變數](assets/approval-350x89.png)\
   根據選取的物件，可能會套用下列變數：

   | 變數 | 定義 |
   |---|---|
   | 欄位名稱 | Workfront API內之作業所使用的欄位名稱。 |
   | 欄位型別 | 可在資料表格的特定欄位中輸入的值型別。 可能的欄位型別值包括字串、double、int、dateTime。 |
   | 列舉型別 | 可用來識別資料型別的值型別。 |
   | 可能的值 | 物件的可接受值。 |
   | 屬性型別物件代碼 | 可用來修改物件類別的屬性。 |
   | URL | 可讓您的應用程式與Workfront API通訊的進入路徑。 |
   | 引數 | 可在應用程式和Workfront之間傳遞的物件變數。 |
   | 結果型別 | 可從方法傳回的允許資料型別。 |
