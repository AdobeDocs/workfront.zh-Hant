---
product-area: projects
navigation-topic: financials
title: 在項目層改寫任務職責開單費率
description: 作為項目經理，您可以指定特定項目上某個職務角色的計費費率。 此項目層開單費率將改寫此職務職責的系統層開單費率。 Workfront會使用工作角色的專案層開單比率來計算收入，而非使用系統層開單比率。
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 在項目層改寫任務職責開單費率

作為項目經理，您可以指定特定項目上某個職務角色的計費費率。 此項目層開單費率將改寫此職務職責的系統層開單費率。 Workfront會使用工作角色的專案層開單比率來計算收入，而非使用系統層開單比率。

本文介紹如何改寫項目的系統職務開單費率。

有關改寫項目職務責任開單費率和計算項目收入的一般資訊，請參閱 [改寫任務職責開單費率和計算項目收入概覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

有關使用哪個職務來計算項目收入的詳細資訊，請參閱文章中的「了解基於用戶和角色分配的任務的收入計算」部分 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>在實際收入情況下，應用於添加到標籤為「開單」的開單記錄的小時的開單費率，不應受在開單記錄開單後發生的開單費率改寫的影響。

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
   <td> <p>編輯對項目和財務資料的訪問</p> <p>作業角色的管理存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理包含編輯財務資料之專案的權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在項目層改寫任務職責開單費率

您可以通過以下方式改寫項目上職務職責的開單費率：

* 一次，為作業角色選擇新費率。\
   新比率會用於專案的整個期間，以計算收入。

* 選取特定日期範圍的數個新費率，即可多次。\
   在每個指定日期範圍內都可以使用不同的比率。

>[!TIP]
>
>您不能改寫項目的用戶開單率。

要改寫項目的開單率，請執行以下操作：

1. 轉到要改寫開單費率的項目。
1. 按一下 **計費率** 中。 您可能必須先按一下 **顯示更多**.
1. 按一下 **添加計費率** > **新計費率**.

   「新開單費率」框開啟。

1. 在 **工作角色** 欄位中，選擇要更改開單費率的職務職責。

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   此 **預設開單率** 欄位顯示此作業角色的系統級別比率。

1. 在 **計費率1** 欄位，輸入一次性開單費率改寫，然後按一下 **儲存** 要改寫一次開單費率

   或

   按一下 **新增率** 添加更多開單費率改寫。

1. （條件性）如果要添加多個開單費率改寫，請指定以下資訊：

   * **計費率1**:從項目開始到第一個改寫的第一個日期的開單費率值。 這通常與 **預設比率**.
   * **開始日期**:這是「預設比率」結束的日期。
   * **結束日期**:新開單費率改寫結束的日期。

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. 所選日期的時區顯示在「新開單費率」框的底部。 這是與您的Workfront例項相關聯的時區，如「設定」的「客戶資訊」區域所示。 如需詳細資訊，請參閱 [配置系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront會將覆寫職務角色比率套用至計算專案收入時，在指定時間範圍內發生的小時數。
1. 兩個覆蓋率的時間範圍之間不應有間隙。 此 **開始日期** 的值應為緊接在 **結束日期** 上一個覆蓋日期。

1. 您不能為第一個改寫率指定「開始日期」，也不能為最後一個改寫率指定「結束日期」。\
   建議您對第一個覆蓋率使用預設比率。\
   Workfront假設第一個覆蓋率應用於日期早於第一個覆蓋的結束日期的所有小時，並且最後一個覆蓋率應用於日期晚於最後一個覆蓋的開始日期的所有小時。\
   如果在項目的「計劃開始日期」之前記錄了一小時，則會使用第一個計費率。\
   如果在項目的計畫完成日期之後記錄了一個小時，則使用最後的開單費率。

1. 按一下&#x200B;**儲存**。
