---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中管理用戶分配
description: 作為資源管理器，您可以為用戶分配工作，並從工作負載平衡器管理其每日、每週或每月分配。
author: Alina
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '2757'
ht-degree: 0%

---

# 在工作負載平衡器中管理用戶分配

作為資源管理器，您可以為用戶分配工作，並從工作負載平衡器管理其每日、每週或每月分配，以確保分配的小時數符合其可用計畫。

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
   <td> <p>在使用團隊或「資源配置」區域中的工作負載平衡器時進行計畫 </p>
   <p>使用項目的工作負載平衡器時工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下項目的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>對要管理分配的任務和問題，提供包括「進行分配」的權限或更高。 </p> <p>或 </p> <p>除了更新分配外，還管理要更新計畫小時數的任務的權限。 有關在工作負載平衡器中更新計畫小時數的資訊，請參見 <a href="#update-task-planned-hours-when-managing-user-allocations">在管理用戶分配時更新任務計畫小時數</a> 一節。 </p> <p>有關任務權限的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md">共用任務 </a><span> 如需問題權限的相關資訊，請參閱</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md">共用問題 </a></span>. </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 了解使用者分配

用戶分配是指用戶在某一天或工作日、周或月中完成工作項所應花費的時間的小時數。 它們包含在工作項目的「計畫小時數」中。

本文說明如何為指派給工作或問題的使用者更新每日、每週或每月的每小時分配。 有關管理用戶的總體分配和任務角色的資訊，請參閱 [管理任務上的用戶和角色分配時數](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [使用者配置概觀](#user-allocation-overview)
* [重設用戶分配的條件](#criteria-that-reset-user-allocations)

### 使用者配置概觀 {#user-allocation-overview}

您可以在工作負載平衡器中以小時或百分比值顯示用戶分配。 您可以調整小時數或百分比。

用戶分配被包括在工作項的「計畫小時數」中。 如需「計畫小時數」的相關資訊，請參閱 [計畫小時數概觀](../../manage-work/tasks/task-information/planned-hours.md).

任務「計畫小時數」在分配給任務的用戶的任務持續時間內的所有天之間平均分配。 例如，如果任務的「持續時間」為5天，總計為10個「計畫小時」，則任務的每日分配數為2小時。 每週分配為10小時。 這表示，系統會為使用者分配每天2小時的工作時間。 但是，您可以使用工作負載平衡器手動更改用戶的每日分配。

>[!CAUTION]
>
>工作負載平衡器僅顯示每個工作項最多1000計畫小時和項目持續時間最多1000天。 在達到1000小時或1000天限制後，工作負載平衡器中的分配將顯示為零。 我們建議將任務分為較小的子任務，以適應更多的計畫小時數或超過1000天的持續時間。

在工作負載平衡器中查找任務或問題的每日、每週或每月分配時，請考慮以下事項：

* 您可以檢視使用者對其工作項目的每日、每週和每月分配。 啟用「周」或「月」視圖，以顯示每週或每月分配。
* 您可以使用工作負載平衡器修改用戶對任務或問題的每日、每週或每月分配。 有關調整工作負載平衡器視圖的資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   >[!NOTE]
   >
   >建議您在管理使用者分配時，決定要一律使用的時間範圍（每日、每週或每月），而不要針對相同的工作項目在使用者之間切換。 更新先前更新過每日分配的同一用戶的每週分配，將更改該用戶的每日分配。

* 您可以更新工作日和非工作日的分配。
* 當Workfront自動計算任務的每日分配時，工作項的計畫起始日期和計畫完成日期以及項目的計畫的時間戳非常重要。

>[!INFO]
>
> 例如，某個任務的「持續時間」可能為2天，「計畫時數」為2小時，其「計劃開始時間」為12:00，在持續時間的第一天，該任務的「計劃開始時間」為12:00，用戶和「項目計畫」為5:00。 使用者第一天的容量為5小時。 使用者第二天的容量為8小時（如果排程從上午9點開始）。
>
>Workfront會使用下列公式計算持續期間2天內2小時的分配：
>
>
```
>
>   Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours
>```
>
>  例如，每天的每日分配小時數為：
>   
>  (2 / 13)* 5 =第一天的分配時數0.77
>
>  (2 / 13)* 8 =第二天的分配時數1.23
>
>  在上述計算中，13是任務的可用總時數：5 + 8 = 13



* 兩個使用者位於不同時區，或分配給不同使用者的排程，可能會導致配置金額對兩個檢視相同工作項目的使用者而言不同。

* 當使用者排程了休息時間時，該日或該日的部分會顯示在灰色背景中。 如果Workfront管理員在「設定」區域中啟用「使用者休息時間」設定，以考慮使用者的休息時間，則分配的小時數會移至時間軸中的下一個可用日。 如果禁用該設定，則分配的小時數將保持在標籤為「暫停」的當天，並且用戶將顯示為「過度分配」。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!TIP]
   >
   >如果在將用戶分配給工作項後標籤了時間，則必須重新計算項目的時間軸，以顯示移動的分配。 如需詳細資訊，請參閱 [重新計算項目時間表](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* 如果有多個用戶分配給任務，則計畫小時數量首先平均分配給每個用戶，然後平均分配給任務持續時間內的每天。 此分配將成為每個用戶對任務的分配。

   例如，可能存在下列情況：

   * 對於「持續時間」為2天且為一個用戶分配了10個「計畫時數」的任務，預設情況下，用戶的每日分配為5小時。
   * 對於「持續時間」為2天、「計畫時數」為2個使用者分配了10個「計畫時數」的任務，依預設，每個使用者的每日分配為2.5小時。

* 如果任務或問題在計畫完成日期之前完成，則剩餘天數的分配小時數將經過，不會計入用戶的總體分配。 只有啟用「顯示分配」表徵圖和「顯示預計日期」設定後，才會顯示此資訊。 有關在工作負載平衡器中啟用設定的詳細資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/allocations-struck-through-highlighted-350x39.png)

* 當用戶被過度分配時，其分配的小時數在用戶欄位中顯示為紅色背景。
* 當用戶被分配不足或分配了等量的小時數到其計畫的可用時間時，小時數將以藍色背景顯示。
* 您可以在使用者行的圖表檢視中顯示使用者配置。 有關為用戶分配啟用圖表視圖的資訊，請參閱文章中的「導航工作負載平衡器」部分 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/user-allocation-chart-350x237.png)

### 重設用戶分配的條件 {#criteria-that-reset-user-allocations}

並非所有任務更改都觸發修改的分配以重新分配。 但是，某些操作可能會重置資源上已調整的分配，並將它們平均重新分配到每個受分配者在工作項目期間的所有天。

>[!NOTE]
>
>如果尚未修改工作項上分配的自動分配，則當工作項上分配的數量、任務的持續時間或計畫小時數發生變化時，小時將在所有分配者中平均分配。

* [重置調整分配的操作](#actions-that-reset-adjusted-allocations)
* [未重置調整分配的操作](#actions-that-do-not-reset-adjusted-allocations)

#### 重置調整分配的操作 {#actions-that-reset-adjusted-allocations}

在您手動調整使用者的每日、每週或每月分配後，以下動作會重設或修改這些分配，如 [修改用戶分配](#modify-user-allocations) 本文一節：

* 當您縮短工作項的長度，從而縮短其持續時間內的天數時，從丟失天數調整的分配小時數將添加到工作項的最後一天的分配量中。
* 當您更改分配或工作項上的計畫小時數時，新的計畫小時數將在工作項的整個持續時間內統一重新分配。
* 將受託人添加或刪除至工作項，並且這會導致任務的「計畫小時數」發生更改時，調整後的值將統一重新分配。

#### 未重置調整分配的操作 {#actions-that-do-not-reset-adjusted-allocations}

對工作項的以下更改不會觸發要重置或修改的調整分配：

* 當您移動工作項的天數但「持續時間」中的天數未更改時，調整後的分配值將保持不變並移至新日期。
* 當增加工作項的「持續時間」(Duration)時，增加其「持續時間」(Duration)中的天數，調整後分配的小時數在調整後的天數內保持不變。 已分配0小時的工作項目將添加其他天數。
* 將受託人添加或刪除至工作項，並且這不會導致項的「計畫小時數」更改時，調整後的值將保持不變。

## 在工作負載平衡器中查找計畫小時數

您可以通過查找分配給用戶的任務或問題的「計畫小時數」，使用工作負載平衡器修改用戶對任務或問題的分配。

在工作負載平衡器中查看計畫小時數時，請考慮以下事項：

* 任務或問題的總計畫小時數顯示在工作負載平衡器左側的任務或問題名稱旁邊。

* 項目的總計計畫時數顯示在工作負載平衡器左側的「項目名稱」旁邊。 這表示在工作負載平衡器中項目下列出的所有任務和問題的「計畫時數」合計，而不是項目的所有「計畫時數」合計。
* 只有在手動啟用「顯示分配」設定時，才會顯示所有任務和所有項目的每日或每週分配的時間量。 有關在工作負載平衡器中啟用設定的資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 修改用戶分配 {#modify-user-allocations}

作為為用戶分配工作的一部分，您可以修改工作負載平衡器中的用戶分配，以確保它們不會被過度分配，或者確保資源之間的小時數達到精確平衡。 如需識別使用者是否被過度配置的相關資訊，請參閱區段 [使用者配置概觀](#user-allocation-overview) 這篇文章。

1. 請確定您有指派給使用者的工作和問題。 有關在工作負載平衡器中為用戶分配工作的資訊，請參見 [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. 轉到工作負載平衡器。
1. （選用）按一下 **周** 或 **月** 管理使用者的每週或每月分配。

   ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. 在 **已分配的工作** 區域，找到要手動修改分配的用戶，然後按一下用戶名左側的右箭頭以展開用戶。

   ![](assets/wb-highlight-on-name-caret-350x106.png)

1. 按一下專案名稱左側的右箭頭，以展開專案並顯示指派給使用者的工作項目。

   >[!TIP]
   >
   >您只能修改任務和問題的用戶分配。 無法修改項目的用戶分配。

1. （選用）按一下 **顯示分配表徵圖** ![](assets/show-allocations-icon-small.png) 顯示所有工作項的分配。

   任務和項目的名稱將替換為任務或項目的用戶分配。

1. （選用）按一下 **設定** 圖示 ![](assets/gear-icon-settings.png) ，然後選擇以下任一選項：

   1. **包括問題的時數**. 這允許您管理除任務分配外的問題分配。
   1. **顯示完成的工作** . 這會顯示在您管理分配的時間軸期間已完成和已排程的項目。
   1. **顯示剩餘時間** 選項。 每個使用者（在使用者行中）變更的總小時數。 啟用此設定後，工作負載平衡器將顯示每個用戶可用的工時數，而不是分配給它們的工時數。

      >[!TIP]
      >
      >啟用此設定時修改分配會減少使用者行中的總數。

   1. **專案** 在 **選擇顏色主題** 區段。 這會以不重複的顏色顯示每個專案及其個別的工作項目，讓您更容易了解哪些項目屬於哪個專案。
   1. **百分比** 在 **在** 區段。 這會以百分比值顯示分配。 根據其排程，使用者的容量會視為100%。 例如，如果使用者與每天8小時的排程相關聯，8小時等於100%的容量。 如果您想要將使用者分配為一天4小時，您會將其分配更新為50%。

1. 按一下 **更多** 功能表 ![](assets/qs-more-menu.png) ，然後按一下 **編輯分配**.

![](assets/more-menu-on-task-wb-nwe.png)

或

按兩下任務或問題欄中的日、周或月。

配置方塊會變成可編輯。

1. 在每日、每週或每月分配的框內按一下，以手動更新要為用戶分配的小時數或百分比值，然後按一下 **儲存** 圖示 ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >按一下 **取消** 圖示 ![](assets/cancel-allocations-wb.png) 刪除您調整的分配。

   ![](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   用戶更新的分配。

   >[!TIP]
   >
   >如果任務或問題在計畫完成日期之前完成，則剩餘天數的分配小時數將經過，不會計入用戶的總體分配。 只有啟用「顯示分配」表徵圖和「顯示預計日期」設定後，才會顯示此資訊。

   存在下列情況：

   * 對於具有「持續時間類型」且「不簡單」或「問題」的任務，分配的總計必須與「計畫小時數」任務匹配，然後您才能按一下複選標籤表徵圖。
   * 對於具有「簡單持續時間類型」的任務，分配的總計可以高於或低於「計畫小時數」，即使它們不匹配，您也可以按一下複選標籤表徵圖。 這也會更新任務的計畫小時數。 您必須擁有正確的權限和訪問權限，才能更新工作負載平衡器中任務的「計畫時數」。

      >[!TIP]
      >
      >當您開始調整分配時，任務名稱的右側將顯示一個鎖定表徵圖，以指示該任務具有「簡單持續時間類型」。

      ![](assets/lock-icon-on-simple-task-in-the-balancer-350x119.png)
   有關在工作負載平衡器中更新計畫小時數時需要滿足的條件的詳細資訊，請參閱本文的以下部分： [在管理用戶分配時更新任務計畫小時數](#update-task-planned-hours-when-managing-user-allocations). 有關任務持續時間類型的資訊，請參閱 [任務持續時間和持續時間類型概覽](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （條件性）如果任務被分配給多個用戶，請對分配給任務的每個用戶重複這些步驟，以更新每個用戶的分配。

   任何有權查看工作負載平衡器並查看相同用戶和您管理的相同項目的人，現在都可以查看您管理的用戶的更新分配。

## 在管理用戶分配時更新任務計畫小時數 {#update-task-planned-hours-when-managing-user-allocations}

在任務的工作負載平衡器中管理用戶分配時，可以更新任務的「計畫小時數」。 當已更新的已分配小時數總計與任務的原始計畫小時數總計不匹配時，就會發生這種情況。

>[!IMPORTANT]
>
>* 更新任務的「計畫時數」可能會影響項目進度。
>* 通過更改每日分配人工更新計畫小時數，在將來從任務中刪除分配時可能會影響計畫小時數。 如需詳細資訊，請參閱 [計畫小時數概觀](../../manage-work/tasks/task-information/planned-hours.md).
>
>* 無法通過更新工作負載平衡器中的分配來更新問題的計畫小時數。
>


當存在下列條件時，即可進行此操作：

* 您擁有從工作負載平衡器管理計畫小時的正確權限和訪問權限。 其中包括：

   * 管理任務的權限。
   * 在訪問級別的「資源管理」區域的「工作負載平衡器訪問」中更新計畫小時數。

   有關使用工作負載平衡器所需的訪問權限的詳細資訊，請參閱本文的以下部分： [存取需求](#access-requirements) .

* 任務的「持續時間類型」為「簡單」。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the statement above might include other duration types in the future)</p>
  -->
