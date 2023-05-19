---
content-type: api
navigation-topic: general-api
title: 使用API資源管理器
description: 使用API資源管理器
author: Becky
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 3db01c329c005570b782ae3445f83b7c44ced676
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 使用API資源管理器

使用Adobe Workfront核心API時，API瀏覽器是一個舊式參考工具，它可以編錄受支援資源、參數和變數之間的關係。

## 訪問API資源管理器：

1. 使用Web瀏覽器導航到 [API資源管理器](https://developer.adobe.com/workfront/api-explorer/)\
   ![](assets/mceclip1-350x149.png)

1. 在API瀏覽器的右上角，選擇所需的Workfront **API版本**，預設情況下自動選擇最新版本
1. 的 **篩選** 欄位，可用於篩選按名稱列出的對象，並將相應地截斷顯示的對象清單：

   ![](assets/mceclip2-350x147.png)

   * **欄位**:指定對象中的可用欄位。
   * **引用**:指定對象的可用引用變數。 引用是變數的別名。 一旦初始化，參照可與變數名稱互換使用。 引用使用初始化的記憶體。
   * **集合**:對象的可用集合。 集合是表示對象和資源之間一對多關係的變數。
   * **搜索**:對象的可用搜索資源。 搜索結果基於由API請求中的搜索資源指定的查詢參數。
   * **操作**:對象支援的操作。 操作可以是針對資源或一組資源執行的簡單或複雜的過程。 給定的操作也可能影響相關資源。

1. 開啟一個頁籤，然後按一下「對象ID」以查看適用的變數。\
   ![](assets/approval-350x89.png)\
   根據所選對象，可以應用以下變數：

   | 變數 | 定義 |
   |---|---|
   | 欄位名稱 | 在WorkfrontAPI內的操作中使用的欄位的名稱。 |
   | 欄位類型 | 可輸入到資料表中特定欄位的值的類型。 可能的欄位類型值包括string、double、int、dateTime。 |
   | 枚舉類型 | 可用於標識資料類型的值類型。 |
   | 可能的值 | 對象的可接受值。 |
   | 屬性類型ObjCode | 可用於修改對象類的屬性。 |
   | URL | 允許你的應用與WorkfrontAPI通信的入口路徑。 |
   | 參數 | 可在應用程式和Workfront之間傳遞的對象變數。 |
   | 結果類型 | 可以從方法返回的允許資料類型。 |
