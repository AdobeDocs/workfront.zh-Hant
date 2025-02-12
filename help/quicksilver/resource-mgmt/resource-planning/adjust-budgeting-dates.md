---
product-area: resource-management
navigation-topic: resource-planning
title: 在資源規劃工具中調整預算日期
description: 如果您在資源規劃工具中編列預算之後發現資源過度分攤，您可以將預算時數、約當全職人數或成本移至另一個時間範圍，以探索假設分析案例。 根據這些案例中的發現，您可以調整預算時數、約當全職人數或成本。
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# 在資源規劃工具中調整預算日期

如果您在資源規劃工具中編列預算之後發現資源過度分攤，您可以將預算時數、約當全職人數或成本移至另一個時間範圍，以探索假設分析案例。 根據這些案例中的發現，您可以調整預算時數、約當全職人數或成本。

當資源的預算時數、FTE或成本高於其可用時數、FTE或成本時，可能會顯示超額分攤。 這會產生負淨值。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
    <td><p>新增：任何</p>
       <p>或</p>
       <p>目前：Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對資源管理的存取權，包括存取資源規劃工具中的編輯優先順序和預算時數</p> <p>編輯財務資料、專案和使用者的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理您要為其編列預算資訊之專案的許可權，並具備管理財務的能力</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 調整預算日期

1. 移至[資源規劃工具]並選取[依專案檢視] ****。

   >[!NOTE]
   >
   >只有在您依專案檢視資源規劃工具時，才能使用「調整預算日期」選項。

1. 將滑鼠停留在專案名稱上，然後按一下&#x200B;**更多**&#x200B;功能表。
1. 按一下&#x200B;**調整預算日期**。\
   專案配置時間表隨即顯示。\
   如果存在預算衝突，目前編列預算時數的時間範圍會以橘色醒目顯示，如果沒有衝突，則會以藍色醒目顯示。

   ![調整預算日期](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 將醒目提示的時間範圍拖放至另一個時間，以瞭解所選專案在何處沒有預算衝突。 當您找到「淨值」為正數的時間範圍時，反白的時間範圍會變更為藍色。
1. 按一下專案配置時間表右上角的「x」以將其關閉。
1. 從專案的現有時間表移除預算時數，並將其新增至顯示最可用性的時間表。
1. 按一下「**儲存**」。
1. （條件式與選擇性）如果沒有預算衝突的時間範圍在專案的時間表之外，請按一下專案名稱以存取專案。
1. （條件式及選擇性）按一下&#x200B;**編輯專案**，然後編輯&#x200B;**規劃開始日期**&#x200B;或&#x200B;**規劃完成日期**，以修改時間範圍內的專案時間表，而不會產生預算衝突。\
   如需有關編輯專案的詳細資訊，請參閱文章[編輯專案](../../manage-work/projects/manage-projects/edit-projects.md)。

1. （條件式與選擇性）按一下&#x200B;**儲存變更**。
1. 返回資源規劃工具，並在時間範圍內重新輸入預算時數、約當全職人數或成本，而不發生預算衝突。
1. 按一下「**儲存**」。
