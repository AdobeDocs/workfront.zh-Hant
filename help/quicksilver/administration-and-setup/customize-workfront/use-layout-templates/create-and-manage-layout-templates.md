---
title: 建立及管理版面範本
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 身為Workfront管理員或群組管理員，您可以建立和修改版面配置範本，以自訂使用者在Workfront中的版面配置元素。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 建立及管理版面範本

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員或群組管理員，您可以建立和修改版面配置範本，為使用者在Workfront中自訂下列版面配置元素：

* 主要功能表
* 左側導覽面板
* 主區域
* 人們用於清單和報告的檢視、篩選器和群組。
* 熒幕術語
* 專案、任務和問題標題

建立或修改版面配置範本後，您可以將其指派給個別使用者、專案團隊、群組或工作角色。

每位使用者的預設Workfront配置取決於其存取層級和授權型別。 例如，有些使用者可能不會在主功能表中看到某些區域。 如需詳細資訊，請參閱[關於預設Adobe Workfront配置](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
   或
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p>
<p>若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>附註</b>：</p> <p>如果您沒有存取權，請洽詢Workfront管理員，瞭解他們是否在您的存取層級設定其他限制。

如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
 </tbody> 
</table>

+++

## 建立及管理版面配置範本的考量事項

* 使用者可以自訂其自身配置的幾個區域。 當您變更版面配置範本時，您的變更會與其所做的任何自訂合併，而不會覆寫或重設它們。 如果您將使用者指派給新的版面配置範本，也會發生這種情況。
* 群組管理員和擁有計畫授權的使用者若能編輯其他使用者，可將系統層級和群組層級的版面配置範本新增到他們編輯個人資料時可管理的使用者中。
* 群組管理員無法將配置範本指派給工作角色或團隊。

如需配置範本的詳細資訊，請參閱[配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## 建立或修改版面範本

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**介面** > **配置範本**。

1. 按一下&#x200B;**新配置範本**。

   或

   按一下要修改的版面配置範本的名稱。

1. 如果您正在建立新的版面配置範本，請輸入&#x200B;**版面配置範本名稱**&#x200B;和（選擇性）它的&#x200B;**描述**。

1. 自訂使用者介面的區域，如下列文章所述：

   * [使用配置範本自訂主功能表](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用版面配置範本自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用版面配置範本自訂釘選頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用配置範本自訂首頁和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用版面配置範本自訂登入頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用版面配置範本自訂使用者介面術語](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 繼續測試您的版面配置範本，並提供給使用者使用，如下文所述：

   * [正在測試新的配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授與配置範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [將使用者指派至版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>您也可以複製配置範本並變更副本，以建立配置範本。 如需詳細資訊，請參閱[複製配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md)。

