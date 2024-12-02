---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：在時程表檢視表中計算加班成本
description: Adobe Workfront預設不會計算加班，但您可以建立計算加班的時程表報表。
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# 檢視：在時程表檢視中計算加班成本

<!--Audited: 11/2024-->

Adobe Workfront預設不會計算加班，但您可以建立計算加班的時程表報表。

如果使用者與其設定檔中的每小時成本費率相關聯，您也可以計算該使用者加班的成本金額。\
如需將使用者與每小時成本費率建立關聯的資訊，請參閱文章[設定我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

>[!NOTE]
>
>您可以在清單或報告中新增至時程表檢視的「加班」欄位會顯示時程表的「加班」欄位中找到的資訊。 這項資訊會由有權修改時程表的使用者手動更新。 如需時程表中超時欄位的詳細資訊，請參閱文章[時程表配置概觀](../../../timesheets/timesheets/timesheet-layout.md)。

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在時程表檢視表中計算加班成本

若要將已計算的「加班」欄新增至時程表檢視：

1. 前往時程表清單。

1. 按一下&#x200B;**檢視**&#x200B;下拉式功能表，然後按一下&#x200B;**新增檢視**。

1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 在&#x200B;**編輯文字模式**&#x200B;方塊中，移除方塊中的文字，然後複製並貼上下列文字模式程式碼：

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >此計算假設使用者通常每週工作40小時。

1. 按一下&#x200B;**完成**，然後命名新檢視並在時程表清單中按一下&#x200B;**儲存檢視**。

   每個使用者的加班成本會顯示在&#x200B;**已計算的加班成本**&#x200B;欄中。


