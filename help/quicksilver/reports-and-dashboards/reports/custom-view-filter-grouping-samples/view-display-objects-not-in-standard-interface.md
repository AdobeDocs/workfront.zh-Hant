---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：顯示未包含在標準介面中的對象'
description: 可以在未包含在標準模式介面中的視圖對象中顯示。 您只能透過文字模式來參照，才能執行此作業。 您可以透過下列其中一種方式（編輯我）來判斷哪些欄位可包含在檢視中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 視圖：顯示未包含在標準介面中的對象

可以在未包含在標準模式介面中的視圖對象中顯示。 您只能透過文字模式來參照，才能執行此作業。\
您可以透過下列其中一種方式，決定檢視中可包含哪些欄位：

* 使用 [API Explorer](https://one.workfront.com/s/api-explorer) 以發現可以通過文本模式引用的其他對象。\
   並非API資源管理器中記錄的所有欄位都是文本模式的有效欄位。 有些欄位只能透過API報告。

* 在欄中找到物件的ID欄位。 大多數具有欄位ID的對象也具有相應的列或欄位名稱，這些名稱可能無法通過標準模式介面訪問。

   您可以使用文字模式來取代 `fieldnameID` 和 `fieldname:name`.

   例如，在標準模式介面中， **Portfolio擁有者ID** 欄位可供專案檢視，但 **Portfolio所有者名稱** 欄位不是。 您可以使用文字模式來顯示 **Portfolio所有者名稱** 在檢視的欄中。

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

## 範例：將「Portfolio擁有者名稱」欄新增至專案檢視

1. 前往專案清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖**.

1. 按一下 **添加列** 然後開始在 **顯示在此列中** 欄位，然後在清單中顯示時選取它。

1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 取代 `valuefield` 行(`valuefield=portfolio:ownerID`)，並加上下列行：

   ```
   valuefield=portfolio:owner:name
   ```

   或

   移除您在 **文字模式** 框中，並將其替換為以下代碼：

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   在此特定範例中，報表會依Portfolio擁有者ID來排序報表，如 `querysort` 行。

   >[!TIP]
   >
   >替換任何欄位 `ID` 和欄位 `name` 使用文字模式，一律取代 `ID` with `:name` 在 `valuefield` 行。

1. 按一下 **儲存**，然後 **保存視圖**.
