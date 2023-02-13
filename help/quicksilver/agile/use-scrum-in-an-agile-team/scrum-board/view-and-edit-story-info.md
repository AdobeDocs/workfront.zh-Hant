---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum展示板上查看和編輯動態資訊
description: 在看板板上查看動態圖磚時，某些資訊可用於直接從動態圖磚內嵌編輯。
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# 查看和編輯 [!UICONTROL Scrum] 展示板

## 了解可檢視和編輯的資訊

在文章展示板上檢視文章圖磚時，可使用下表中的資訊。 您可以直接從動態圖磚內嵌編輯大部分資訊。

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
   <td> <p>具有直接連結至專案的專案名稱<br>在小版本上使用敏捷檢視時，此連結只會顯示在動態（父任務，而非子任務）上；對專案使用敏捷檢視時，不會顯示此檢視。</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>動態完成的點數或小時數，以及指派給動態的點數或小時數<br>這些數字用於計算並顯示每個動態的[!UICONTROL百分比完成]。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>每個動態和問題的[!UICONTROL百分比完成]。<br>小版本的[!UICONTROL百分比完成]是根據每個文章的[!UICONTROL百分比完成]計算的。</p> <p>更新文章或期刊的[!UICONTROL百分比完成]時，您可以選擇0到100之間的任何數字。</p> </td> 
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
   <td> <p>修改敏捷視圖而可能已新增至敏捷視圖的任何其他欄位（包括自訂欄位），如 <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!UICONTROL Adobe Workfront]中的檢視概觀</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>編輯對任務或問題的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在動態圖磚上檢視及編輯資訊

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 在左側面板中，選取 **[!UICONTROL 迭代]** 要選擇特定的小版本，或選擇 **[!UICONTROL 當前迭代]**.

1. 前往 [!UICONTROL Scrum] 敏捷的故事板。
1. 展開 [!UICONTROL 故事] 拼貼以查看與文章關聯的所有欄位。

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. （可選）若要編輯欄位，請按一下欄位，然後進行任何變更。

   您必須 [!UICONTROL 編輯] 對任務或期刊的權限，可編輯動態圖磚。

>[!NOTE]
>
>若要變更 [!UICONTROL 完成百分比]，您必須輸入介於0和100之間的數字。 欄位不是可移動的滑桿。
