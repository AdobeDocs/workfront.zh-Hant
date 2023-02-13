---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 編輯動態資訊
description: 在看板板上查看動態圖磚時，某些資訊可用於直接從動態圖磚內嵌編輯。
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 編輯動態資訊

## 了解可檢視和編輯的資訊 {#understand-what-information-can-be-viewed-and-edited}

在上查看動態圖磚時 [!UICONTROL 看板] 展示板，下表中的資訊可供參考。 您可以直接從動態圖磚內嵌編輯大部分資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>信息</strong> </th> 
   <th><strong>可見</strong> </th> 
   <th><strong>可編輯的內嵌</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>具有直接指向任務或問題的連結的動態名稱</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>具有直接連結至專案的專案名稱</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>動態完成的點數或小時數，以及指派給動態的點數或小時數<br>這些數字用於計算並顯示每個動態的「完成百分比」。</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>每個動態和問題的[!UICONTROL百分比完成]。<br>[!UICONTROL小版本的「完成百分比」是根據每個文章的「完成百分比」來計算的。<br></p> <p>更新文章或期刊的[!UICONTROL百分比完成]時，您可以選擇0到100之間的任何數字。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>將故事分配給誰</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>磁貼的顏色或類別</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>如「建立和自訂敏捷視圖」中所述，修改敏捷視圖可能已新增至敏捷視圖的任何其他欄位（包括自訂欄位） <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">檢視概觀，於 [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在動態圖磚上檢視及編輯資訊

1. 按一下 *[!UICONTROL *主菜單]**表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉菜單中選擇新看板組，或在搜索欄中搜索組。

1. 前往 [!UICONTROL 看板] 展示板。
1. 展開動態圖磚，以檢視與動態相關聯的所有欄位。

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. （可選）若要編輯欄位，請按一下欄位，然後進行任何變更。\
   您必須 [!UICONTROL 編輯] 對任務或期刊的權限，以編輯動態圖磚。\
   如需每個欄位的詳細資訊，以及是否可以編輯，請參閱 [了解可檢視和編輯的資訊](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>若要變更 [!UICONTROL 完成百分比]，您必須輸入介於0和100之間的數字。 欄位不是可移動的滑桿。
