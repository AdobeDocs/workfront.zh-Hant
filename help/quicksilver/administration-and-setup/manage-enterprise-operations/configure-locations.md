---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 設定位置
description: 您可以設定預設位置，以指派為費率卡中工作角色的屬性。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 5%

---

# 設定位置

您可以設定預設位置，以指派為費率卡中工作角色的屬性。 這可確保費率卡準確反映每個位置的市場費率。

費率卡可讓您的組織輕鬆管理專案的收費率。 如需詳細資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL標準]</td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 新增位置

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **位置**]。
1. 按一下清單底部的&#x200B;[!UICONTROL **新增更多位置**]。
1. 輸入地點名稱和說明。
1. 按一下輸入區域外部以儲存位置。
1. 若要刪除位置，請在清單中選取該位置，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除](assets/delete.png)。

>[!NOTE]
>
>無法刪除與費率卡上工作角色相關聯的位置。

## 新增子位置

您可以將子位置新增至現有位置。 舉例來說，如果您已有英國的地點，則倫敦可以是子地點。

允許子位置的三個層級。 國家/地區、州/省和城市是次地點的常見用法。

您可以使用與最上層地點相同的方法，將每個子地點新增為費率卡上的屬性，以定義該地點特定職務角色的費率。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **位置**]。
1. 在清單中選取現有的位置，然後按一下[新增子位置] ****。
1. 輸入地點名稱和說明。
1. 按一下輸入區域外部以儲存位置。

   子位置會縮排在頂層位置下。

   ![位置和子位置](assets/locations-sublocations.png)


