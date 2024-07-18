---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 使用Adobe Workfront API追蹤小時記錄
description: 如果您的組織使用Adobe Workfront來輸入工作時數，但使用其他工具作為該資料的記錄系統，您可以使用Workfront API在兩個系統之間同步資料。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 使用Adobe Workfront API追蹤小時記錄

如果您的組織使用Adobe Workfront來輸入工作時數，但使用其他工具作為該資料的記錄系統，您可以使用Workfront API在兩個系統之間同步資料。

單純地追蹤時數記錄並不可行，因為如果移除時數輸入項，就會刪除整個記錄，而需要您提取整個資料集並與舊資料集進行比較。 幸運的是，所有小時異動都記錄在Workfront分錄中。

擷取系統中所有目前時數的初始集合後，您可以透過「日誌專案」追蹤任何及所有變更。
<pre>GET/attask/api/v5.0/JRNLE/search？subObjCode=HOUR&amp;fields=changeType，aux2，newNumberVal，oldNumberVal，subObjCode，subObjID</pre><pre>{<br>"資料"： [<br>{<br>"ID"： "5785406d008d93dd35665f14d90d4929"，<br>"objCode"： "JRNLE"，<br>"changeType"： "A"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 1，<br>"oldNumberVal"： null，<br>"subObjCode" "HOUR"，<br>"subObjID"： "5785406d008d93dce3f7f2e0e8eda4ea"<br>}，<br>{<br>"ID"： "57854124008da2b9f372c01f8b9054bf"，<br>"objCode"： "JRNLE"，<br>"changeType"： "D"，<br>"aux2"： brad Littler」，<br>"newNumberVal"： null，<br>"oldNumberVal"： 1，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785406d008d93dce3f7f2e0e8eda4ea"<br>}，<br>{<br>"ID"： "5785416f08db05ecee934663968366"，<br>"objCode"： "JRNLE"，<br>"changeType"： "A"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 1，<br>"oldNumberVal"： null，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785416f008db05d9d2925c 112b10f521"<br>}，<br>{<br>"ID"： "57854176008db22fe974b7c67feea6b2"，<br>"objCode"： "JRNLE"，<br>"changeType"： "E"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 2，<br>"oldNumberVal"： 1，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>以下為包含欄位的說明：

* **changeType：**&#x200B;對物件進行的變更型別：

   * **A：**&#x200B;新增

   * **E：**&#x200B;編輯

   * **天：**&#x200B;刪除

* **aux2：**&#x200B;時數記錄所針對的使用者名稱。

* **newNumberVal：**&#x200B;小時記錄的新值（如果changeType是D，則為Null）。

* **oldNumberVal：**&#x200B;小時記錄的先前值。

* **subObjCode：**&#x200B;正在修改的記錄型別（應該一律為HOUR）。

* **subObjID：**&#x200B;時數記錄的識別碼。

您可以使用此資訊來探索哪些小時記錄已變更、編輯或刪除。 如有必要，您可以使用subObjID從小時記錄中擷取更多資訊。
