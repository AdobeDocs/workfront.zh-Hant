---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：計算工時單視圖中的加班成本'
description: Adobe Workfront預設不計算加班時間，但您可以建立計算加班時間的時間表報表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 查看：在工時單視圖中計算加班成本

Adobe Workfront預設不計算加班時間，但您可以建立計算加班時間的時間表報表。

如果用戶在其配置檔案中與每小時成本費率關聯，您也可以計算該用戶的特定時段成本金額。\
有關將用戶與每小時成本費率關聯的資訊，請參閱文章 [配置我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>可以添加到清單或報表中的「時間表」視圖的「特定時間」欄位顯示在時間表的「特定時間」欄位中找到的資訊。 此資訊由有權修改時間表的用戶手動更新。 有關工時單中的「加班」欄位的詳細資訊，請參閱文章 [了解工時單佈局](../../../timesheets/timesheets/timesheet-layout.md).

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

## 在工時單視圖中計算加班成本

要將計算的「加班」列添加到時間表視圖，請執行以下操作：

1. 轉到時間表清單，或建立時間表報告。

   如需建立報表的相關資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 按一下 **自訂檢視** 在時間表清單中。

   或

   選取 **欄（檢視）** 頁簽。

1. 按一下 **添加列**.
1. 按一下 **切換到文本模式**.
1. 在 **顯示在此列中** 按一下 **按一下「 」以編輯文字**.
1. 複製下列文字模式程式碼並貼到 **文字模式** 對話框。
   <pre>displayname=計算加班成本<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}。{costPerHour},{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >此計算假設使用者通常每週工作40小時。

1. 按一下 **儲存**，然後為新檢視命名，然後按一下 **保存視圖** 在時間表清單中。

   或

   按一下 **儲存+關閉** 在「時間表」報告中。

1. （可選和條件性）如果要構建時間表報告，請指定報告的名稱，然後按一下 **儲存報表**.

   每個使用者的加班成本會顯示在 **計算的加班成本** 欄。

   ![calculated_overtimed_cost_in_timestee_report_png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
