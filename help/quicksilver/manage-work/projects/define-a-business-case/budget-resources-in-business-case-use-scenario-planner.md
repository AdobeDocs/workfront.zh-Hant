---
navigation-topic: business-case-and-scorecards
title: 使用方案計畫器在業務案例中的預算資源
description: 作為資源計畫的一部分，您可以使用Adobe Workfront方案計畫器來預算在構建業務案例時完成項目中的工作所需的任務職責。
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 使用方案計畫器在業務案例中的預算資源

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

作為資源計畫的一部分，您可以使用Adobe Workfront方案計畫器來預算在構建業務案例時完成項目中的工作所需的任務職責。

有關建立業務案例的詳細資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>在系統層方案計畫器中輸入的與項目連結的方案的任務職責資訊，在您發佈方案時，將顯示在項目業務案例的「資源預算」區域中。 方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md).

您也可以使用資源計畫器來預算業務案例中的資源。 如需詳細資訊，請參閱下列內容：

* [業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>建議您在開始處理項目時決定是使用資源計畫員還是方案計畫員。 在專案期間經常在兩者之間切換，可能會造成您為專案預算資源的方式不一致。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>業務或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須為Adobe Workfront方案規劃器購買額外的許可證，才能訪問本文所述的功能。</p> <p>有關獲取Workfront方案計畫程式的資訊，請參閱 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用方案計畫員所需的訪問權限</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下項目的存取權： </p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>財務資料</p> </li> 
     <li> <p>案例規劃工具 </p> </li> 
    </ul> <p>有關訪問預算資源所需的資訊，另請參閱 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">獲得Adobe Workfront預算資源所需資源</a>.</p> <p>注意：如果您仍無權存取，請洽詢您的Adobe Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須執行下列操作：

* 使用方案計畫員建立計畫。

   如需詳細資訊，請參閱 [在方案計畫員中建立和編輯計畫](../../../scenario-planner/create-and-edit-plans.md).

* 建立計畫方案並將其連結到項目。

   請確保為方案指定所需的職務職責資訊，並使用此資訊更新連結的項目。

   如需詳細資訊，請參閱下列文章：

   * [在方案計畫器中建立和編輯方案](../../../scenario-planner/create-and-edit-initiatives.md)
   * [將項目導入方案計畫器中的計畫](../../../scenario-planner/import-projects-to-plans.md)
   * [通過在方案計畫器中發佈方案來更新或建立項目](../../../scenario-planner/publish-scenarios-update-projects.md).

* 雖然這些不是先決條件，但我們也建議：

   * 將項目上的任務分配給方案計畫員中預算的任務職責。
   * 指定項目任務的計畫小時數。

      這有助於您了解任務可能需要完成的工作量，從而有助於決定完成任務所需的資源預算時間。

      有關將任務與計畫小時數關聯的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 在業務案例中，使用方案計畫器對連結至方案的項目進行預算資源

>[!IMPORTANT]
您可以將資源預算為15年。 如果為持續時間超過15年的項目預算資源，則預算資訊可能不準確。
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. 轉到要為其預算資源的項目。

   >[!TIP]
   這是與方案規劃器中的方案連結的項目，其連結的方案至少已發佈一次。

1. 按一下 **業務案例** 中。
1. （有條件）在 **資源預算** 部分，執行下列操作之一：

   * 如果您剛從方案計畫員發佈資訊，請在 **選擇要用於計算項目預算人工成本的小時數** 欄位，然後按一下 **選擇**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * 如果先前為項目預算資源選擇了資源計畫器，請按一下 **變更** > **方案計畫員** > **選擇**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront使用連結計畫中所需的工作職責小時數來計算項目的預算人工成本和預算工時。 這是建議的選項。 成本以項目的幣種顯示在「業務案例」中。

      <!--drafted for Budgeted Hours:
   <span class="preview">在複製項目並選擇將預算小時數複製到新項目時，使用方案計畫程式編製預算的小時數不會複製到新項目。 系統僅複製資源計畫員中預算的小時數。 如需詳細資訊，請參閱 [複製專案](../manage-projects/copy-project.md)</span>
-->

   >[!IMPORTANT]
   > 
   >使用方案計畫器來預算項目資源時，預算的人工成本將顯示在Workfront的以下區域：
   >* 業務案例的資源預算區
   >* 系統層的方案計畫器作為與項目連結的計畫的人員成本。 如需詳細資訊，請參閱 [在方案計畫器中建立和編輯方案](../../../scenario-planner/create-and-edit-initiatives.md).


1. （選用）按一下 **在方案計畫器中查看** 開啟包含與項目連結的方案的計畫。 這將在新瀏覽器頁簽中開啟方案規劃器。
1. （可選）更新計畫的資訊。 如需詳細資訊，請參閱 [在方案計畫器中建立和編輯方案](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   > 
   >在項目上的「資源預算編製」區域的每次更改後，您必須發佈方案以進行更新。
