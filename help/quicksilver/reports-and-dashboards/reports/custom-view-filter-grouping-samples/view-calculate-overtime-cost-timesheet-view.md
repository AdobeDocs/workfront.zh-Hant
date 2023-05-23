---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：計算工時單視圖中的加班成本'
description: 在Adobe Workfront，預設情況下不計算加班時間，但您可以建立計算加班時間的時間表報告。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# 視圖：在工時單視圖中計算加班成本

在Adobe Workfront，預設情況下不計算加班時間，但您可以建立計算加班時間的時間表報告。

如果用戶在其配置檔案中與每小時成本費率關聯，您還可以計算該用戶的加班成本金額。\
有關將用戶與每小時成本費率關聯的資訊，請參閱文章 [配置我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

>[!NOTE]
>
>您可以添加到清單或報表中的時間表視圖的加班欄位顯示在時間表的「加班」欄位中找到的資訊。 此資訊由有權修改時間表的用戶手動更新。 有關工時單中「加班」欄位的詳細資訊，請參閱文章 [瞭解時間表佈局](../../../timesheets/timesheets/timesheet-layout.md)。

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

## 計算工時單視圖中的加班成本

要將計算的加班時間列添加到時間表視圖，請執行以下操作：

1. 轉至時間表清單或建立時間表報告。

   有關建立報告的資訊，請參閱文章 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 按一下 **自定義視圖** 的子菜單。

   或

   選擇 **列（視圖）** 頁籤。

1. 按一下 **添加列**。
1. 按一下 **切換到文本模式**。
1. 在 **在此列中顯示** 的 **按一下可編輯文本**。
1. 複製並貼上以下文本模式代碼 **文本模式** 對話框。
   <pre>displayname=已計算的加班成本<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}。{costPerHour},{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >此計算假定用戶通常每週工作40小時。

1. 按一下 **保存**，然後命名新視圖並按一下 **保存視圖** 的子菜單。

   或

   按一下 **保存+關閉** 在「時間表」報告中。

1. （可選和條件）如果要生成時間表報告，請指定報告的名稱，然後按一下 **保存報告**。

   每個用戶的加班成本顯示在 **計算的加班成本** 的雙曲餘切值。

   ![calculated_加班_成本_in_timesheet_report_png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
