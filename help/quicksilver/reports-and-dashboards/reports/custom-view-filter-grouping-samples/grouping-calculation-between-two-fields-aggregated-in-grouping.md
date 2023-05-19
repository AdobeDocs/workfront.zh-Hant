---
content-type: reference
product-area: reporting;projects
keywords: 計算，聚合，高級，視圖
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：顯示在分組中聚合多個計算值的結果'
description: 可以在列中使用文本模式來在報表或清單視圖中的兩個欄位之間顯示計算。 每行都顯示報表或清單中每個對象的計算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 分組：顯示分組中聚合多個計算值的結果

可以在列中使用文本模式來在報表或清單視圖中的兩個欄位之間顯示計算。 每行都顯示報表或清單中每個對象的計算。

例如，您可以在任務報表中每個任務的第三列（稱為「工作餘額」）中顯示「實際小時數」和「計畫小時數」之間的差異。 有關計算資料表達式的詳細資訊，請參見 [計算的資料表達式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

通過將計算添加到 `aggregator` 包含計算值的列的行。 例如，您可以匯總（顯示）報表分組或「工作餘額」列清單中所有任務的工作餘額小時數。 本文介紹了如何做到這一點。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問</p> <p>編輯對篩選器、視圖、分組的訪問</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 顯示分組中聚合多個計算值的結果

1. 轉到任務報告，按一下 **報告操作** > **編輯**。
1. 在 **分組** 按鈕 **添加分組**，然後開始鍵入 **項目名稱** 的 **將報告分組** > **第一個** 的子菜單。

1. 在 **列（視圖）** 按鈕 **添加列**，然後開始鍵入 **計畫小時數** 的 **在此列中顯示** 的子菜單。

   >[!TIP]
   >
   >在文本模式下編輯資訊之前，請始終使用「標準」介面添加盡可能多的資訊。 添加最接近或包含您嘗試進行的計算的最大資訊量的欄位。

1. 在 **按以下方式匯總此列** 欄位，選擇 **和**，然後按一下 **完成**。
1. 按一下 **切換到文本模式** 的子菜單。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 替換 `valuefield ` 和 `aggregator.valuefield` 在以下文本模式示例中加亮線條的線條：

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >為了在分組中獲取匯總值以顯示「計畫小時數」和「實際小時數」欄位之間的匯總差，請將同一公式輸入到 `aggregator.valuefield` 。 的 `aggregator.displayformat` 用於「計畫小時數」列將分鐘數轉換為小時數。 由於「計畫小時數」欄位用作佔位符，因此無需調整此行。
   >
   >
   >的 `minutesAsHoursString` 定義 `aggregator.displayformat` 行表示無需按在 `valueexpression` 的下界。 在 `aggregator.valuefield=workRequired` 變為： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`。

1. 按一下 **保存+關閉**。
