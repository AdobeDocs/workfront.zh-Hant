---
product-area: resource-management
navigation-topic: resource-planning
title: 在資源計畫器中調整預算日期
description: 如果在資源計畫員中預算資源後發現資源存在超額分配，則可以通過將預算小時數、FTE或成本移至另一個時間範圍來探索假設情況。 然後，您可以根據這些方案中的結果調整預算的小時數、FTE或成本。
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# 在資源計畫器中調整預算日期

如果在資源計畫員中預算資源後發現資源存在超額分配，則可以通過將預算小時數、FTE或成本移至另一個時間範圍來探索假設情況。 然後，您可以根據這些方案中的結果調整預算的小時數、FTE或成本。

當資源的預算小時數、FTE或成本高於其可用小時數、FTE或成本時，可能會出現超額分配。 這會產生負淨值。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對資源管理的訪問，包括對資源計畫員中「編輯優先順序」和「預算小時數」的訪問</p> <p>編輯對財務資料、項目和用戶的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理您要預算資訊的項目的權限，並能夠管理財務</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 調整預算日期

1. 轉至資源計畫器，然後選擇 **依專案檢視**.

   >[!NOTE]
   >
   >只有在按項目查看資源計畫員時，您才可以使用「調整預算日期」選項。

1. 將滑鼠指標暫留在專案名稱上，然後按一下 **更多** 功能表。
1. 按一下 **調整預算日期**.\
   隨即顯示專案分配時間軸。\
   如果存在預算衝突，當前預算小時的時間範圍將以橙色突出顯示；如果沒有衝突，則以藍色突出顯示。

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 將突出顯示的時間範圍拖放到另一個時間，以了解所選項目沒有預算衝突的位置。 當您找到淨值為正的時間範圍時，醒目提示的時間範圍會變成藍色。
1. 按一下專案分配時間軸右上角的「x」，將其關閉。
1. 從項目的現有時間表中刪除預算小時數，並將它們添加到顯示最可用時間表的時間表中。
1. 按一下&#x200B;**儲存**。
1. （有條件和可選）如果沒有預算衝突的時間範圍不在項目時間軸之外，請按一下項目名稱以訪問項目。
1. （條件式和選用式）按一下 **編輯專案**，然後編輯 **計劃開始日期** 或 **計畫完成日期** 修改項目的時間表，不發生預算衝突。\
   如需編輯專案的詳細資訊，請參閱文章 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).

1. （條件式和選用式）按一下 **儲存變更**.
1. 返回到資源計畫器，然後重新輸入時間範圍內的預算小時數、FTE或成本，而不會發生預算衝突。
1. 按一下&#x200B;**儲存**。
