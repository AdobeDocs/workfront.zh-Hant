---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中管理使用者配置
description: 身為資源管理員，您可以指派工作給使用者，並從「工作負載平衡器」管理他們的每日、每週或每月配置。
author: Alina
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: b68436ff0c7edf3129b13e10859d63d73e4553de
workflow-type: tm+mt
source-wordcount: '2808'
ht-degree: 0%

---

# 在工作負載平衡器中管理使用者配置

{{highlighted-preview}}

身為資源管理員，您可以指派工作給使用者，並從工作負載平衡器管理他們的每日、每週或每月配置，以確保他們被配置符合其可用排程的時數量。

## 存取需求 {#access-requirements}

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫，在資源區域使用工作負載平衡器</p>
   <p>工作，使用團隊或專案的工作負載平衡器時</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻許可權或更高，包括指派給您要管理配置的任務和問題。 </p> <p>或 </p> <p>管理您要更新計畫時數以及更新配置的任務的許可權。 如需有關更新工作負載平衡器中規劃時數的資訊，請參閱 <a href="#update-task-planned-hours-when-managing-user-allocations">管理使用者分派時更新任務計畫時數</a> 一節。 </p> <p>如需工作許可權的相關資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md">共用任務 </a><span> 如需問題許可權的相關資訊，請參閱</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md">共用問題 </a></span>. </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 瞭解使用者配置

使用者配置是時數，表示使用者在某一指定日或工作日、周或月完成工作專案應花費的時間。 它們包含在工作專案的計畫時數中。

本文會說明如何更新指派給任務或問題的使用者的每日、每週或每月小時配置。 如需有關管理使用者及工作角色對任務的整體配置的資訊，請參閱 [管理任務的使用者和角色分配時數](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [使用者配置總覽](#user-allocation-overview)
* [重設使用者配置的條件](#criteria-that-reset-user-allocations)

### 使用者配置總覽 {#user-allocation-overview}

您可在工作負載平衡器中將使用者分配顯示為時數或百分比值。 您可以調整小時或百分比。

使用者配置包含在工作專案的計畫時數中。 如需有關計畫時數的資訊，請參閱 [計畫時數概觀](../../manage-work/tasks/task-information/planned-hours.md).

對於指派給任務的使用者，任務計畫時數在任務期間內的所有天數之間平均分配。 例如，如果任務的工期為5天，總共有10個計畫時數，則任務的每日分配數為2小時。 每週配置為10小時。 這表示使用者會被分配每天工作2小時。 不過，您可以使用工作負載平衡器手動變更使用者的每日分配。

>[!CAUTION]
>
>工作負載平衡器僅顯示每個工作專案最多1000個計畫時數，以及專案持續時間最多1000天。 達到1000小時或1000天限制後，工作負載平衡器中的配置顯示為零。 我們建議將任務分成較小的子任務，以因應較多的計畫時數或超過1000天的持續時間。

為工作負載平衡器中的任務或問題找到每日、每週或每月分配時，請考慮以下事項：

* 您可以檢視每日、每週和每月使用者對其工作專案的配置。 啟用「週」或「月」檢視，以顯示每週或每月配置。
* 您可以使用工作負載平衡器來修改每日、每週或每月將使用者配置給任務或問題。 如需有關調整工作負載平衡器檢視的資訊，請參閱 [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  >[!NOTE]
  >
  >我們建議您決定要在管理使用者配置時一律使用哪個時間範圍（每日、每週或每月），而不是針對相同工作專案在它們之間切換。 針對您先前已更新每日配置的相同使用者更新每週配置，會變更使用者的每日配置。

* 您可以更新工作天和非工作天的配置。
* 當Workfront自動計算任務的每日分配時，工作專案的「計劃開始日期」與「計畫完成日期」的時間戳記以及專案的「排程」都非常重要。

>[!INFO]
>
> 例如，任務的工期可能為2天且計畫時間為2小時，其計劃開始時間為工期第一天下午12:00，使用者與專案排程於下午5點結束。 使用者第一天的容量為5小時。 第二天的使用者容量為8小時（如果排程從上午9點開始）。
>
>Workfront會使用下列公式，計算工期2天內2小時的分配：
>
>```
>
>   Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours
>```
>
>  例如，每天的每日配置時數為：
>   
>  (2 / 13) * 5 =第一天的0.77配置小時
>
>  (2 / 13) * 8 =第二天的1.23配置小時
>
>  在上述計算中，13是工作的總可用時數： 5 + 8 = 13



* 位於不同時區的兩個使用者或位於不同時區的排程，與指派使用者的使用者不同，這會造成檢視相同工作專案的兩個使用者看見分配金額的方式不同。

* 當使用者已排程休假時，一天或一天的一部分會以灰色背景顯示。 如果Workfront管理員在設定區域中啟用了使用者休息時間設定，以將使用者的休息時間列入考量，則分配的時數會移至時間軸中的下一個可用日。 如果停用此設定，則配置的時數仍會保留在標示為休假的當天，且使用者會顯示為過度配置。 如需詳細資訊，請參閱 [設定全系統專案偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!TIP]
  >
  >如果在將使用者指派給工作專案後標籤休假，您必須重新計算專案的時間表以顯示移動的分配。 如需詳細資訊，請參閱 [重新計算專案時間表](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* 如果有多個使用者被指派到任務，則計畫時數的數量會先平均分配給每個使用者，然後平均分配給任務期間內的每一天。 此分配會成為每個使用者對任務的配置。

  例如，可能有下列情況：

   * 對於持續時間為2天且指派給一位使用者的10個計畫時數的任務，使用者的每日分配預設為每天5小時。
   * 對於持續期間2天且將10個計畫時數指派給兩名使用者的任務，每個使用者的每日配置預設為每日2.5小時。

* 如果任務或問題在計畫完成日期之前完成，則剩餘天數的分配時數會被刪除，且不計入使用者的整體分配。 只有在同時啟用顯示配置圖示與顯示預計日期設定時，才會顯示此圖示。 如需有關在工作負載平衡器啟用設定的詳細資訊，請參閱 [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![](assets/allocations-struck-through-highlighted-350x39.png)

* 當使用者被過度分配時，他們分配的時數在使用者欄位中以紅色背景顯示。
* 當使用者未充分分配或分配了相等數量的時數到其排程的可用時間，時數會以藍色背景顯示。
* 您可以在使用者折線的圖表檢視中顯示使用者的配置。 如需為使用者配置啟用圖表檢視的相關資訊，請參閱文章中的「瀏覽工作負載平衡器」一節 [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![](assets/user-allocation-chart-350x237.png)

### 重設使用者配置的條件 {#criteria-that-reset-user-allocations}

並非所有任務變更都會觸發修改的分配，以重新分配。 但是，某些動作可能會重設資源上已調整的配置，並將它們平均重新分配至每個受指派人工作專案期間的所有天數。

>[!NOTE]
>
>如果您未修改工作專案上的自動分派分配，則當工作專案的受指派人數目、任務期間或計畫時數金額有所變更時，時數會在所有受指派人之間平均重新分配。

* [重設已調整配置的動作](#actions-that-reset-adjusted-allocations)
* [不會重設已調整配置的動作](#actions-that-do-not-reset-adjusted-allocations)

#### 重設已調整配置的動作 {#actions-that-reset-adjusted-allocations}

在您手動調整使用者之每日、每週或每月配置後，下列動作會重設或修改這些配置，如 [修改使用者配置](#modify-user-allocations) 章節：

* 當您縮短工作專案的長度以縮短其「持續時間」中的天數時，會從遺失的天數加入已調整配置時數，以配置工作專案最後一天的數量。
* 當您變更工作分派或工作專案上的計畫時數時，新的計畫時數會在工作專案的整個期間中統一重新分配。
* 當您將受指派人新增或移除至工作專案，而這會造成任務的計畫時數變更時，調整的值會均勻地重新分配。

#### 不會重設已調整配置的動作 {#actions-that-do-not-reset-adjusted-allocations}

工作專案的下列變更不會觸發已調整配置以重設或修改：

* 當您移動工作專案的天數，但「持續時間」中的天數未變更時，調整的配置值會維持不變，並移至新日期。
* 當您增加工作專案的「工期」以增加其「工期」中的天數時，調整的已分配時數與調整的天數相同。 會將額外的天數新增至具有0個分配時數的工作專案。
* 當您將受指派人新增或移除至工作專案，而且這不會導致專案的計畫時數變更時，調整的值會維持不變。

## 在工作負載平衡器中找到規劃時數

您可以使用工作負載平衡器，透過尋找指派給使用者的任務或問題的規劃時數，修改使用者對任務或問題的指派。

在工作負載平衡器檢視計畫時數時，請考慮以下事項：

* 任務或問題的總計畫時數顯示在工作負載平衡器左側的任務或問題名稱旁。

* 專案的總計畫時數顯示在工作負載平衡器左側的專案名稱旁。 這代表工作負載平衡器專案下列出的所有任務和問題的總計畫時數，而非專案的所有計畫時數。
* 只有當您手動啟用「顯示配置」設定時，才會顯示所有任務與專案的每日或每週配置時間量。 如需有關在工作負載平衡器啟用設定的資訊，請參閱 [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 修改使用者配置 {#modify-user-allocations}

將工作指派給使用者時，您可以修改工作負載平衡器中的使用者指派，以確保不會過度指派，或確保資源之間準確平衡時數。 如需識別使用者是否過度配置的資訊，請參閱區段 [使用者配置總覽](#user-allocation-overview) 本文章內容。

1. 確保您有指派給使用者的任務和問題。 如需有關在工作負載平衡器指派工作給使用者的資訊，請參閱 [在工作負載平衡器中指派工作的總覽](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. 前往工作負載平衡器。
1. （選用）按一下 **周** 或 **月** 管理使用者的每週或每月配置。

   ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. 在 **已指派的工作** 區域，尋找您要手動修改其配置的使用者，然後按一下使用者名稱左側的向右箭頭以展開使用者。

   ![](assets/wb-highlight-on-name-caret-350x106.png)

1. 按一下專案名稱左側的向右箭頭，展開專案並顯示指派給使用者的工作專案。

   >[!TIP]
   >
   >您只能修改任務和問題的使用者配置。 您無法修改專案的使用者配置。

1. （可選）按一下 **顯示配置圖示** ![](assets/show-allocations-icon-small.png) 以顯示所有工作專案的配置。

   任務與專案的名稱會由任務或專案的使用者配置取代。

1. （可選）按一下 **設定** 圖示 ![](assets/gear-icon-settings.png) 並選取下列任一選項：

   1. **包括問題的時數**. 這可讓您在任務指派之外管理問題指派。
   1. **顯示完成的工作** . 這會顯示已在您管理配置的時間表期間完成並排程的專案。
   1. **顯示剩餘時間** 選項。 每個使用者（在使用者行中）的變更總時數。 啟用此設定後，工作負載平衡器顯示每個使用者可供工作的時數，而不是他們被分配的時數。

      >[!TIP]
      >
      >啟用此設定時修改配置會減少使用者明細行中的總數。

   1. **專案** 在 **選取顏色主題** 區段。 這樣會以獨特的顏色顯示每個專案及其各自的工作專案，並可讓您更容易瞭解哪些專案屬於哪個專案。
   1. **百分比** 在 **顯示使用者分配於** 區段。 這會將配置顯示為百分比值。 根據排程，使用者的容量視為100%。 例如，如果使用者與每天8小時的排程相關聯，則8小時等於100%容量。 如果您想要將使用者配置為一天工作4小時，則將其配置更新為50%。

      >[!NOTE]
      >
      >Workfront管理員在「設定」的「資源管理」區域中，決定要在整個系統中使用哪個排程來計算使用者的容量。 如需詳細資訊，請參閱 [設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).


1. 按一下 **更多** 功能表 ![](assets/qs-more-menu.png) ，然後按一下 **編輯配置**.

   ![](assets/more-menu-on-task-wb-nwe.png)

   或

   在任務或問題列中的日、周或月上按兩下。

   配置方塊變為可編輯。

1. 按一下每個每日、每週或每月配置的方塊，以手動更新每日、每週或每月要配置使用者的小時數或百分比值，然後按一下 **儲存** 圖示 ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >按一下 **取消** 圖示 ![](assets/cancel-allocations-wb.png) 以移除您已調整的分配。

   ![](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   使用者配置的更新。

   >[!TIP]
   >
   >如果任務或問題在計畫完成日期之前完成，則剩餘天數的分配時數會被刪除，且不計入使用者的整體分配。 只有在同時啟用顯示配置圖示與顯示預計日期設定時，才會顯示此圖示。

   存在下列情況：

   * 對於工期型別不是「簡單」的任務或對於問題，配置總計必須符合任務計畫時數，然後才能按一下核取記號圖示。
   * 對於具有簡單期間型別的任務，配置總計可以高於或低於計畫時數，並且您可以按一下核取記號圖示，即使它們不相符。 這也會更新任務的計畫時數數量。 您必須擁有正確的許可權和存取權才能從工作負載平衡器更新任務的計畫時數。

     >[!TIP]
     >
     >當您開始調整配置時，任務名稱的右側會顯示一個鎖定圖示，表示任務具有「簡單期間型別」。

     ![](assets/lock-icon-on-simple-task-in-the-balancer-350x119.png)

   如需更新工作負載平衡器中規劃時數所需滿足條件的詳細資訊，請參閱本文中的以下章節： [管理使用者分派時更新任務計畫時數](#update-task-planned-hours-when-managing-user-allocations). 如需有關工作期間型別的資訊，請參閱 [任務期間與期間型別概觀](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （視條件而定）如果任務指派給多個使用者，請對指派給任務的每個使用者重複這些步驟，以更新每個使用者的分配。

   有權檢視工作負載平衡器並檢視相同使用者和您管理的相同專案的任何人，現在都會檢視您管理之使用者的更新分配。

>[!TIP]
>
><span class="preview">工作專案名稱的右側會顯示一個鉛筆圖示，表示已手動調整。</span>

![手動調整時數圖示](assets/icon-for-manually-adjusted-hours.png)

## 管理使用者分派時更新任務計畫時數 {#update-task-planned-hours-when-managing-user-allocations}

當在工作負載平衡器中管理使用者指派時，您可以更新任務的規劃時數。 當更新的分配時數總計與任務的計畫時數的原始總計不符時，就會發生這種情況。

>[!IMPORTANT]
>
>* 更新任務的計畫時數可能會影響專案進度。
>* 當從未來的任務中移除指派時，透過變更每日指派來手動更新計畫時數可能會對計畫時數產生影響。 如需詳細資訊，請參閱 [計畫時數概觀](../../manage-work/tasks/task-information/planned-hours.md).
>
>* 無法透過更新工作負載平衡器中的分配來更新問題的計畫時數。

當存在以下條件時，這是可能的：

* 您擁有從工作負載平衡器管理計畫時數的正確許可權和存取權。 這些功能包括：

   * 管理任務的許可權。
   * 更新計畫時數（在存取層級的「資源管理」區域的工作負載平衡器存取）。

  如需有關使用工作負載平衡器所需存取權的詳細資訊，請參閱本文中的下列章節： [存取需求](#access-requirements).

* 任務的期間型別為「簡單」。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the statement above might include other duration types in the future)</p>
  -->
