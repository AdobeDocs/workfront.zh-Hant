---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選器：比較兩個欄位來排除清單中的專案」
description: 您可以比較清單中兩個欄位，藉此篩選清單中的專案。 例如，您只能顯示任務的實際完成日期晚於計畫完成日期的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 篩選器：比較兩個欄位來排除清單中的專案

您可以比較清單中兩個欄位，藉此篩選清單中的專案。 例如，您只能顯示任務的實際完成日期晚於計畫完成日期的任務。

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 比較兩個欄位以篩選專案

1. 前往工作清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. 按一下&#x200B;**新增篩選器規則**&#x200B;並新增&#x200B;**實際完成日期** >**大於** > **選取日期**。

   >[!TIP]
   >
   >選擇您要用於所選欄位的過濾條件修正因子（若有）。

1. 按一下&#x200B;**切換到文字模式**。
1. 在&#x200B;**設定報表**&#x200B;的篩選規則區域中，新增下列程式碼：

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存篩選器**。
