---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 建立進階任務指派
description: 您可以使用「進階指派」來管理任務或問題指派。
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 793b1b0db3fcf66782cd25566df5803df955cb0d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# 建立進階任務指派

{{highlighted-preview}}

您可以使用「進階指派」來管理任務或問題指派。

進行進階指派時，您可以調整下列指派資訊：

* 將使用者指派給任務或問題（這可以在進階指派之外完成）。
* 調整並重新分配每個受指派人分配的時數。
* 決定應將哪些使用者指定為任務或問題的擁有者或主要受指派人。
* 指定每個使用者在處理任務或問題時履行哪個角色。
* <span class="preview">覆寫工作角色的計費率。</span>

>[!NOTE]
>
>指派使用者工作時，其根據排程的可用性會影響任務和問題的計畫和預計日期。 如需排程的相關資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## 您可以進行進階指派的Adobe Workfront區域

本文說明如何在任務或問題的標題中存取進階指派。

此外，您可以在Workfront的下列區域進行進階任務指派：

* 在清單與報表中，當「工作總攬」欄位顯示在檢視中時。
* 編輯任務時顯示在「工作總攬」區段中。 如需詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在任務或問題標題中，在指派區域中。
* 在工作負載平衡器中。 如需詳細資訊，請參閱 [使用工作負載平衡器手動指派工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務和問題的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>對任務或問題貢獻或更高許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 進行進階任務指派

1. 前往您要指派任務或問題的專案。
1. 按一下 **任務** 或 **問題** 然後，在左側面板中，按一下清單中任務或問題的名稱。

   >[!TIP]
   >
   >如果有兩個或更多人員被指派，您可以直接在任務或問題清單上進行進階指派。 按一下 **指定任務** 欄位，然後按一下 **人員圖示** 以開啟「進階指定」視窗。 跳至步驟5以繼續建立進階指派。\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. 按一下 **指派給** 在 **指定任務** 任務或問題標題中的欄位

   或

   如果任務或問題已經指派，請按一下指派的名稱。

1. 按一下 **進階**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 在 **搜尋人員、角色和團隊** 欄位，開始輸入使用者、角色或團隊的名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   >[!NOTE]
   >
   >如果使用者名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

1. （選用）繼續在中新增受指派人 **搜尋人員、角色或團隊** 方塊以新增多個資源至任務或問題。

   >[!TIP]
   >
   >* 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >* 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >
   >
   >* <span class="preview">新增工作角色指派時，您可以搜尋工作角色或地點。 選取「系統/預設職務角色」以使用指定的預設收費率，或選取「費率卡職務角色」以修訂指定層次的費率。 如需費率卡的詳細資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
   >
   >
   >* 如果在停用使用者、工作角色或團隊之前已將其指派，則他們仍會被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >   
   >   * 將工作專案重新指派給使用中資源。
   >   * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。
   >   
   >

1. 對於中的每位使用者 **被指定者** 欄中，指定下列資訊：


   * **所有者**：將游標停留在受指派人名稱上，然後按一下 **設為主要播放器** 「擁有者」欄位中，將受指派人標示為任務或問題擁有者。 綠色核取方塊表示指定的使用者是任務或問題的主要聯絡人。 Adobe Workfront會將您指派給任務或問題的第一個使用者或工作角色標示為擁有者或主要指派。 團隊不能被指定為任務或問題的主要擁有者。

     >[!IMPORTANT]
     >
     >根據您的Workfront管理員或群組管理員設定專案偏好設定的方式，當您有多個使用者指派至任務時，Workfront可能會使用任務負責人的排程來計算任務的時間表。 如需關於多個任務受指派人的資訊，請參閱文章中的「將多個使用者指派到一個任務」一節 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **配置** ：當任務的期間型別為簡單時，指定應指派給任務的每個使用者或工作角色的小時數。 每位使用者所有指派時數的總和等於 **計畫時數** 欄底部的欄位。 在所有其他情況下，請指定您希望受指派人解決任務或問題的時間百分比（或配置）。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * 在您手動修改任務的指派分配後，任務的計畫時數可能會相應地更新。 如需詳細資訊，請參閱文章中的「管理使用者指派時更新任務規劃時數」一節 [計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * 您無法手動修改問題的指派分配。
     >   * 您無法手動修改指派給任務的團隊配置。
     >   
     >

   * **受指派人的角色：** 選取使用者完成此指派時應使用的角色。  預設會顯示使用者的主要角色。 按一下「受指派人的角色」方塊以選取其他角色。  當您先將任務或問題指派給角色，然後新增可以履行該角色的使用者作為第二個指派時，會篩選建議使用者清單，以供可以履行已指派給任務和問題的角色的使用者使用。

     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   <div class="preview">

   * **位置**：如果附加至專案的費率卡使用具有職務角色的位置，則該位置會來自費率卡。 無法變更位置。

   * **收費率**：使用者的收費率來自使用者或其相關職務角色的系統費率。 職務角色的計費費率來自系統費率或費率卡（如果費率卡已附加至專案）。 此欄位中未顯示現有的收費率。 按一下欄位以變更此特定任務指派的計費率。

   </div>

   * **期間型別**：這僅適用於任務。 按一下「持續時間型別」的名稱，然後從下拉式選單中選取「持續時間型別」。 如需持續時間型別的相關資訊，請參閱 [任務工期與工期型別概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **持續時間：** 當您有任務的「管理」許可權時，您可以更新任務的此欄位。

     如需詳細資訊，請參閱 [任務工期與工期型別概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 大量編輯工作分派資訊時，會出現類似的對話方塊，以指派使用者、時數、配置和任務擁有者。

   * **計畫時數**：當期間型別為計算指派或簡單時，更新計畫時數。 因此，每個資源的配置百分比或時數會平均分配。 當期間型別為已計算的工作或投入比導向時，Workfront會計算計畫時數。 如需詳細資訊，請參閱 [任務工期與工期型別概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

     生產環境中的影像範例：

     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     「預覽」環境中的範例影像：

     ![進階任務指派](assets/advanced-assignments-location-billing-rates.png)

     </div>

1. 按一下&#x200B;**儲存**。
