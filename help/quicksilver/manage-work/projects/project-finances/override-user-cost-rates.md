---
content-type: overview
product-area: projects
navigation-topic: financials
title: 修訂專案層次的使用者成本費率
description: 本文說明如何覆寫專案的系統使用者成本費率。
author: Lisa
feature: Work Management
exl-id: ff1110fd-2d24-48a7-8000-712e551ca61a
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 3%

---

# 覆寫專案層次的使用者成本費率

您可以指定使用者在特定專案上的成本費率。 此專案層次成本費率會覆寫此使用者之系統層次的成本費率。 Workfront使用工作角色的專案層次成本費率來計算成本，而不使用系統層次成本費率。

本文說明如何覆寫專案的系統使用者成本費率。

如需有關計算專案成本的詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)和[追蹤成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

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
   <td>管理包含編輯成本費率的專案許可權 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

使用者必須在其使用者設定檔上啟用&#x200B;**允許成本費率覆寫**&#x200B;欄位。 當使用者未啟用成本覆寫欄位時，不允許該使用者在任何專案上的成本覆寫，且系統會使用使用者設定檔上的費率來計算成本。

如需詳細資訊，請參閱[編輯使用者的設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 覆寫專案層次的使用者成本費率

1. 移至您要覆寫成本費率的專案。
1. 按一下左側面板中的&#x200B;**費率**。 您可能需要先按一下「**顯示更多**」。
1. 按一下&#x200B;**成本**&#x200B;標籤（如果尚未選取）。
1. 按一下&#x200B;**新增成本費率** > **新使用者成本費率**。

   「新增使用者成本費率」方塊開啟。

1. 在&#x200B;**使用者**&#x200B;欄位中，選取您要變更其成本費率的使用者。
1. 選取成本費率覆寫的&#x200B;**貨幣**。
1. 在&#x200B;**成本費率**&#x200B;欄位中輸入第一個成本費率覆寫。
1. （選擇性）按一下&#x200B;**新增日期有效費率**&#x200B;以新增更多成本費率覆寫。

   >[!NOTE]
   >
   >如果您輸入單一費率覆寫，則適用於專案的整個生命週期。
   >如果您想要在一段時間內使用不同的費率，可以新增多個生效日期覆寫。

1. （視條件而定）如果您要新增多重成本費率修訂，請為每一資料列指定下列資訊：

   * **成本費率**：指定期間內的成本費率值。
   * **開始日期**：成本費率覆寫開始的日期。
   * **結束日期**：成本費率覆寫結束的日期。

   ![顯示有效日期的新使用者成本費率方塊](assets/new-user-cost-rate-box.png)

   計算專案成本時，Workfront會將覆寫工作角色費率套用至這些時間範圍內發生的小時。

   Workfront可讓您在覆寫時間範圍之間保留間隙，但您將會收到警告，確認這是刻意為之。

   您不需要為第一個覆寫費率指定「開始日期」，也不需要為最後一個覆寫費率指定「結束日期」。

   我們建議您為第一個覆寫率使用預設率。

   Workfront假設首次覆寫率適用於日期早於首次覆寫結束日期的所有時數，而上次覆寫率適用於日期晚於上次覆寫開始日期的所有時數。

   如果在專案的計劃開始日期之前記錄了一小時，則使用第一個成本費率。

   如果在專案的計畫完成日期後記錄一小時，則使用最後的成本費率。

1. 按一下「**儲存**」。
