---
product-area: resource-management;projects
navigation-topic: resource-planning
title: 排定資源規劃工具中專案的優先順序
description: 專案會依優先順序列在資源規劃工具中，最重要的專案會列在頂端。
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 1%

---

# 排定資源規劃工具中專案的優先順序

專案會依優先順序列在資源規劃工具中，最重要的專案會列在頂端。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯對資源管理的存取權，包括存取資源規劃工具中的編輯優先順序和預算時數</p> <p>編輯財務資料、專案和使用者的存取權</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>管理您要為其編列預算資訊之專案的許可權，並具備管理財務的能力</p></td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 資源規劃工具中專案的預設順序

預設情況下，專案會考慮以下條件，列在資源規劃工具的專案檢視中。

>[!IMPORTANT]
>
>專案只會根據您第一次開啟資源規劃工具時的以下三個條件列出。 但是，此預設優先順序會自動成為您的自訂優先順序，並且在您執行以下操作之一時無法恢復為原始優先順序：
>
>* 隨時按一下「儲存」時。
>* 當您手動變更專案計畫優先順序時。 如需有關手動變更專案計畫優先順序的資訊，請參閱本文中的[手動變更專案計畫優先順序](#manually-change-the-project-planning-priority)一節。
>
>專案優先順序成為您的自訂優先順序後，專案資訊中的任何變更將不再影響使用這些條件的專案順序。 之後，您只能手動排定專案的優先順序。

在「專案檢視」中列出專案的原始預設條件如下，順序如下：

1. 依專案上的對齊分數。\
   如需專案對齊分數的詳細資訊，請參閱[將計分卡套用至專案並產生對齊分數](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) 。

1. 依專案的計劃開始日期（如果「校準」欄位為Null或數個專案相同）。
1. 依字母順序（如果「校準」欄位為Null或相同，且數個專案的「計劃開始日期」相同）。

在資源規劃工具中使用專案優先順序時，請考慮下列事項：

* 您只能在套用專案檢視時手動自訂專案優先順序。 這也會變更資源規劃工具中的專案順序。
* 當您套用資源規劃工具中的角色或使用者檢視，專案會以在「專案檢視」中建立的相同優先順序顯示。
* 資源規劃工具中的專案順序是您獨有的。 其他使用者可以在資源規劃工具中檢視相同的專案，但使用不同的順序。 您無法報告「專案計畫優先順序」欄位。 這僅在資源規劃工具中可見，並且可作為排定專案優先順序的標幟。

與投資組合相關的專案可能具有投資組合層級的優先順序。 除了資源規劃工具優先順序之外，您還可以啟用在資源規劃工具中檢視專案的投資組合優先順序。 您也可以根據專案的投資組合優先順序來排序專案。

## 手動變更專案計畫優先順序 {#manually-change-the-project-planning-priority}

您必須擁有資源管理的編輯存取權和管理專案的許可權，才能在資源規劃工具中重新排序專案。

藉由指定專案新的優先順序，您可以依重要性順序排列專案。

若要編輯專案計畫優先順序，請執行下列動作：

1. 移至&#x200B;**資源規劃工具**。

1. 按一下專案名稱左側的欄位（包含數字），然後輸入數字以變更Planning優先順序，然後按Enter鍵。\
   ![變更規劃優先順序](assets/mceclip4.png)\
   或\
   暫留在專案名稱上，並按一下專案名稱左側的指示器，然後將其拖放到正確的位置，以變更優先順序。

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   當您選取數字來排定專案的優先順序時，請為較高（較重要）的優先順序選取較低的數字，為較低（較不重要）的優先順序選取較高的數字。 當您將專案的優先順序數字變更為較低的數字（更高的優先順序）時，資源規劃工具中的所有其他專案會在清單中向下移動（變得不那麼重要）。\
   當您將專案的優先順序數字變更為較高的數字（較低優先順序）時，資源規劃工具中的所有其他專案會在清單中上移（變得更加重要）。

1. 按一下「**儲存**」。\
   專案順序會根據您的選擇而改變，這會成為您在資源規劃工具中的自訂專案優先順序。 其他使用者無法在資源規劃工具中檢視專案的優先順序順序，雖然他們或許可以在他們的資源規劃工具中檢視相同的專案。

## 根據專案在資源規劃工具中的Portfolio優先順序來排序專案

>[!IMPORTANT]
>
>貴公司必須有業務或以上的Workfront計畫，才能在Portfolio Optimizer中排定專案的優先順序。
>
>如需Workfront計畫的詳細資訊，請參閱[我們的計畫](https://business.adobe.com/tw/products/workfront/pricing.html)。
>
>如需有關在Portfolio Optimizer中排定專案優先順序的資訊，請參閱[在Portfolio Optimizer中排定專案優先順序](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)。

1. 在&#x200B;**專案檢視**&#x200B;中開啟&#x200B;**資源規劃工具**。
1. 按一下&#x200B;**設定**&#x200B;圖示。
1. 啟用&#x200B;**顯示Portfolio優先順序**&#x200B;設定，以根據其指派的Portfolio顯示專案優先順序。 根據其投資組合的專案優先順序顯示在資源規劃工具優先順序旁邊。 此設定預設為停用。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![Portfolio優先順序](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   專案的專案組合優先順序僅在資源規劃工具的專案檢視中顯示。

1. 按一下&#x200B;**訂單**，根據投資組合優先順序來訂購專案。

   如果您的專案屬於多個專案組合，則可以在資源規劃工具中看到多個專案具有相同的專案組合優先順序。 在此情況下，具有相同專案組合優先順序的專案將依下列條件列出，順序如下：

   1. 一致性分數
   1. 規劃開始日期
   1. 專案名稱

   ![已排序的Portfolio優先順序](assets/rp-portfolio-priority-ordered-350x198.png)

1. 按一下「**儲存**」。

## 變更專案計畫優先順序對使用者可用時數的影響

專案計畫優先順序會影響使用者的可用時數。 與具有最高優先順序的專案相關聯的使用者，會根據其排程，針對此專案的「可用時數」(AVL)欄顯示其最充分的可用性。

依優先順序與第二個專案相關聯的相同使用者將顯示可用時數值，這是其完整可用時數與已針對預算時數欄中的第一個專案編列預算之值之間的差額，以此類推。 如需資源規劃工具中預算資源的相關資訊，請參閱資源規劃工具中使用專案與角色檢視的[預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

如果第一個專案尚未針對使用者編列時數預算（依優先順序排列），但第二個專案已針對相同使用者編列時數預算，則使用者將顯示兩個專案的完整可用時數金額。

我們建議按資源規劃工具中專案的順序更新使用者的預算時數欄，以確保您隨時都可以準確檢視使用者的可用時數。

>[!NOTE]
>
>由於「專案計畫優先順序」對每個資源管理員都是獨一無二的，因此您的第二個優先順序專案可能會是另一個使用者在其資源規劃工具中檢視相同專案的第一個優先順序專案。 如果其他資源經理為其第一個專案編列了資源預算，則您的第一個專案的「可用時數」會根據該變更而減少。
>
>預算時數的使用者會先配置該資源，並減少整個系統中該資源的「可用時數」。 為資源規劃工具中的資源儲存預算時數後，應立即更新所有使用者的可用時數金額。
>
>如需有關可用時數的詳細資訊，請參閱[資源使用狀態和配置](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources)。
