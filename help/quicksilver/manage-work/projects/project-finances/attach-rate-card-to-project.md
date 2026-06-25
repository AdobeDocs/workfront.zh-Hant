---
title: 將費率卡附加至專案
description: 當您在專案中附加費率卡時，所有角色及其相關收費率都會新增至專案。
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
TQID: https://experienceleague.adobe.com/waVWQfq2YqgDXZx3wl0ahzuQx7UJ78S1kYY8xBgi5OQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0ae6286f0c76f638358839603fba1301d5557d83
workflow-type: tm+mt
source-wordcount: 564
ht-degree: 3%

---

# 將費率卡附加至專案

費率卡會根據屬性儲存每個工作角色的多個收費率。 例如，代理商A的工作角色為位於巴黎的Designer，代理商B的工作角色為另一個位於巴黎的Designer，而位於紐約的第三個Designer未指派給代理商，每個代理商的計費率不同。 不過，費率卡上的工作角色不需要屬性。 屬性可作為工具，用來建立更精細的速率。 費率卡上的收費率也可以是生效日期，因此費率在指定日期開始和結束。

當您在專案中附加費率卡時，所有角色及其相關收費率都會新增至專案。

>[!NOTE]
>
>附加費率卡會覆寫專案上任何現有的費率卡收費率。 不會移除直接新增至專案的記帳費率覆寫。

如需有關建立費率卡的資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

如需有關覆寫專案的工作角色收費率和計算專案收入的一般資訊，請參閱[覆寫收費率和計算專案收入的概觀](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

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
   <td>編輯專案、財務資料和費率卡的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理具有編輯收費率許可權之專案的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將費率卡附加至專案

1. 前往專案。
1. 按一下左側面板中的&#x200B;**費率**，然後選取&#x200B;**帳單**。
1. 按一下&#x200B;**新增收費率>附加費率卡**。

   **附加速率卡**&#x200B;方塊開啟。 您可以在清單中搜尋費率卡。

   ![附加費率卡盒](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >費率卡上的「群組」和「公司」會作為此清單上的篩選器。 由於專案也包含「群組」和「公司」欄位，Workfront會使用這些值，將可用的費率卡片清單縮小至與專案內容相關的清單，而非整個系統內的所有費率卡。
   >
   >相符項不一定是精確的。 依專案的群組/公司組態，包含空白群組和/或公司值的費率卡仍可能會出現。 例如，如果專案已選取「群組」，但「公司」空白，您可能會看到與該「群組」相關聯的費率卡，即使費率卡的「公司」不同或空白。

1. 選取要新增至專案的費率卡，然後按一下&#x200B;**附加**。

   費率卡及其所有工作角色費率會新增至計費費率清單。

   ![將評等卡新增至專案](assets/rate-card-on-project.png)

## 從專案移除費率卡

當您從專案移除費率卡時，會移除其所有工作角色費率。 您無法從專案中移除來自費率卡的個別費率。

您可以移除直接新增至專案的使用者或工作角色的計費費率覆寫，而不移除整個費率卡。

1. 前往專案。
1. 按一下左側面板中的&#x200B;**費率**，然後選取&#x200B;**帳單**。
1. 按一下&#x200B;**移除**&#x200B;圖示![移除圖示](assets/remove-icon.png)。
1. 按一下確認訊息上的&#x200B;**確認**&#x200B;以移除費率卡。

