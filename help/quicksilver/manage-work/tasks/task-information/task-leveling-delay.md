---
product-area: projects
navigation-topic: task-information
title: 更新任務調平延遲
description: 有時，項目上的任務計畫之間可能會發生衝突。 您可以通過重新計畫資源和任務來分級資源或解決資源衝突，以便所有任務都可以在實際的計畫內完成。 有關調平任務的資訊，請參閱甘特圖中的「級資源」。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# 更新任務調平延遲

有時，項目上的任務計畫之間可能會發生衝突。 您可以通過重新計畫資源和任務來分級資源或解決資源衝突，以便所有任務都可以在實際的計畫內完成。 有關調平任務的資訊，請參閱 [甘特圖中的層資源](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

作為項目經理或任務受託人，您還可以在單個任務上添加「調平延遲」，以處理任何資源或計畫衝突。 換句話說，可以延遲排程任務，以確保當Adobe Workfront將任務分級時，更現實的排程能克服資源衝突。

向任務添加調平延遲可調整任務的預計完成日期。 有關預計完成日期的資訊，請參閱 [項目、任務和問題的預計完成日期概覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務權限 </p> <p>為專案貢獻或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 向任務添加調平延遲

1. 轉到要添加「調平延遲」的任務。
1. 按一下 **更多圖示** 在任務名稱的右側，然後按一下 **編輯**.

   ![](assets/qs-task-edit-icon-highlighted-350x154.png)

1. 按一下 **設定**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 指定 **調平延遲**，以小時為單位，然後選擇時間單位。\
   這是資源因資源衝突而延遲開始任務的時間。

   從下列時間單位選項中選取：

   * 分鐘
   * 時數. 這是預設值。
   * 天
   * 週
   * 月
   * 經過的分鐘數
   * 經過的時數
   * 經過的天數
   * 經過的週數
   * 經過的月數

   >[!TIP]
   >
   >已用時間是任務持續時間的單位。 它是任務（包括節假日、週末和休假時間）的「計畫起始日期」和「計畫完成日期」之間的時間。 換句話說，經過的時間是日曆天數的過去。

1. 按一下 **儲存**. 

 
