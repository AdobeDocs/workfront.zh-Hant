---
navigation-topic: business-case-and-scorecards
title: 將計分卡套用至專案並產生對齊分數
description: 您可以使用計分卡來測量專案與先前建立之產品組合標準的一致程度。 計分卡通常反映組織的使命、價值和戰略目標。
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# 將計分卡套用至專案並產生對齊分數

<span class="preview">本頁強調顯示的資訊指的是尚未普遍提供的功能。 它僅在預覽環境中可用。</span>

您可以使用計分卡來測量專案與先前建立之產品組合標準的一致程度。 計分卡通常反映組織的使命、價值和戰略目標。

如需計分卡以及如何建立計分卡的詳細資訊，請參閱 [建立計分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>業務或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>檢視或更高存取Portfolio</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>檢視或更高產品組合權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 專案計分卡 {#project-scorecards}

* [計分卡概述](#scorecards-overview)
* [專案計分卡](#project-scorecards)

### 計分卡概述 {#scorecards-overview}

通常，項目經理會完成計分卡資訊，為項目生成介於0和100之間的對齊值。 產品組合經理稍後審閱產品組合優化程式中的項目以比較它們時，將使用產生的值。

如需產品組合最佳化的詳細資訊，請參閱文章 [Portfolio優化程式概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### 將計分卡套用至專案

對於具有計畫許可和管理項目權限的用戶，可以在項目中附加記分卡。

如需專案權限的詳細資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

您可以將計分卡新增至專案，作為建立專案業務案例的一部分。

有關構建業務案例的詳細資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您的Adobe Workfront管理員或群組管理員必須先啟用專案「業務案例」區域中的計分卡區段，才能從「業務案例」存取計分卡。 有關設定項目首選項和啟用業務案例區域的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

要將記分卡應用於項目，請執行以下操作：

1. 前往您要套用計分卡的專案。
1. 按一下 **業務案例** 中。
1. 尋找 **計分卡** 部分。\
   您必須在 **計分卡** 區段。

   如需建立計分卡的相關資訊，請參閱 [建立計分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. 從下拉式功能表中選取計分卡。

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. 指定計分卡中所有問題的答案。

   Workfront會對每個已回答的問題套用分數，並根據每個問題的個別分數來計算整體專案分數。

   有關生成項目整體對齊分數的詳細資訊，請參閱 [為項目生成對齊分數](#generate-an-alignment-score-for-a-project).

1. 按一下 **儲存** 儲存計分卡並對專案評分。

   計分卡現在會與專案建立關聯，且專案會獲得分數。

1. （條件性）當計分卡問題的值發生變更時，您必須重新計算計分卡，以反映專案分數的新值。 若要重新設定計分卡，請執行下列動作：

   1. 移至專案清單，然後選取清單中的所有專案。
   1. 按一下 **編輯** 表徵圖。
   1. 按一下 **設定** 在左側面板中，檢查 **重新計算計分卡** 選項。
   1. 按一下儲存。這會根據所有所選專案附加的計分卡，重新計算分數值。

      >[!NOTE]
      >
      >   <span class="preview">大量編輯專案時，「預覽」環境中已移除重新計算計分卡的選項。 </span>


## 生成對齊分數

* [為項目生成對齊分數](#generate-an-alignment-score-for-a-project)
* [為產品組合產生對齊分數](#generate-an-alignment-score-for-a-portfolio)

### 為項目生成對齊分數 {#generate-an-alignment-score-for-a-project}

對齊分數是完成計分卡後產生的值。

計分卡包含的問題包含已指派數值（稱為對齊點）的答案選擇。 這些點可用來決定專案與貴組織的一致程度。 每個問題的對齊點都包含0到100之間的數字。

完成計分卡後，Workfront會使用下列公式，以百分比計算專案的對齊分數：

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

如需詳細資訊，請參閱 [建立計分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### 為產品組合產生對齊分數 {#generate-an-alignment-score-for-a-portfolio}

產品組合的對齊分數是產品組合中所有專案的對齊分數的平均值。

當專案的計分卡完成時，Workfront會使用這些值，透過下列公式，以百分比計算產品組合的對齊分數：

Portfolio對齊分數=專案對齊分數百分比/產品組合中專案數的總和

>[!NOTE]
>
>如果專案沒有與其相關聯的計分卡，因此沒有對齊分數，則會將其視為產品組合中的對齊率為0%。 項目在項目組合中的項目數中予以考慮。

## 查看對齊分數

您可以在項目級別或在Portfolio優化程式中查看項目的對齊分數。

* [查看項目上的對齊分數](#View%20the)
* [在Portfolio優化程式中查看項目和產品組合的對齊分數](#View%20the2)

### 查看項目上的對齊分數

如果您對專案擁有Contribute權限，則可在專案層級檢視專案的對齊分數。

1. 轉到要查看其「對齊分數」的項目。
1. 按一下 **業務案例** 中。
1. 前往 **業務案例摘要** 在螢幕的右側。

   Alignment Score位於Business Case Summary（業務案例摘要）中，位於 **對齊** 值。

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### 在Portfolio優化程式中查看項目和產品組合的對齊分數

如果您有管理對產品組合的訪問權，則可以在Portfolio優化程式中查看項目或產品組合的對齊分數。

如需Portfolio優化程式中顯示資訊的詳細資訊，請參閱 [Portfolio優化程式概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [在Portfolio優化程式中查找項目的對齊分數](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [在Optimizer中找出產品組合的對齊分數](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### 在Portfolio優化程式中查找項目的對齊分數 {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後 **Portfolio**.

1. 按一下Portfolio的名稱。
1. 按一下 **Portfolio最佳化** 中。

   Portfolio優化程式隨即顯示。

1. 專案的對齊分數會以百分比顯示於 **對齊方式** Portfolio優化程式的列。

   這是根據與專案相關聯之計分卡的專案對齊分數。

#### 在Optimizer中找出產品組合的對齊分數  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. 前往 **專案** 欄的URL區域。
1. 選取 **Portfolio** 標籤。
1. 按一下Portfolio的名稱。
1. 選取 **Portfolio最佳化** 標籤。
1. 在Portfolio優化程式頂端， **對齊** 值，以及 **對齊方式** 表示產品組合對齊分數的量規。

   這是作品集的對齊分數。

   如需如何產生產品組合之對齊分數的詳細資訊，請參閱 [為產品組合產生對齊分數](#generate-an-alignment-score-for-a-portfolio).

## Portfolio優化程式分數概觀

項目的對齊分數與產品組合優化程式分數之間存在差異。

專案的對齊分數會根據完成計分卡後取得的點數計算。 然後，系統會使用此分數來判斷產品組合對齊分數。 對齊分數會以百分比顯示。

專案的對齊分數會顯示在 **對齊方式** Portfolio優化程式的列。

產品組合優化程式分數是在Portfolio優化程式中自動計算的排名，可依此排列項目的優先順序。 產品組合最佳化程式分數會以指標圖示的形式顯示，並附上數字，並顯示在 **分數** Portfolio優化程式的列。 只有在「業務案例」的所有部分（目標除外）完成時，才會生成Portfolio優化程式分數。

有關為項目建立業務案例的詳細資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

如需有關計算專案的產品組合最佳化程式分數的詳細資訊，請參閱 [Portfolio優化程式分數概觀](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
