---
product-area: reporting
navigation-topic: text-mode-reporting
title: 比較條件式格式中的欄位
description: 您可以使用條件式格式來比較檢視中的2個不同欄位，並在欄位之間符合特定條件時加以反白顯示。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 比較條件式格式中的欄位

您可以使用條件式格式來比較檢視中的2個不同欄位，並在欄位之間符合特定條件時加以反白顯示。

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
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的檢視</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限以編輯報表中的檢視</p> <p>管理檢視的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 範例：比較實際起始日期和計畫起始日期

例如，如果任務的實際起始日期晚於計畫起始日期，則可以使用條件格式來突出顯示「計畫起始日期」列。

要使用條件格式來比較任務的計畫起始日期和實際起始日期，請執行以下操作：

1. 轉至任務視圖或報表。
1. （條件性）若您使用報表，請從&#x200B;**欄（檢視）** 頁簽，按一下要有條件格式的列的標題以選擇它。\
   例如，選取 **實際開始日期** 欄位（通過比較「計劃開始日期」和「實際開始日期」欄位）來添加條件格式。

1. 按一下 **進階選項**，然後按一下「新增」 **此列的規則**.

1. 使用產生器中找到的現有值輸入比較條件，並指定條件式格式。\
   例如，我們要突出顯示實際開始日期晚於（或大於）計劃開始日期的任務。 選擇大於修改量，然後在日期欄位中選擇實際日期。\
     ![](assets/cond-format-1-350x84.png)

1. （選用）選取 **套用至整列** 如果要將格式應用到整行。
1. 按一下 **新增規則**，然後 **完成**.

1. 選取 **實際開始日期** 欄，然後按一下 **切換到文本模式**.

1. **按一下「 」以編輯文字** 模式，然後新增下列文字行：

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   在我們的範例中： 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >如果要比較Workfront原生欄位，請使用駝峰式大小寫語法來比較欄位名稱。 如果要比較自訂欄位，請使用 **DE：欄位的實際名稱** 對於要與第一個欄位比較的名稱欄位。\
   >例如，如果您要比較 **實際開始日期** 以標示為的自訂欄位 **傳送日期**，請在文字模式程式碼中新增下列陳述式：
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 確保 `righttext` 代碼行與 `rightmethod` 代碼行。

   ![](assets/cond-format-2-350x171.png)

1. 按一下&#x200B;**儲存**。
1. 按一下 **儲存+關閉**.

   欄會反白標示符合您條件的欄位。
