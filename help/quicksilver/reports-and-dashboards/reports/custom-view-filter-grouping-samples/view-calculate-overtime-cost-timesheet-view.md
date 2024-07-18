---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：在時程表檢視中計算加班成本」
description: Adobe Workfront預設不會計算加班，但您可以建立計算加班的時程表報表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# 檢視：在時程表檢視中計算加班成本

Adobe Workfront預設不會計算加班，但您可以建立計算加班的時程表報表。

如果使用者與其設定檔中的每小時成本費率相關聯，您也可以計算該使用者加班的成本金額。\
如需將使用者與每小時成本費率建立關聯的資訊，請參閱文章[設定我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

>[!NOTE]
>
>您可以在清單或報告中新增至時程表檢視的「加班」欄位會顯示時程表的「加班」欄位中找到的資訊。 這項資訊會由有權修改時程表的使用者手動更新。 如需時程表中超時欄位的詳細資訊，請參閱文章[時程表配置概觀](../../../timesheets/timesheets/timesheet-layout.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 在時程表檢視表中計算加班成本

若要將已計算的「加班」欄新增至時程表檢視：

1. 前往時程表清單，或建立時程表報告。

   如需有關建立報告的資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 在時程表清單中按一下&#x200B;**自訂檢視**。

   或

   選取時程表報告中的&#x200B;**欄（檢視）**&#x200B;標籤。

1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**。
1. 在&#x200B;**顯示在此欄**&#x200B;區域中，按一下&#x200B;**按一下以編輯文字**。
1. 在&#x200B;**文字模式**&#x200B;對話方塊中，複製並貼上下列文字模式程式碼。
   <pre>displayname=計算的加班成本<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40，({totalHours}-40)*{user}。{costPerHour}，{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >此計算假設使用者通常每週工作40小時。

1. 按一下[儲存]****，然後命名新檢視，再按一下時程表清單中的[儲存檢視]****。

   或

   在時程表報表中按一下&#x200B;**儲存+關閉**。

1. （選擇性和條件性）如果您要建立時程表報告，請指定報告的名稱，然後按一下&#x200B;**儲存報告**。

   每個使用者的加班成本會顯示在&#x200B;**已計算的加班成本**&#x200B;欄中。

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
