---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 使用Adobe Workfront API追蹤小時記錄
description: 如果貴組織使用Adobe Workfront輸入工作時數，但使用其他工具作為該資料的記錄系統，則您可以使用Workfront API來同步這兩個系統之間的資料。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 使用Adobe Workfront API追蹤小時記錄

如果貴組織使用Adobe Workfront輸入工作時數，但使用其他工具作為該資料的記錄系統，則您可以使用Workfront API來同步這兩個系統之間的資料。

單純追蹤小時記錄並不可行，因為如果移除小時項目，就會刪除整個記錄，您必須提取整個資料集，並與舊資料集比較。 所幸的是，所有小時事務處理都記錄在Workfront日記帳分錄中。

檢索系統中所有當前小時的初始集合後，您可以通過「日記帳分錄」跟蹤任何更改和所有更改。
<pre>GET/attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data":[<br>{<br>"ID":"5785406d008d93dd35665f14d90d4929",<br>"objCode":"JRNLE",<br>"changeType":"A"<br>"aux2":《布拉德·利特勒》<br>"newNumberVal":1,<br>"oldNumberVal":null,<br>"subObjCode":「小時」，<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"57854124008da2b9f372c01f8b9054bf",<br>"objCode":"JRNLE",<br>"changeType":"D",<br>"aux2":《布拉德·利特勒》<br>"newNumberVal":null,<br>"oldNumberVal":1,<br>"subObjCode":「小時」，<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"5785416f008db05ecee934663a968366",<br>"objCode":"JRNLE",<br>"changeType":"A"<br>"aux2":《布拉德·利特勒》<br>"newNumberVal":1,<br>"oldNumberVal":null,<br>"subObjCode":「小時」，<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID":"57854176008db22fe974b7c67feea6b2",<br>"objCode":"JRNLE",<br>"changeType":"E",<br>"aux2":《布拉德·利特勒》<br>"newNumberVal":2,<br>"oldNumberVal":1,<br>"subObjCode":「小時」，<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>以下是所包含欄位的說明：

* **changeType:** 對對象進行的更改類型：

   * **答：** 新增

   * **E:** 編輯

   * **D:** 刪除

* **aux2:** 小時記錄的用戶名。

* **newNumberVal:** 小時記錄的新值（如果changeType為D，則此值為null）。

* **oldNumberVal:** 小時記錄的前一個值。

* **subObjCode:** 要修改的記錄類型（應始終為HOUR）。

* **subObjID:** 小時記錄ID。

您可以使用此資訊來發現哪些小時記錄已更改、編輯或刪除。 如有必要，您可以使用subObjID從小時記錄中擷取更多資訊。
