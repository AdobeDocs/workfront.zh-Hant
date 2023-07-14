---
title: 建立和管理版面範本
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 身為Workfront管理員或群組管理員，您可以建立和修改版面配置範本，以針對使用者自訂Workfront中的版面配置元素。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 建立和管理版面範本

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Workfront管理員或群組管理員，您可以建立和修改版面配置範本，以針對您的使用者在Workfront中自訂下列版面配置元素：

* 主要選單
* 左側導覽面板
* 主區域
* 檢視、篩選器和群組人員用於清單和報告。
* 熒幕術語

建立或修改版面配置範本後，您可以將其指派給個別使用者、團隊、群組或工作角色。

每位使用者的預設Workfront配置取決於其存取層級和授權型別。 例如，有些使用者可能不會在主功能表中看到某些區域。 如需詳細資訊，請參閱 [關於預設Adobe Workfront配置](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立和管理版面範本的考量事項

* 使用者可以自訂自己版面的幾個區域。 當您變更版面配置範本時，您的變更會與其所做的任何自訂合併，而不會覆寫或重設它們。 如果您將使用者指派給新的版面配置範本，也會發生這種情況。
* 您在Adobe Workfront Classic中建立的舊版面範本，自2019年秋初移轉後，現在已可自動用於新Adobe Workfront Experience的執行個體。 2020年4月，在Adobe Workfront Classic中建立並移轉的版面配置範本。 建議您更新新Adobe Workfront體驗中的這些版面範本，以運用新功能，並讓這些範本在該環境中更加實用。
* 擁有計畫授權且可以編輯其他使用者的群組管理員和使用者可以將系統層級和群組層級版面範本新增到他們可以在編輯其設定檔時管理的使用者中。
* 群組管理員無法將版面配置範本指派給工作角色或團隊。

如需版面配置範本的詳細資訊，請參閱 [版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## 建立或修改版面範本

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **介面** > **版面配置範本**.

1. 按一下 **新版面範本**.

   或

   按一下要修改的版面配置範本名稱。

1. 如果要建立新的版面範本，請鍵入 **版面配置範本名稱** 和（選用） a **說明** 為了它。

1. 自訂使用者介面的區域，如下列文章所述：

   * [使用版面配置範本自訂主功能表](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用版面配置範本自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用版面配置範本自訂釘選頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用版面配置範本自訂首頁和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用版面配置範本自訂登入頁面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用版面配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用版面配置範本自訂使用者介面術語](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 繼續測試您的版面配置範本，並提供給使用者使用，如下文所述：

   * [測試新版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予配置範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [將使用者指派至版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

您也可以複製並變更副本，以建立新的版面範本。 如需詳細資訊，請參閱 [復製版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
