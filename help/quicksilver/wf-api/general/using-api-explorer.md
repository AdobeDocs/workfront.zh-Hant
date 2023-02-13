---
content-type: api
navigation-topic: general-api
title: 使用API Explorer
description: 使用API Explorer
author: John
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 使用API Explorer

使用Adobe Workfront核心API時，API總管是舊版參考工具，可記錄支援的資源、參數和變數之間的關係。

## 存取API總管：

1. 使用網頁瀏覽器導覽至 [API Explorer](https://one.workfront.com/s/api-explorer)\
   ![](assets/mceclip1-350x149.png)

1. 在API Explorer的右上方，選取所需的Workfront **API版本**，預設會自動選取最新版本
1. 此 **篩選** 欄位，可用來篩選依名稱列出的物件，並會截斷相應顯示的物件清單：

   ![](assets/mceclip2-350x147.png)

   * **欄位**:指定對象內的可用欄位。
   * **參考**:指定對象的可用引用變數。 參考是變數的別名。 初始化後，參照可與變數名稱交互使用。 引用使用初始化的記憶體。
   * **集合**:對象的可用集合。 集合是代表物件和資源之間一對多關係的變數。
   * **搜尋**:對象的可用搜索資源。 搜尋結果以API請求中搜尋資源所指定的查詢參數為基礎。
   * **動作**:支援的物件動作。 動作可以是針對資源或一組資源執行的簡單或複雜程式。 指定的動作也可能會影響相關資源。

1. 開啟標籤，然後按一下「物件ID」以檢視適用的變數。\
   ![](assets/approval-350x89.png)\
   根據選取的物件，可能會套用下列變數：

   | 變數 | 定義 |
   |---|---|
   | 欄位名稱 | Workfront API內作業中使用的欄位名稱。 |
   | 欄位類型 | 可輸入到資料表中特定欄位的值類型。 可能的欄位類型值包括字串、double、int、dateTime。 |
   | 枚舉類型 | 可用於識別資料類型的值類型。 |
   | 可能的值 | 物件的可接受值。 |
   | 屬性類型ObjCode | 可用於修改對象類的屬性。 |
   | URL | 允許應用程式與Workfront API通訊的進入路徑。 |
   | 引數 | 可在您的應用程式與Workfront之間傳遞的物件變數。 |
   | 結果類型 | 可從方法傳回的允許資料類型。 |
