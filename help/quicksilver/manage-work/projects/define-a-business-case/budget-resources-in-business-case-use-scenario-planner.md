---
navigation-topic: business-case-and-scorecards
title: 使用案例規劃工具之業務案例中的預算資源
description: 作為資源計畫的一部分，當您建立業務案例時，可以使用Adobe Workfront案例規劃工具來預算完成專案中工作所需的職務角色。
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# 使用案例規劃工具之業務案例中的預算資源

<!--Audited: 06/2025-->

作為資源計畫的一部分，當您建立業務案例時，可以使用Adobe Workfront案例規劃工具來預算完成專案中工作所需的職務角色。

如需建立業務案例的詳細資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

>[!TIP]
>
>當您發佈方案時，專案業務案例的「資源預算」區域中會顯示連結至您於系統層次「案例規劃工具」中所輸入專案之方案的工作角色資訊。 Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。

您也可以使用資源規劃工具，為業務案例中的資源編列預算。 如需詳細資訊，請參閱下列內容：

* [業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>建議您在開始處理專案時，決定使用資源規劃工具或情境規劃工具。 在專案生命週期中經常在這兩個之間切換，可能會造成您為專案編列資源預算的方式不一致。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td><p>目前： Ultimate</p> 
   <p>舊版：商務或更新版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p>目前：淺色或更高 
   <p>舊版：檢閱或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>產品</p></td> 
   <td><p>情境規劃工具包含在目前的Ultimate Workfront計畫中。</p> 
   <p>針對舊版Workfront計畫，除了Workfront授權外，您必須購買Adobe Workfront情境規劃工具的授權，才能存取本文所述功能。</p> <p>如需有關取得Workfront Scenario Planner的資訊，請參閱<a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用Scenario Planner所需的存取權</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>編輯下列專案的存取權： </p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>財務資料</p> </li> 
     <li> <p>情境規劃工具 </p> </li> 
    </ul> <p>如需有關預算資源所需存取許可權的資訊，另請參閱<a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">在Adobe Workfront中預算資源所需的存取許可權</a>。</p> <p>注意：如果您還是沒有存取權，請詢問您的Adobe Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須執行下列動作：

* 使用「情境規劃工具」建立計畫。

  如需詳細資訊，請參閱[在Scenario Planner](../../../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

* 在計畫上建立方案，並將其連結至專案。

  請務必指明方案所需的工作角色資訊，並使用此資訊更新連結的專案。

  如需詳細資訊，請參閱下列文章：

   * [在Scenario Planner中建立和編輯方案](../../../scenario-planner/create-and-edit-initiatives.md)
   * [將專案匯入至「情境規劃工具」中的計畫](../../../scenario-planner/import-projects-to-plans.md)
   * [在Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md)中發佈行動方案以更新或建立專案。

* 雖然這些並非必要條件，我們仍建議您採取下列步驟：

   * 將專案上的任務指派給案例規劃工具中預算的工作角色。
   * 表示專案上任務的計畫時數。

     這有助於您瞭解任務可能需要完成的工作量，有助於決定資源應編列預算多長時間來完成任務。

     如需將任務與計畫時數建立關聯的資訊，請參閱[編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 針對連結至方案的專案，使用案例規劃工具之業務案例中的預算資源

>[!IMPORTANT]
>
>您可以為資源編列為期15年的預算。 如果您為持續期間超過15年的專案編列資源預算，預算資訊可能不準確。
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. 移至您要編列資源預算的專案。

   >[!TIP]
   >
   >此專案連結至「情境規劃工具」中的方案，其連結的方案已發佈至少一次。

1. 按一下左側面板中的&#x200B;**業務案例**。
1. （視條件而定）在&#x200B;**資源預算**&#x200B;區段中，執行下列其中一項作業：

   * 如果您剛從「情境規劃工具」發佈資訊，請在「資源預算」區域中選取「情境規劃工具」**選擇要用於計算專案預算勞力成本的時數**，然後按一下&#x200B;**選擇**。

     ![資源規劃工具中的業務案例與選擇按鈕](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * 如果先前已針對專案的預算資源選取資源規劃工具，請按一下&#x200B;**變更** > **情境規劃工具** > **選擇**。

     ![具有「選擇」按鈕的情境規劃工具中的業務案例](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront使用連結行動方案中的所需職務角色時數，來計算專案的預算勞力成本和預算時數。 這是建議的選項。 成本會以專案的貨幣顯示在業務案例中。

     當您複製專案並選擇將預算時數複製到新專案時，使用案例規劃工具的預算時數未複製到新專案。 僅複製資源規劃工具中的預算時數。 如需詳細資訊，請參閱[複製專案](../manage-projects/copy-project.md)。

     >[!IMPORTANT]
     >
     >當您使用「情境規劃工具」為專案編列資源預算時，「預算勞力成本」會顯示在Workfront的下列區域中：
     >
     >   
     >   
     >   * 業務案例的資源預算區域
     >   * 系統層級「情境規劃工具」為連結至專案的方案的「人員成本」。 如需詳細資訊，請參閱[在Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。
     >   
     >

1. （選擇性）按一下「情境規劃工具」中的&#x200B;**檢視**&#x200B;以開啟包含連結至專案的方案之計畫。 這會在新的瀏覽器標籤中開啟「情境規劃工具」。
1. （選用）更新方案資訊。 如需詳細資訊，請參閱[在Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

   >[!NOTE]
   >
   >每次變更專案上的資源預算區域後，您必須發佈方案以進行更新。
