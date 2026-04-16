---
title: 建立和管理版面範本
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 身為Workfront管理員或群組管理員，您可以建立和修改版面配置範本，以自訂使用者在Workfront中的版面配置元素。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 5%

---

# 建立和管理版面配置範本

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員或群組管理員，您可以建立和修改版面配置範本，為使用者在Workfront中自訂下列版面配置元素：

* 主要功能表
* 左側導覽面板
* 主區域
* 摘要面板
* 人們用於清單和報告的檢視、篩選器和群組。
* 熒幕術語
* 物件標頭
* 物件的「更多」選單（三點選單）

建立或修改版面配置範本後，您可以將其指派給個別使用者、專案團隊、群組或工作角色。

每位使用者的預設Workfront配置取決於其存取層級和授權型別。 例如，有些使用者可能不會在主功能表中看到某些區域。 如需詳細資訊，請參閱[關於預設Adobe Workfront配置](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
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

## 建立及管理版面配置範本的考量事項

* 使用者可以自訂其自身配置的幾個區域。 當您變更版面配置範本時，您的變更會與其所做的任何自訂合併，而不會覆寫或重設它們。 如果您將使用者指派給新的版面配置範本，也會發生這種情況。
* 群組管理員和擁有計畫授權的使用者若能編輯其他使用者，可將系統層級和群組層級的版面配置範本新增到他們編輯個人資料時可管理的使用者中。
* 群組管理員無法將配置範本指派給工作角色或團隊。

如需配置範本的詳細資訊，請參閱[配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

## 建立或修改版面範本

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**介面** > **配置範本**。

1. 按一下&#x200B;**新配置範本**。

   或

   按一下要修改的版面配置範本的名稱。

1. 如果您正在建立新的版面配置範本，請輸入&#x200B;**版面配置範本名稱**&#x200B;和（選擇性）它的&#x200B;**描述**。

1. 自訂使用者介面的區域，如下列文章所述：

   * [使用版面配置範本自訂主功能表](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用版面配置範本自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用版面配置範本自訂「更多」選單](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-more-menu.md)
   * [使用版面配置範本自訂釘選頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用版面配置範本自訂摘要面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用版面範本自訂首頁](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [使用版面配置範本自訂登入頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用版面配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用版面配置範本自訂使用者介面術語](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 繼續測試您的版面配置範本，並提供給使用者使用，如下文所述：

   * [測試新的配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授與配置範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [將使用者指派至版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>您也可以復製版面範本並變更複製的版本，以建立版面範本。 如需詳細資訊，請參閱[複製配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md)。

