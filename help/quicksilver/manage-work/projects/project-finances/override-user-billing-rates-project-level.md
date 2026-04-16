---
content-type: overview
product-area: projects
navigation-topic: financials
title: 覆寫專案層級的使用者收費率
description: 本文說明如何覆寫專案的系統使用者收費率。
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 2%

---

# 覆寫專案層級的使用者收費率

身為專案經理，您可以指定特定專案上使用者的收費率。 此專案層級的收費率會覆寫此使用者之系統層級的收費率。 Workfront使用使用者的專案層級收費率來計算收入，而不使用系統層級收費率。

本文說明如何覆寫專案的系統使用者收費率。

如需有關覆寫專案的收費率以及計算專案收入的一般資訊，請參閱[覆寫收費率以及計算專案收入的概觀](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

如需有關計算專案收入的詳細資訊，請參閱[收入和成本階層概觀](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)以及文章[帳單和收入概觀](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)中的[根據使用者和角色指派的任務收入計算](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)區段。

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
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯專案與財務資料的存取權</p>
       <p><p>您也必須具備下列其中一項：</p> 
        <ul> 
          <li> <p>系統管理員存取層級。 </li> 
          <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <b>下啟用的兩個</b>使用者管理員<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理包含編輯財務資料的專案許可權 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆寫專案層級的使用者收費率

當您覆寫專案上使用者的收費率時，您可以指定有效日期，而且每個日期範圍都有不同的費率。 如果您未指定有效日期，則會針對專案的整個期間使用您輸入的帳單費率覆寫來計算收入。

若要覆寫專案的使用者收費率，請執行下列步驟：

1. 移至您要覆寫其計費率的專案。
1. 按一下左側面板中的&#x200B;**費率**。 您可能需要先按一下「**顯示更多**」。
1. 按一下&#x200B;**帳單**&#x200B;標籤（如果尚未選取）。
1. 按一下&#x200B;**新增收費率** > **新增使用者收費率**。

   「新增使用者收費率」方塊開啟。

1. 在&#x200B;**使用者**&#x200B;欄位中，選取您要變更收費率的使用者。
1. 選取要覆寫收費率的&#x200B;**貨幣**。
1. 在&#x200B;**收費率**&#x200B;欄位中，輸入第一個收費率覆寫。
1. （選擇性）按一下&#x200B;**新增日期有效費率**&#x200B;以新增更多計費費率覆寫。
1. （視條件而定）如果您要新增多重帳單費率覆寫，請為每一資料列指定下列資訊：

   * **收費率**：指定時段內的收費率值。
   * **開始日期**：開始覆寫收費率的日期。
   * **結束日期**：計費率覆寫結束的日期。

   ![顯示有效日期的新使用者收費率方塊](assets/new-user-billing-rate-on-project2.png)

   Workfront計算專案收入時，會將覆寫使用者費率套用至這些時間範圍內發生的小時。

   Workfront可讓您在覆寫時間範圍之間保留間隙，但您將會收到警告，確認這是刻意為之。

   您不需要為第一個覆寫費率指定「開始日期」，也不需要為最後一個覆寫費率指定「結束日期」。

   如果您只輸入一個計費費率覆寫，則該費率適用於整個專案期間。 如果您新增多個生效日期的覆寫，Workfront會假設第一個覆寫套用至其「結束日期」之前的所有時數，而最後一個覆寫套用至其「開始日期」之後的所有時數。

   Workfront假設首次覆寫率適用於日期早於首次覆寫結束日期的所有時數，而上次覆寫率適用於日期晚於上次覆寫開始日期的所有時數。

   如果在專案的計劃開始日期之前記錄了一小時，則使用第一個收費率。

   如果是在專案的計畫完成日期後記錄一小時，則會使用最後記帳費率。

1. 按一下「**儲存**」。
