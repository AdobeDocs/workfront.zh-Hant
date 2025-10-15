---
product-area: reporting
navigation-topic: text-mode-reporting
title: 比較條件式格式的欄位
description: 您可以使用條件式格式來比較檢視中的2個不同欄位，並在欄位之間符合特定條件時反白顯示它們。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# 比較條件式格式的欄位

<!-- Audited: 1/2025 -->

您可以使用條件式格式來比較檢視中的2個不同欄位，並在欄位之間符合特定條件時反白顯示它們。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
     <p>標準</p>
     <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的檢視</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報告的許可權以編輯報告中的檢視</p> <p>管理檢視的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 範例：比較實際開始日期與計劃開始日期

例如，如果任務的實際開始日期在計劃開始日期之後，您可以使用條件式格式來反白計劃開始日期欄。

若要使用條件式格式來比較任務的計劃開始日期與實際開始日期：

1. 前往任務檢視或報告。
1. （視條件而定）如果您正在使用報表，請從報表編輯器中的&#x200B;**欄（檢視）**&#x200B;索引標籤按一下要視條件格式化之欄的標題以選取它。\
   例如，如果您要透過比較「計劃開始日期」與「實際開始日期」欄位，將條件式格式新增至欄位，請選取&#x200B;**實際開始日期**&#x200B;欄。

1. 按一下[進階選項]****，然後按一下[新增此資料行的&#x200B;**規則]**。

1. 使用在產生器中找到的現有值輸入比較條件，並指定您的條件式格式。\
   例如，我們要反白顯示實際開始日期晚於（或大於）計劃開始日期的任務。 選取「大於」修正因子，然後在日期欄位中選取實際日期。

   ![實際開始日期的條件式格式](assets/cond-format-1-350x84.png)

1. （選擇性）如果要套用格式至整列，請選取&#x200B;**套用至整列**。
1. 按一下「**儲存**」。

1. 選取&#x200B;**實際開始日期**&#x200B;欄，然後按一下&#x200B;**切換到文字模式**。

1. 按一下&#x200B;**編輯文字模式**，然後新增下列文字行：

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   在我們的範例中：

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >如果您要比較Workfront原生欄位，請使用駝峰式大小寫語法來取得欄位名稱。 如果您要比較自訂欄位，請針對要與第一個欄位比較的名稱欄位，使用欄位&#x200B;**的:ActualDE**&#x200B;名稱。\
   >例如，如果您要比較&#x200B;**實際開始日期**&#x200B;與標示為&#x200B;**傳送日期**&#x200B;的自訂欄位，請在文字模式程式碼中新增下列陳述式：
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 請確定`righttext`行程式碼符合`rightmethod`行程式碼中的陳述式。

   ![條件式格式](assets/cond-format-2-350x171.png)

1. 按一下「**儲存**」。
1. 按一下「**儲存並關閉**」。

   欄會反白顯示符合條件的欄位。
