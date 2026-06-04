---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum板上檢視和編輯內文資訊
description: 在Kanban板上檢視內文拼貼時，可以直接從內文拼貼編輯某些資訊。
author: Courtney
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Hu0M7Y-w2u9NIISFgpf7Vg6tlz5AwsrFRtEEPhd4eMc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 445
ht-degree: 3%

---

# 在[!UICONTROL Scrum]板上檢視及編輯內文資訊

## 瞭解哪些資訊可以檢視和編輯

在內文板上檢視內文拼貼時，可使用下表中的資訊。 您可以直接從內文拼貼內嵌編輯大部分資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>資訊</strong> </th> 
   <th><strong>可見</strong> </th> 
   <th><strong>可編輯的內嵌</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>內文名稱，內有直接指向任務或問題的連結</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>含有直接連結至專案的專案名稱<br>在反複專案上使用敏捷檢視時，此連結只會顯示在內文上（父系任務，而非子任務）；在專案上使用敏捷檢視時則不會顯示。</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>內文的完成點數或小時數，以及指派給內文的點數或小時數<br>這些數字用於計算並顯示每個內文的[！UICONTROL完成百分比]。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>每個內文和問題的[！UICONTROL完成百分比]。<br>反複專案的[！UICONTROL完成百分比]是根據每個內文的[！UICONTROL完成百分比]計算的。</p> <p>更新內文或問題的[！UICONTROL完成百分比]時，您可以選擇0到100之間的任何數字。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>將劇本指派給誰</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>圖磚的顏色或類別</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>任何可能透過修改敏捷檢視而新增至敏捷檢視的其他欄位（包括自訂欄位），如[！UICONTROL Adobe Workfront]</a>中<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">檢視總覽的「建立和自訂[！UICONTROL Agile]檢視」中所述。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p> 
   或
   <p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>[！UICONTROL Contribute]或[！UICONTROL Manage]任務或問題的存取權</td> 
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視和編輯內文拼貼上的資訊

{{step1-to-team}}

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

1. 在左側面板中，選取&#x200B;**[!UICONTROL 反複專案]**&#x200B;以選擇特定反複專案，或選取&#x200B;**[!UICONTROL 目前反複專案]**。

1. 移至[!UICONTROL Scrum]敏捷故事板。
1. 展開[!UICONTROL 劇本]拼貼以檢視與劇本相關的所有欄位。

   ![劇本卡](assets/agile-storycard-scrum-2021-350x333.png)

1. （可選）若要編輯欄位，請按一下該欄位，然後進行任何變更。

   您必須擁有任務或問題的[!UICONTROL 編輯]許可權，才能編輯劇本拼貼。

>[!NOTE]
>
>若要變更[!UICONTROL 完成百分比]，您必須輸入介於0到100之間的數字。 此欄位不是您可以移動的滑桿。
