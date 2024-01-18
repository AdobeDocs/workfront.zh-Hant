---
product-area: projects
navigation-topic: task-information
title: 更新任務平準延遲
description: 有時候，專案上的任務排程之間可能會發生衝突。 您可以重新排程資源與工作，讓所有工作都能在現實的排程內完成，以平準資源或解決資源衝突。 如需有關平準任務的資訊，請參閱甘特圖中的平準資源。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# 更新任務平準延遲

有時候，專案上的任務排程之間可能會發生衝突。 您可以重新排程資源與工作，讓所有工作都能在現實的排程內完成，以平準資源或解決資源衝突。 如需有關平準任務的資訊，請參閱 [在甘特圖中平準資源](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

身為專案經理或任務受指派人，您也可以在個別任務上新增「平準延遲」，以說明任何資源或排程衝突。 換言之，一項任務可能會延遲排程，以確保Adobe Workfront在排程任務時能以更實際的排程克服資源衝突。

將平準延遲新增至任務會調整任務的「預計完成日期」。 有關預計完成日期的資訊，請參閱 [專案、任務和問題的預計完成日期總覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權 </p> <p>貢獻或更高的專案許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 將平準延遲新增至任務

1. 移至您要為其新增「平準延遲」的工作。
1. 按一下 **「更多」圖示** 在任務名稱的右側，然後按一下 **編輯**.

1. 按一下 **設定**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 指定 **平準延遲**，則以小時為單位，然後選擇時間單位。\
   這是資源因資源衝突而延遲啟動工作的時間。

   從下列時間單位選項中選取：

   * 分鐘
   * 小時。 這是預設值。
   * 天
   * 週
   * 個月
   * 經過的分鐘數
   * 經過的時數
   * 經過的天數
   * 經過的週數
   * 經過的月數

   >[!TIP]
   >
   >經過的時間是任務期間的時間單位。 這是任務的計劃開始日期與計畫完成日期之間的時間，包括假日、週末和休假。 換句話說，經過的時間就是行事曆的天數。

1. 按一下 **儲存**. 

 
