---
title: 使用版面配置範本自訂主功能表
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在Workfront中開啟「主要」功能表時看到的選項。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 4%

---

# 使用版面配置範本自訂主功能表

{{preview-fast-release-general}}

<!--Audited: 01/2024-->

作為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在Workfront中開啟「主要」功能表時看到的選項。

>[!NOTE]
>
>使用者看到的主要功能表選項取決於其授權型別以及在其存取層級中設定的設定。 某些將使用此配置範本的使用者可能不會看見您在這裡選擇的所有選項。 如需詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)以及[每個物件型別可設定的功能存取權](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)。
>
>如果您的組織已上線Adobe Workfront Unified Experience，您可能會在主要功能表中看到不同的選項。 如需詳細資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

如需有關建立版面配置範本的資訊，請參閱[建立和管理版面配置範本](../use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p>
       <p>將自訂應用程式新增至主功能表僅適用於授權Adobe App Builder的組織。</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p>
        <p>若要為群組執行這些動作，您必須是該群組的管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自訂主要功能表

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下範本右上角的&#x200B;**設定主功能表**。

   「主選單」方塊開啟，您可以看到目前顯示在範本的「主選單」中的區域，以及可新增的專案。 以下是您可以新增的所有可能專案：
   * 首頁

     >[!TIP]
     >
     >依預設，主功能表中的「首頁」圖示會顯示「我的更新」區域給檢閱授權使用者（在目前的授權計畫中），除非他們有一個與其設定檔相關聯的版面範本，其中除了「首頁」區域外，還包括主功能表中的「我的更新」區域。

   * 專案組合
   * 計劃
   * 專案
   * 報告
   * 儀表板
   * 行事曆
   * 資源分配
   * 方案

     >[!NOTE]
     >
     >Scenario Planner需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。

   * 團隊
   * 使用者

     >[!NOTE]
     >
     >只有擁有計畫授權的使用者（在目前的授權模式中）或擁有標準授權的使用者（在新的授權模式中），才能在主要功能表中看到使用者區域![使用者圖示](assets/users-icon-in-main-menu.png)。

   * 請求
   * 時程表
   * 文件
   * 範本
   * 目標

     >[!NOTE]
     >
     >目標需要額外的授權。 如需Workfront目標的相關資訊，請參閱[Adobe Workfront目標總覽](../../../workfront-goals/goal-management/wf-goals-overview.md)。

   * 我的更新
   * 展示板
   * 藍圖
   * 計畫

     >[!NOTE]
     >
     >Planning需要額外的授權。 如需Workfront Planning的相關資訊，請參閱[Adobe Workfront Planning概觀](/help/quicksilver/planning/general/planning-overview.md)。

   * 自訂應用程式

     >[!NOTE]
     >
     > 自訂應用程式必須個別建立，才能作為主功能表選項使用。 如需詳細資訊，請參閱[使用Adobe App Builder建立Workfront的自訂應用程式](/help/quicksilver/app-builder/app-builder.md)。

1. 執行下列任一項作業：

   * 隱藏![隱藏圖示](assets/remove-icon---x-in-circle.png) **您不想要顯示的作用中專案**
   * 顯示您想要顯示在主功能表上的![顯示圖示](assets/add-icon-plus-in-circle.png) **可用專案**。
   * 拖曳![拖曳圖示](assets/move-icon---dots.png) **作用中專案**&#x200B;以變更它們在主功能表上的顯示順序。

1. 按一下「**完成**」。

   如果您要捨棄變更，也可以隨時按一下&#x200B;**取消**。

1. <span class="preview">在預覽環境中：繼續自訂版面範本。 您可以隨時按一下&#x200B;**套用**&#x200B;以儲存進度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自訂，請按一下&#x200B;**儲存並關閉**。</span>

1. 在生產環境中：繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >您可以隨時按一下[儲存]來儲存進度，然後再繼續修改範本。****

如需配置範本的詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
