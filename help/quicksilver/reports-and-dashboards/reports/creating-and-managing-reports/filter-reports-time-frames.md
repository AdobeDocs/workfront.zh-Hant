---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 依時間範圍篩選報表
description: 您可以依物件上存在之日期的時間範圍來篩選報表。 例如，您可以篩選小時報表，以找出輸入小時的特定時間範圍。
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# 依時間範圍篩選報表

您可以依物件上存在之日期的時間範圍來篩選報表。 例如，您可以篩選小時報表，以找出輸入小時的特定時間範圍。

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

## 必要條件

必須先建立報表，才能篩選其結果。

如需建立報表的詳細資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 依日期的時間範圍篩選報表 {#filter-a-report-by-the-time-frame-of-a-date}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **報表**.

1. 按一下 **新增報表**，然後選取您想要的報表類型。\
   例如，選取 **小時報告**.

1. 選取 **篩選器** 標籤。
1. 按一下 **新增篩選規則**，然後選取 **小時參加日期**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 在下列下拉式功能表中，選取下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">等於</td> 
      <td>選擇此修改量後，指定輸入小時的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不等於</td> 
      <td>選擇此修改量後，指定輸入小時的日期，以從報表中排除此日期。 報表會顯示所有日期的記錄時數（預計為您指定的日期）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">空</td> 
      <td>選擇此修改量以僅顯示「錄入日期」缺失的小時。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非空</td> 
      <td>選擇此修改量以僅顯示錄入日期具有值的小時。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">介於</td> 
      <td>選擇此修改量後，指定輸入小時數的日期範圍。 報表會顯示指定日期之間所輸入的小時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">小於</td> 
      <td>選擇此修改量後，請指定小時輸入前的日期。 報表會顯示在指定日期之前輸入的小時數，而不包括指定日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">小於和等於</td> 
      <td>選擇此修改量後，請指定小時輸入前的日期。 報表會顯示在指定日期（包括指定日期）之前輸入的小時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大於</td> 
      <td>選擇此修改量後，請指定輸入小時的日期。 報表會顯示在指定日期之後輸入的小時數，而不包括指定日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大於或等於</td> 
      <td> <p>選擇此修改量後，請指定輸入小時的日期。 報表會顯示在指定日期（包括指定日期）之後輸入的小時數。</p> <p>選擇任何內置時間框架修飾符，如 <a href="#built-in-time-frame-modifiers" class="MCXref xref">內建時間框架修飾元</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 這些修改量適用於篩選器中的任何日期欄位，或任何報表中的提示。
1. 按一下 **儲存+關閉**.

## 內建時間框架修飾元 {#built-in-time-frame-modifiers}

Adobe Workfront有內建的時間範圍修飾元，您不需定義特定日期即可使用。 

這些修改量適用於篩選器中的任何日期欄位，或任何報表中的提示。 

如需如何依與日期相關聯的時間範圍篩選報表的詳細資訊，請參閱  [依日期的時間範圍篩選報表](#filter-a-report-by-the-time-frame-of-a-date).

例如，如果您要建立小時報表，並想要顯示在特定時間範圍內輸入的小時數，則可以從以下內建的時間範圍篩選選項中進行選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今天</td> 
   <td>顯示「登入日期」為今天的小時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本周</td> 
   <td>顯示「登入日期」是當週日期的小時，該周從星期日開始，到星期六結束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下周</td> 
   <td>顯示「登入日期」是當周後一週中的日期的小時，該周從星期日開始，到星期六結束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">上週</td> 
   <td>顯示「登入日期」是當周前一週中的日期的小時，該周從星期日開始，到星期六結束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本月</td> 
   <td>顯示當月的「登入日期」為日期的小時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下個月</td> 
   <td>顯示「登入日期」是當月後月份中的日期的小時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上個月</td> 
   <td>顯示「登入日期」是當月前月份中的日期的小時數</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本季度</td> 
   <td> <p>顯示當前季度中的「錄入日期」為日期的小時數，其中季度定義為：</p> 
    <ul> 
     <li>第一季度：1月1日 — 3月30日</li> 
     <li>第二季度：4月1日 — 6月30日</li> 
     <li>第三季度：7月1日 — 9月30日</li> 
     <li>第四季度：10月1日至12月31日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">下個季度</td> 
   <td>顯示「登入日期」是當前季度後的季度中的日期的小時數，其中已定義了季度。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上個季度</td> 
   <td> <p>顯示「登入日期」是當前季度之前的季度中的日期的小時，其中已定義季度。</p> <p>注意：如果您的Workfront管理員已為您的系統啟用並定義自訂季別，季別的內建篩選器將替換為您的自訂季度資訊。 有關啟用自定義季度的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">啟用項目的自定義季數</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>顯示「登入日期」為當年日期的小時數，當年從1月1日開始，到12月31日結束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">過去一年</td> 
   <td>顯示「登入日期」是過去一年中的日期的小時數，過去一年從當前日期前12個月開始。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">去年</td> 
   <td> <p>顯示「登入日期」是去年日期的小時數，其中去年從1月1日開始，到當年前一年的12月31日結束。</p> <p>注意：會計年度沒有內建的時段。 您可以使用自訂修改量，按照組織中的定義，為會計年度的日期範圍建立報表並依日期篩選資訊。 如果您想要現場選擇某個會計年度的時間範圍，則應使用提示，而不是篩選器。 </p> </td> 
  </tr> 
 </tbody> 
</table>
