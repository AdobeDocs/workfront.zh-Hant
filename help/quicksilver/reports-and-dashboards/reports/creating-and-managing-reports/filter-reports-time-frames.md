---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 依時間範圍篩選報表
description: 您可以依物件上現存日期的時間範圍來篩選報表。 例如，您可以篩選輸入時數之特定時間範圍的時數報告。
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: f78a86dcdf7b63e98bec5216fb5ab7622775a053
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 5%

---

# 依時間範圍篩選報表

<!-- Audited: 4/2025 -->

您可以依物件上現存日期的時間範圍來篩選報表。 例如，您可以篩選輸入時數之特定時間範圍的時數報告。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
      <td> 
      <p>新增：標準</p>
       <p> 或</p>
      <p>目前：計畫</p>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

必須先建立報表，然後才能篩選結果。

如需建立報告的詳細資訊，請參閱[建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 依日期的時間範圍篩選報表 {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. 按一下左上角的&#x200B;**新增報告**，然後選取您要建立的報告型別。

1. 在&#x200B;**新報告**&#x200B;頁面上，選取&#x200B;**篩選器**&#x200B;索引標籤。

1. 按一下&#x200B;**新增篩選規則**，然後&#x200B;**選取欄位**。

1. 在&#x200B;**選取欄位**&#x200B;對話方塊中，選取&#x200B;**小時**，然後選取&#x200B;**輸入日期**。
   ![依時間範圍篩選小時報告](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 在出現的下拉式清單中，選取下列其中一個選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">等於</td> 
      <td>選取此修正因子後，請指定輸入時數的日期。</td> 
     </tr>

   <tr> 
      <td role="rowheader">不等於</td> 
      <td>選取此修正因子後，請指定輸入時數的日期，以將此日期排除在報表之外。 報表會針對您指定的日期，顯示所有日期記錄的時數。</td> 
     </tr>

   <tr> 
      <td role="rowheader">小於</td> 
      <td>選取此修正因子後，請指定輸入時數之前的日期。 報表顯示在指定日期之前輸入的小時，不包括指定日期。</td> 
     </tr>

   <tr> 
      <td role="rowheader">小於和等於</td> 
      <td>選取此修正因子後，請指定輸入時數之前的日期。 報表顯示在指定日期（包括指定日期）之前輸入的小時。</td> 
     </tr>

   <tr> 
      <td role="rowheader">大於</td> 
      <td>選取此修正因子後，請指定輸入時數的日期。 報表顯示在指定日期之後輸入的小時，不包括指定日期。</td> 
     </tr>

   <tr> 
      <td role="rowheader">大於或等於</td> 
      <td> 選取此修正因子後，請指定輸入時數的日期。 報表顯示在指定日期（包括指定日期）之後輸入的小時。 </td> 
     </tr>

   <tr> 
      <td role="rowheader">介於</td> 
      <td>選取此修正因子後，請指定輸入時數的日期範圍。 報表會顯示輸入於指定日期之間的時數。</td> 
     </tr>

   <tr> 
      <td role="rowheader">Null</td> 
      <td>選取此修正因子可只顯示缺少「輸入日期」的小時。</td> 
     </tr>

   <tr> 
      <td role="rowheader">不是 Null</td> 
      <td>選取此修正因子以僅顯示「輸入日期」具有值的小時。</td> 
     </tr>

   </tbody> 
   </table>

1. 按一下「**儲存並關閉**」。

## 內建時間範圍修飾元 {#built-in-timeframe-modifiers}

Adobe Workfront有內建的時間範圍修飾元，您無需定義特定日期即可使用。 這些修飾詞適用於篩選器中的任何日期欄位，或任何報表中的提示。

例如，如果您正在建立時數報表，而且想要顯示特定時間範圍內輸入的時數，您可以從下列內建時間範圍篩選選項中選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今天</td> 
   <td>顯示輸入日期為今天的小時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本週</td> 
   <td>顯示「輸入日期」為本週中日期的時數，其中周從星期日開始，到星期六結束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下週</td> 
   <td>顯示「輸入日期」為本週後一週內日期的時數，其中一週從星期日開始，到星期六結束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">上週</td> 
   <td>顯示「輸入日期」為本週前一週中日期的小時，其中一週從星期日開始，到星期六結束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本月</td> 
   <td>顯示「輸入日期」為當月日期的小時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下個月</td> 
   <td>顯示「輸入日期」為目前月份後一個月中日期的小時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上個月</td> 
   <td>顯示「輸入日期」為目前月份前一個月中日期的小時</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本季度</td> 
   <td> <p>顯示「輸入日期」為本季日期的小時，其中季度定義為：</p> 
    <ul> 
     <li>第一季： 1月1日至3月30日</li> 
     <li>第二季： 4月1日至6月30日</li> 
     <li>第三季： 7月1日至9月30日</li> 
     <li>第四季： 10月1日至12月31日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">下個季度</td> 
   <td>顯示「輸入日期」為本季後一季中的日期（其中上定義了季度）的小時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上個季度</td> 
   <td> <p>顯示「輸入日期」為本季前一個季度之日期的小時，其中季度定義於上面。</p> <p>注意：如果您的Workfront管理員已啟用並定義系統的自訂季度，則季度的內建篩選器會取代為您的自訂季度資訊。 如需啟用自訂季數的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">啟用專案的自訂季數</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>顯示「輸入日期」為目前年份中日期的小時，其中目前年份從1月1日開始，到12月31日結束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">過去一年</td> 
   <td>顯示「輸入日期」為過去一年的日期時的小時，其中過去一年的開始日期為目前日期之前的12個月。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">去年</td> 
   <td> <p>顯示「輸入日期」為去年日期的時數，其中去年從1月1日開始，結束日期為今年之前一年的12月31日。</p> <p>備註：會計年度沒有內建時間期間。 您可以建立報表，並使用會計年度日期範圍的自訂修正因子依日期篩選資訊，如您的組織中所定義。 如果您想要即時選擇財政年度的時間範圍，則應該使用提示而非篩選器。 </p> </td> 
  </tr> 
 </tbody> 
</table>
