---
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: '''分組：顯示在分組中聚合多個計算值的結果'
description: 您可以在欄中使用文字模式，在報表或清單檢視的兩個欄位之間顯示計算。 每行顯示報告或清單中每個對象的計算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 分組：顯示在分組中聚合多個計算值的結果

您可以在欄中使用文字模式，在報表或清單檢視的兩個欄位之間顯示計算。 每行顯示報告或清單中每個對象的計算。

例如，您可以在名為「工作餘額」的第三列中顯示任務報表中每個任務的實際小時數和計畫小時數之間的差異。 如需計算資料運算式的詳細資訊，請參閱 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

您可以將計算新增至 `aggregator` 包含計算值的欄的行。 例如，您可以匯總（顯示總和）報表分組或「工作餘額」列清單中所有任務的工作餘額小時數。 本文說明如何執行此操作。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 顯示在分組中聚合多個計算值的結果

1. 前往任務報表，按一下 **報表動作** > **編輯**.
1. 在 **分組** 按一下 **添加分組**，然後開始輸入 **專案名稱** 在 **將報表分組** > **第一個** 欄位，然後在清單中顯示時選取它。

1. 在 **列（視圖）** 按一下 **添加列**，然後開始輸入 **計畫小時數** 在 **顯示在此列中** 欄位，然後在清單中顯示時選取它。

   >[!TIP]
   >
   >在文本模式中編輯資訊之前，請始終使用標準介面添加盡可能多的資訊。 新增最接近或包含您嘗試進行之計算之最多資訊的欄位。

1. 在 **匯總此欄，依** 欄位，選擇 **總和**，然後按一下 **完成**.
1. 按一下 **切換到文本模式** 在您新增的欄中。
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 取代 `valuefield ` 和 `aggregator.valuefield` 在以下文本模式中突出顯示的行示例：

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >為了在分組中獲取匯總值以顯示「計畫小時數」和「實際小時數」欄位之間的匯總差異，請將相同的公式輸入到 `aggregator.valuefield` 行。 此 `aggregator.displayformat` 用於「計畫小時數」列將分鐘數轉換為小時數。 由於「計畫時數」欄位是作為預留位置，因此無需調整此行。
   >
   >
   >此 `minutesAsHoursString` 定義 `aggregator.displayformat` 折線表示不需要依照 `valueexpression` 為結果。 在此 `aggregator.valuefield=workRequired` 變成： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. 按一下 **儲存並關閉**.
