---
product-area: resource-management;projects
navigation-topic: resource-planning
title: 在資源計畫器中排列項目優先順序
description: 在Oracle Resource Planner中，按優先順序列出項目，而最重要的項目在頂部。
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# 在資源計畫器中排列項目優先順序

在Oracle Resource Planner中，按優先順序列出項目，而最重要的項目在頂部。

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

## 資源計畫員中項目的預設順序

預設情況下，考慮以下標準後，這些項目將列在資源計畫員的「項目視圖」中。

>[!IMPORTANT]
>
>只有在您首次開啟資源計畫程式時，才會根據以下三個標準列出項目。 不過，此預設優先順序會自動變成您的自訂優先順序，且每當您執行下列其中一項作業時，就無法還原為原始優先順序：
>
>* 您隨時按一下「儲存」時。
>* 手動更改項目計畫優先順序時。 有關手動更改項目計畫優先順序的資訊，請參閱節 [人工更改項目計畫優先順序](#manually-change-the-project-planning-priority) 這篇文章。
>
>在專案優先順序成為您的自訂優先順序後，專案資訊中的任何變更不再影響使用這些條件進行專案的順序。 之後，您只能手動排定專案的優先順序。

在「項目視圖」中列出項目的原始預設標準如下所示：

1. 按項目上的對齊分數。\
   如需專案對齊分數的詳細資訊，請參閱 [將計分卡套用至專案並產生對齊分數](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. 按項目的「計畫起始日期」（如果「對齊」欄位為Null或對於多個項目相同）。
1. 按字母順序（如果「對齊」欄位為Null或相同，並且多個項目的「計劃開始日期」相同）。

在資源計畫器中處理項目優先順序時，請考慮以下事項：

* 只有在套用「專案檢視」時，您才能手動自訂專案優先順序。 這也會更改資源計畫員中項目的順序。
* 在「資源計畫器」中應用「職責」或「用戶視圖」時，項目將按照在「項目視圖」中建立的優先順序的順序顯示。
* 資源計畫員中項目的順序對您來說是唯一的。 其他用戶可以在資源計畫器中查看相同的項目，但按不同順序查看。 無法報告「項目計畫優先順序」欄位。 這將顯示在「資源規劃器」中，並作為項目優先順序的標誌。

與產品組合相關聯的專案可能具有產品組合層級的優先順序。 除了資源計畫員優先順序外，您還可以在資源計畫員中啟用查看項目的產品組合優先順序。 您也可以根據專案的產品組合優先順序來排序專案。

## 人工更改項目計畫優先順序 {#manually-change-the-project-planning-priority}

要在資源計畫器中重新排序項目，您必須具有「編輯」資源管理訪問權限和「管理」項目權限。

將專案賦予新的優先順序，您就可依其重要性排序。

要編輯項目計畫優先順序，請執行以下操作：

1. 前往 **資源計畫員**.

1. 按一下項目名稱左側欄位內包含數字，然後輸入數字以更改計畫優先順序，然後按Enter。\
   ![](assets/mceclip4.png)\
   或\
   將滑鼠指標暫留在專案名稱上，按一下專案名稱左側的指標，然後將其拖曳至正確的位置，以變更優先順序。

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   當選擇要優先處理項目的數字時，請選擇較低的數字，以表示較高（更重要）的優先順序，選擇較高的數字，以表示較低（較不重要）的優先順序。 將項目的優先順序編號更改為較低編號（優先順序較高）時，資源計畫器中的所有其他項目都會在清單上向下移動（變得不重要）。\
   當將項目的優先順序編號更改為較高的編號（較低的優先順序）時，資源計畫器中的所有其他項目將在清單上向上移動（變得更重要）。

1. 按一下&#x200B;**儲存**。\
   項目順序會根據您的選擇而更改，這將成為資源計畫器中的自定義項目優先順序。 其他用戶在資源計畫員中看不到項目的優先順序順序，儘管他們可能可以在資源計畫員中查看相同的項目。

## 在資源計畫器中根據項目的Portfolio優先順序對項目進行排序

>[!IMPORTANT]
>
>貴公司必須有業務或更高版本的Workfront計畫，才能在Portfolio優化程式中排定專案優先順序。
>
>如需Workfront計畫的詳細資訊，請參閱 [我們的計畫](https://www.workfront.com/plans).
>
>如需在Analytics Optimizer中排定專案優先順序的相關資訊，請參閱 [在Portfolio優化程式中排定專案優先順序](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. 開啟 **資源計畫員** 在 **專案檢視**.
1. 按一下 **設定** 表徵圖。
1. 啟用 **顯示Portfolio優先順序** 設定，以根據項目被分配的Portfolio顯示項目優先順序。 根據項目組合的優先順序顯示在「資源規劃器」優先順序旁。 預設會停用此設定。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   項目的產品組合優先順序僅顯示在資源計畫員的「項目」視圖中。

1. 按一下 **順序** 根據項目組合的優先順序排序項目。

   如果您的項目屬於多個產品組合，則可以在資源規劃器中看到具有相同產品組合優先順序的多個項目。 在這種情況下，具有相同產品組合優先順序的專案會依下列條件依序列出：

   1. 一致性分數
   1. 計畫開始日期
   1. 專案名稱

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. 按一下&#x200B;**儲存**。

## 更改項目計畫優先順序對用戶可用小時數的影響

項目計畫優先順序會影響用戶的可用小時數。 與具有最高優先順序的專案相關聯的使用者會根據其排程，顯示此專案的「可用時數(AVL)」欄的最完整可用性。

按優先順序與第二個項目關聯的同一用戶將顯示「可用時數」值，該值是其「可用時數」的完整數量與「已預算小時數」列中第一個項目已預算的數量之間的差值，以此類推。 有關資源計畫員中預算資源的資訊，請參閱 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

如果沒有為用戶的第一個項目預算小時數（按優先順序），但為同一用戶的第二個項目預算小時數，則用戶將顯示兩個項目的全部可用小時數。

我們建議按資源規劃器中項目的順序為用戶更新「預算小時數」列，以確保您隨時都能夠準確查看用戶的可用小時數。

>[!NOTE]
>
>因為項目計畫優先順序對每個資源管理器都是唯一的，所以您的第二優先順序項目可能是另一個用戶在資源規劃器中查看相同項目時的第一優先順序項目。 如果另一個資源管理器為其第一個項目預算資源，則根據該更改，該資源的可用時數將減少。
>
>預算小時數的用戶首先分配該資源，並減少整個系統內該資源的可用小時數。 在Oracle Resource Planner中為資源保存預算小時數後，應更新所有用戶的可用小時數。
>
>如需「可用時數」的詳細資訊，請參閱 [資源的可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
