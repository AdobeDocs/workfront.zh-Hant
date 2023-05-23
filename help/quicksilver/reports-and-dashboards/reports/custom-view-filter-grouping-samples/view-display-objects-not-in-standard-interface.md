---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：顯示未包括在標準介面中的對象」'
description: 可以在未包括在標準模式介面中的視圖對象中顯示。 只有通過文本模式引用它們，才能執行此操作。 您可以通過以下任一方式確定視圖中可以包括哪些欄位 — 「編輯我」。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 視圖：顯示未包含在標準介面中的對象

可以在未包括在標準模式介面中的視圖對象中顯示。 只有通過文本模式引用它們，才能執行此操作。\
您可以通過以下任一方法確定視圖中可以包括哪些欄位：

* 使用 [API資源管理器](../../../wf-api/general/api-explorer.md) 查找可以通過文本模式引用的其他對象。\
   並非API資源管理器中記錄的所有欄位都是文本模式的有效欄位。 某些欄位僅通過API報告。

* 在列中查找對象的ID欄位。 具有欄位ID的大多數對象還具有相應的列或欄位名，這些列或欄位名可能無法通過標準模式介面訪問。

   可以使用文本模式在視圖中包括列或欄位名稱，而不是ID，方法是替換 `fieldnameID` 和 `fieldname:name`。

   例如，在標準模式介面中， **Portfolio所有者ID** 欄位可用於項目視圖，但 **Portfolio所有者名稱** 欄位不是。 可以使用文本模式顯示 **Portfolio所有者名稱** 的子菜單。

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
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 示例：將「Portfolio所有者名稱」列添加到項目視圖

1. 轉到項目清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 然後在中鍵入「Portfolio所有者ID」 **在此列中顯示** 的子菜單。

1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 替換 `valuefield` 行(`valuefield=portfolio:ownerID`)，其行如下：

   ```
   valuefield=portfolio:owner:name
   ```

   或

   刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   在此特定示例中，報告將按Portfolio所有者ID對報告進行排序，如 `querysort` 。

   >[!TIP]
   >
   >替換任何欄位 `ID` 和 `name` 使用文本模式始終替換 `ID` 與 `:name` 的 `valuefield` 。

1. 按一下 **保存**，則 **保存視圖**。
