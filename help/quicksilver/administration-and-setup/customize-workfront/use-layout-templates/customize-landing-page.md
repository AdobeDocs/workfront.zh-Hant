---
title: 使用版面配置範本自訂登入頁面
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Workfront管理員，您可以使用版面配置範本來指定使用者每次登入Workfront時想要看到的區域。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 8%

---

# 使用版面配置範本自訂登入頁面

{{preview-fast-release-general}}

身為Adobe Workfront管理員，您可以使用版面配置範本來指定使用者每次登入Workfront時想要看到的區域。

使用者可以開啟下列其中一項：

* 指定的Workfront區域
* 自訂儀表板。

如需有關建立版面配置範本的資訊，請參閱[建立和管理版面配置範本](../use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

>[!NOTE]
>
>當請求設定為登入頁面時，指派給版面配置範本的貢獻者或請求者使用者會改為檢視首頁作為登入頁面。 除了針對投稿人或請求者使用者的版面配置範本請求外，建議選擇登陸頁面。

## 存取需求

+++ 展開以查看此文章中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 套件</td> 
   <td><p>任何</p></td> 
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

## 自訂登入頁面

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 在&#x200B;**上層導覽區域**&#x200B;中，按一下&#x200B;**選取登陸頁面**，然後選取使用者登入時您想要看到的區域。

   從下列區域選取，或新增自訂儀表板：

   * 行事曆
   * 儀表板
   * 文件
   * 目標
   * 首頁
   * 我的更新
   * 專案組合
   * 計劃
   * 專案
   * 報告
   * 請求
   * 資源分配
   * 方案
   * 團隊
   * 範本
   * 時程表
   * 使用者
   * 藍圖
   * 計畫

   >[!IMPORTANT]
   >
   >若要檢視「案例」、「目標」和「規劃」區域，需要額外的授權。
   >
   >* 如需Workfront目標的相關資訊，請參閱[Adobe Workfront目標總覽](../../../workfront-goals/goal-management/wf-goals-overview.md)。
   >
   >* 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。
   >
   >* 如需Workfront Planning的相關資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

1. <span class="preview">在預覽環境中：繼續自訂版面範本。 您可以隨時按一下&#x200B;**套用**&#x200B;以儲存進度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自訂，請按一下&#x200B;**儲存並關閉**。</span>

1. 在生產環境中：繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >您可以隨時按一下[儲存]來儲存進度，然後再繼續修改範本。**&#x200B;**
