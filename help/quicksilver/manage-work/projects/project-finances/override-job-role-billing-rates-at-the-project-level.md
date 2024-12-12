---
product-area: projects
navigation-topic: financials
title: 覆寫專案層級的工作角色收費率
description: 身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此工作角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# 覆寫專案層級的工作角色收費率

身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此工作角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。

本文說明如何覆寫專案的系統工作角色收費率。

如需有關覆寫專案的工作角色收費率以及計算專案收入的一般資訊，請參閱[覆寫工作角色收費率以及計算專案收入的總覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

如需有關哪一個工作角色用於計算專案收入的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

>[!NOTE]
>
>在實際收入中，套用至新增至標示為已記帳之記帳記錄時數的記帳費率，不應受記帳記錄記帳後發生的記帳費率覆寫影響。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案與財務資料的存取權</p> <p>工作角色的管理存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>管理包含編輯財務資料的專案許可權 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆寫專案層級的工作角色收費率

您可以透過下列方式覆寫專案上工作角色的計費率：

* 一次，藉由選取工作角色的新比率。\
  新費率會用於專案的整個期間，以計算收入。

* 多次，針對特定日期範圍選取數個新費率。\
  在每個指定日期範圍內可使用不同的費率。

>[!TIP]
>
>您無法覆寫專案的使用者收費率。

若要覆寫專案的收費率，請執行下列步驟：

1. 移至您要覆寫其計費率的專案。
1. 按一下左側面板中的&#x200B;**收費率**。 您可能需要先按一下「**顯示更多**」。
1. 按一下&#x200B;**新增收費率** > **新增收費率**。

   「新收費率」方塊開啟。

1. 在&#x200B;**工作角色**&#x200B;欄位中，選取您要變更收費率的工作角色。

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   **預設收費率**&#x200B;欄位會顯示此工作角色的系統層級費率。

1. 在&#x200B;**帳單費率1**&#x200B;欄位中，輸入單次帳單費率覆寫，然後按一下[儲存] **來覆寫單次帳單費率**

   或

   按一下&#x200B;**新增費率**&#x200B;以新增更多計費率覆寫。

1. （視條件而定）如果您新增多個計費率覆寫，請指定下列資訊：

   * **收費率1**：從專案開始到第一次覆寫第一個日期的收費率值。 這通常與&#x200B;**預設費率**&#x200B;相同。
   * **開始日期**：這是預設匯率結束的日期。
   * **結束日期**：新收費率覆寫結束的日期。

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. 您選取之日期的時區會顯示在「新增收費率」方塊的底部。 這是與您的Workfront執行個體相關聯的時區，如設定的客戶資訊區域所示。 如需詳細資訊，請參閱[設定您系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
1. Workfront會將覆寫工作角色費率套用至計算專案收入時指定的時間範圍內發生的小時。
1. 兩個覆寫率的時間範圍之間應該沒有間隙。 覆寫率的&#x200B;**開始日期**&#x200B;應該是緊接先前覆寫日期的&#x200B;**結束日期**&#x200B;之後的日期。

1. 您不能為第一個覆寫費率指定「開始日期」，也不能為最後一個覆寫費率指定「結束日期」。\
   我們建議您為第一個覆寫率使用預設率。\
   Workfront假設首次覆寫率適用於日期早於首次覆寫結束日期的所有時數，而上次覆寫率適用於日期晚於上次覆寫開始日期的所有時數。\
   如果在專案的計劃開始日期之前記錄了一小時，則使用第一個收費率。\
   如果是在專案的計畫完成日期後記錄一小時，則會使用最後收費率。

1. 按一下「**儲存**」。
