---
title: 建立和管理版面範本
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 身為Workfront管理員或群組管理員，您可以建立和修改版面範本，為使用者自訂Workfront中的版面元素。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 建立和管理版面範本

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Workfront管理員或群組管理員，您可以建立和修改版面範本，為使用者在Workfront中自訂下列版面元素：

* 主要選單
* 左側導覽面板
* 首頁
* 人們搭配清單和報表使用的檢視、篩選和分組。
* 螢幕術語

建立或修改版面範本後，您可以將其指派給個別使用者、團隊、群組或工作角色。

每個使用者的預設Workfront版面配置視其存取層級和授權類型而定。 例如，某些使用者在主功能表中可能看不到某些區域。 如需詳細資訊，請參閱 [關於預設Adobe Workfront版面](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立和管理版面範本的考量事項

* 使用者可以自訂自己版面的幾個區域。 當您變更版面範本時，您的變更會與他們所做的任何自訂項目合併，而不會覆寫或重設這些項目。 如果您將使用者指派給新的版面範本，也會是如此。
* 自2019年秋初移轉以來，您在Adobe Workfront Classic中建立的舊版面範本已自動提供給新Adobe Workfront體驗的執行個體。 在Adobe Workfront Classic中建立的版面範本在2020年4月移轉後。 建議您在新的Adobe Workfront體驗中更新這些版面範本，以充分運用新功能，並讓這些範本在該環境中更實用。
* 具有可編輯其他用戶的計畫許可證的組管理員和用戶可以在編輯其配置檔案時向他們可以管理的用戶添加系統級別和組級別佈局模板。
* 群組管理員無法將版面範本指派給工作角色或團隊。

如需版面範本的詳細資訊，請參閱 [版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## 建立或修改版面範本

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **介面** > **版面範本**.

1. 按一下 **新版面範本**.

   或

   按一下要修改的版面模板的名稱。

1. 如果要建立新的版面範本，請輸入 **版面範本名稱** 和（選用）a **說明** 為了它。

1. 自訂使用者介面的區域，如下列文章所述：

   * [使用版面範本自訂主功能表](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用版面範本自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用版面範本自訂已固定的頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用版面範本自訂「詳細資料」檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用版面範本自訂首頁和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用版面範本自訂登錄頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用版面範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用版面範本自訂使用者介面術語](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 繼續測試您的版面範本，並讓使用者能使用，如下文所述：

   * [測試新的版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予版面範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [將使用者指派至版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

您也可以複製新的版面範本並變更副本，以建立新的版面範本。 如需詳細資訊，請參閱 [復製版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
