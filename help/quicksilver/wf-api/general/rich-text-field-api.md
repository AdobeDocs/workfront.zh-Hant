---
content-type: api
navigation-topic: general-api
title: Adobe Workfront API中的RTF欄位
description: Adobe Workfront API中的RTF欄位
author: Becky
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Adobe Workfront API中的RTF欄位

Adobe Workfront中的某些物件可儲存具有RTF格式的文字。 在Workfront API中，使用開放原始碼架構Draft.js時，RTF會儲存為JSON。

## 概述範例

會呼叫具有RTF格式的自訂欄位 **具有RTF文字的欄位** 和可以有下列與之相關聯的值：

![](assets/rich-text-example-350x158.png)

**範例：** 擷取自訂表單欄位值的基本GET請求 **具有RTF文字的欄位**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**範例：** 此要求會傳回 **具有RTF文字的欄位** 儲存於 **parameterValue** **DE:RTF欄位**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**範例：** 這是上圖中特有的格式化響應版本

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## 區塊

儲存RTF內容的JSON物件由兩個主要部分組成： **塊** 和 **entityMaps**.

區塊是JSON物件，代表單行格式化文字。 由於單個自訂欄位可以有多行文字，因此每行文字都有其專屬的區塊，且每個區塊在稱為的父陣列中以元素的形式呈現 **塊**.

**範例：** 在此，自訂欄位的每行文字都對應至陣列區塊中的區塊元素

![](assets/copy-of-rich-text-mapping-350x159.png)

由於每個區塊元素也是JSON物件，因此每個區塊都由元素組成： **key**, **文字**, **type**, **深度**, **inlineStyleRanges**, **entityRanges**，和 **資料**. 這些元素的作用如下：

* **金鑰** 是該區塊的唯一識別碼。 索引鍵可用來透過entityMaps對應一行文字。 有關entityMaps的詳細資訊可在此文檔的entityMaps部分中找到。
* **文字** 是從自訂欄位儲存的文字內容行。
* **類型** 說明要呈現的文字類型。 例如，儲存在區塊中的一行文字可能是清單的一部分。 如果該行文本是未排序清單的一部分，則其類型將定義為：無序清單項。
* 目前不支援清單，但應盡快提供。
* **深度** 當行是有序或無序清單的嵌套部分時，此參數定義行的深度。
* **inlineStyleRanges** 是一個陣列，用於描述應用於當前塊所表示文本行的格式類型。

**範例：** 以下是描述字元級別每個樣式的inlineStyleRanges陣列。 在此情況下：9個字元(長度：9)從索引0開始(偏移：0)有樣式 **粗體** 已套用：

![](assets/copy-of-rich-text-mapping-2-350x136.png)

若已將多種格式類型套用至單一行，則樣式會對應至** inlineStyleRanges**陣列中的其他元素。

**範例：** 以下是儲存包含混合格式的文字行時區塊的外觀： **粗體文字和斜體**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>20.3版之後的所有版本都支援粗體、斜體和底線格式選項。

## entityMaps和entityRanges

資料塊可能包含超連結等實體，或連接到位於自訂文字欄位外部資料來源的其他類型化格式。

## 範例

### 從JSON擷取純文字

提交具有RTF格式的自訂欄位時，所有文字都會儲存在陣列中 **塊**. 不過，每行全文都會儲存在 **文字參數** 在組成父陣列的每個獨立塊元素內 **塊**. 因此，為了檢索全文，需要提取每一行單獨的文本，並將它們分開。 這可透過循環區塊中的所有元素並串連每個文字參數，以及行分隔字元(\n)來達成。

**範例：** 以下是您的JS看起來的樣子：

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### 使用Workfront API儲存RTF欄位值

若要使用Workfront API儲存RTF欄位的下列值：
<pre>
		Hello <strong>世界</strong>!!!
		這是我的第一個 <strong>RTF</strong></pre>

1. 建構JSON，此JSON可將每行文字組織到陣列中的區塊元素，以呈現您嘗試擷取的RTF欄位值 **塊**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 使用 **inlineStyleRanges** 參數

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 若要擷取第二行，文字「Rtf」必須以粗體和斜體格式。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >雖然初始發行期間不支援entityMap功能，但仍是在請求中傳遞此JSON的必要欄位

1. 使用 **stringify** 方法（如上所述）來建立 **PUT** 要求和傳送更新

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
