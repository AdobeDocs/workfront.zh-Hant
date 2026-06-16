---
product-area: programs
navigation-topic: create and manage programs
title: 將現有方案新增至Portfolio
description: 您可以將現有方案新增至投資組合。 由於計畫不能存在於兩個不同的投資組合中，因此新增現有計畫會將其從一個投資組合永久移動到另一個投資組合。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LkyWuPHqv0muTinWZT1PMKPGUNErWulIIxHmXVtPIVg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 4%

---

# 將現有方案新增至投資組合

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

您可以將現有方案新增至投資組合。 由於計畫不能存在於兩個不同的投資組合中，因此新增現有計畫會將其從一個投資組合永久移動到另一個投資組合。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>[！UICONTROL標準]</p><p>[！UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[！UICONTROL Edit]對[！UICONTROL Portfolios]和[！UICONTROL Programs]的存取權 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合和計畫的[！UICONTROL管理]許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 將現有方案新增至投資組合

>[!NOTE]
>
>當您的組織同時使用舊版Workfront和Adobe雲端儲存空間來儲存檔案時，您無法將Adobe雲端儲存空間計畫新增至舊版儲存空間產品組合，也無法將雲端儲存空間計畫新增至Adobe雲端儲存空間產品組合。
>您的Workfront執行個體可能沒有這兩種型別的檔案儲存空間。
>如需詳細資訊，請參閱[專案和相關物件的檔案管理概觀](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)。
>

若要將現有方案新增至另一個投資組合：

1. 前往投資組合，然後按一下左側面板中的&#x200B;**[!UICONTROL 程式]**。
1. 按一下&#x200B;**[!UICONTROL 新增程式]**。
1. 按一下&#x200B;**[!UICONTROL 現有程式]**。

   **新增程式**&#x200B;方塊開啟。<!--check screen shot - I logged changes for this casing-->

   ![新增程式方塊](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >新增現有方案會將與該方案相關聯的所有專案帶入投資組合。 請留意勿以這種方式無意中移動專案。

1. 在&#x200B;**[!UICONTROL 將程式新增至此投資組合]**&#x200B;欄位中，輸入程式的名稱，然後當它顯示在清單中時選取它。<!--see the name of this field, I suggested changes here-->

   您可以新增多個計畫。

1. （選擇性）如果您決定不將方案新增至投資組合，請按一下方案名稱旁的&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete-icon.png)。

1. 按一下&#x200B;**[!UICONTROL 新增程式]**。

   程式會顯示在您選取的投資組合上的&#x200B;**[!UICONTROL 程式]**&#x200B;索引標籤中。

