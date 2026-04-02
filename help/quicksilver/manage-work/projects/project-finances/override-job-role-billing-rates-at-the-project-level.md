---
product-area: projects
navigation-topic: financials
title: 覆寫專案層級的工作角色收費率
description: 身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此工作角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 2%

---

# 覆寫專案層級的工作角色收費率

{{highlighted-preview}}

身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此工作角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。

本文說明如何覆寫專案的系統工作角色收費率。

如需有關覆寫專案的工作角色收費率和計算專案收入的一般資訊，請參閱[覆寫收費率和計算專案收入的概觀](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

如需有關哪一個工作角色用於計算專案收入的詳細資訊，請參閱[收入與成本階層概要](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)以及文章[帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)中的[根據使用者和角色指派的任務收入計算](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)區段。

>[!NOTE]
>
>在實際收入中，套用至新增至標示為已記帳之記帳記錄時數的記帳費率，不應受記帳記錄記帳後發生的記帳費率覆寫影響。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td> <p>覆寫專案的工作角色收費率：任何Workfront或Workflow套件</p>
        <p>若要將屬性套用至工作角色：工作流程Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯專案與財務資料的存取權</p> <p>工作角色的管理存取權</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理包含編輯財務資料的專案許可權 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆寫專案層級的工作角色收費率

當您修訂專案上工作的收費率時，您可以指定有效日期，而每個日期範圍都有不同的費率。 如果您未指定有效日期，則會針對專案的整個期間使用您輸入的帳單費率覆寫來計算收入。

您可以將新的收費率新增至專案範本，當您從該範本建立專案時，這些收費率就會成為專案收費率。 如需有關編輯範本的資訊，請參閱[編輯專案範本](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)。

>[!TIP]
>
>除非您有Workflow Ultimate套件，否則無法覆寫專案的使用者收費率。

若要覆寫專案的收費率，請執行下列步驟：

1. 移至您要覆寫其計費率的專案。
1. 按一下左側面板中的&#x200B;**收費率**。

   或

   <span class="preview">按一下左側面板中的&#x200B;**費率**，然後按一下&#x200B;**帳單**&#x200B;標籤（如果尚未選取）。</span>

1. 按一下&#x200B;**新增收費率** > **新增收費率**。

   或

   <span class="preview">按一下&#x200B;**新增收費率>新工作角色收費率**。</span>

   「新收費率」方塊開啟。

1. 在&#x200B;**工作角色**&#x200B;欄位中，選取您要變更收費率的工作角色。

1. <span class="preview">（選擇性）選取收費率的任何屬性，例如代理商或地點。</span>

   <span class="preview">系統管理員在[設定]區域中定義速率屬性。</span>

1. 選取要覆寫收費率的&#x200B;**貨幣**。
1. 在&#x200B;**收費率**&#x200B;欄位中輸入收費率覆寫，然後按一下&#x200B;**儲存**&#x200B;來覆寫一次收費率

   或

   按一下&#x200B;**新增費率**&#x200B;以新增更多計費率覆寫。

1. （視條件而定）對於日期有效帳單費率修訂，請為各資料列輸入下列資訊：

   * **收費率**：從專案開始到第一次覆寫第一個日期的收費率值。
   * **開始日期**：開始覆寫收費率的日期。
   * **結束日期**：收費率覆寫結束的日期。

   ![覆寫日期的收費率](assets/new-job-role-billing-rate-on-project2.png)

   Workfront在計算專案收入時，會將覆寫工作角色費率套用至這些時間範圍內發生的小時。

   Workfront可讓您在覆寫時間範圍之間保留間隙，但您將會收到警告，確認這是刻意為之。

   您不需要為第一個覆寫費率指定「開始日期」，也不需要為最後一個覆寫費率指定「結束日期」。

   如果您只輸入一個計費費率覆寫，則該費率適用於整個專案期間。 如果您新增多個生效日期的覆寫，Workfront會假設第一個覆寫套用至其「結束日期」之前的所有時數，而最後一個覆寫套用至其「開始日期」之後的所有時數。

   Workfront假設首次覆寫率適用於日期早於首次覆寫結束日期的所有時數，而上次覆寫率適用於日期晚於上次覆寫開始日期的所有時數。

   如果在專案的計劃開始日期之前記錄了一小時，則使用第一個收費率。

   如果是在專案的計畫完成日期後記錄一小時，則會使用最後記帳費率。

1. 按一下「**儲存**」。
