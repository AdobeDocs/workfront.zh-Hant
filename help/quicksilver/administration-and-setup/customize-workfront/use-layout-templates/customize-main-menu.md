---
title: 使用版面配置範本自訂主功能表
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在Workfront中開啟「主要」功能表時看到的選項。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 4%

---

# 使用版面配置範本自訂主功能表

<!--Audited: 01/2024-->

作為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在Workfront中開啟「主要」功能表時看到的選項。

![主要功能表選項](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>使用者看到的主要功能表選項取決於其授權型別以及在其存取層級中設定的設定。 某些將使用此配置範本的使用者可能不會看見您在這裡選擇的所有選項。 如需詳細資訊，請參閱 [存取層級和許可權如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 和 [可設定的每種物件型別功能存取權](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

如需有關建立版面配置範本的資訊，請參閱 [建立及管理版面範本](../use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需有關指派配置範本給使用者的資訊，請參閱 [將使用者指派至版面配置範本](../use-layout-templates/assign-users-to-layout-template.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td><p>目前：計畫</p>
   或
   <p>新增：標準</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p>
    <p>若要為群組執行這些動作，您必須是該群組的管理員。</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 自訂主要功能表

1. 開始使用版面範本，如所述 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下 **設定主功能表** 在範本的右上角。

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
   * 情境

     >[!NOTE]
     >
     >Scenario Planner需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱 [情境規劃工具概觀](../../../scenario-planner/scenario-planner-overview.md).

   * 團隊
   * 使用者

     >[!NOTE]
     >
     >只有具有「計畫」許可證的使用者（在目前的許可證模型中）或具有「標準」許可證的使用者（在新的許可證模型中），才能看到「使用者」區域 ![](assets/users-icon-in-main-menu.png) 在主要功能表中。

   * 請求
   * 時程表
   * 文件
   * 範本
   * 分析
   * 校訂
   * 目標

     >[!NOTE]
     >
     >目標需要額外的授權。 如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標總覽](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 我的更新
   * 展示板
   * 藍圖

1. 執行下列任一項作業：

   * 隱藏 ![](assets/remove-icon---x-in-circle.png) **使用中的專案** 您不想要顯示的專案
   * 顯示 ![](assets/add-icon-plus-in-circle.png) **可用專案** 您想要顯示在主功能表上的資訊。
   * 拖曳 ![](assets/move-icon---dots.png) **使用中的專案** 以變更主功能表的顯示順序。

1. 按一下 **完成**.

   您也可以按一下 **取消** 隨時放棄變更。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後繼續修改範本。

如需版面配置範本的詳細資訊，請參閱 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
