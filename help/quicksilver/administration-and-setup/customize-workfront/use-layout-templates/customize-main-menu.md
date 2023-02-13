---
title: 使用版面範本自訂主功能表
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員或群組管理員，您可以使用配置範本，設定使用者在Workfront中開啟「主功能表」時看到的選項。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# 使用版面範本自訂主功能表

身為Adobe Workfront管理員或群組管理員，您可以使用配置範本，設定使用者在Workfront中開啟「主功能表」時看到的選項：

![主菜單選項](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>使用者看到的主功能表選項視其授權類型以及其存取層級中設定的設定而定。 有些使用此版面範本的使用者可能看不到您在此處選擇的所有選項。 如需詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 和 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權</strong></td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂主功能表

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下 **設定主菜單** 在右上角。

   在出現的「主菜單」(Main Menu)框中，您可以查看模板的「主菜單」中當前處於活動狀態的項以及可添加的項。 可新增的所有可能項目如下：

   * 首頁

      >[!TIP]
      >
      >預設情況下，「首頁」(Home)將顯示為「My Updates for Review-license」（查看許可證）用戶的「My Updates」（我的更新），除非他們具有與其配置檔案關聯的佈局模板，該佈局模板包含在主菜單中的「My Updates」（我的更新）區域。

   * 專案組合
   * 計劃
   * 專案
   * 報告
   * 儀表板
   * 行事曆
   * 資源分配
   * 情景

      >[!NOTE]
      >
      >方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md).

   * 團隊
   * 使用者

      >[!NOTE]
      >
      >只有具有計畫許可證的用戶才能看到用戶 ![](assets/users-icon-in-main-menu.png) 的下限。

   * 請求
   * 時程表
   * 文件
   * 範本
   * 分析
   * 校訂
   * 目標

      >[!NOTE]
      >
      >這需要額外的授權。 如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標概覽](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 我的更新
   * 面板
   * 藍圖

1. 執行下列任一操作：

   * 隱藏 ![](assets/remove-icon---x-in-circle.png) **作用中項目** 你不想展示
   * 顯示 ![](assets/add-icon-plus-in-circle.png) **可用項目** 顯示在「主菜單」中。
   * 拖曳 ![](assets/move-icon---dots.png) **作用中項目** 來更改其在主菜單中的顯示順序。

1. 按一下 **完成**.

   您也可以按一下 **取消** 在任何時候捨棄更改。

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後稍後繼續修改範本。

如需版面範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
