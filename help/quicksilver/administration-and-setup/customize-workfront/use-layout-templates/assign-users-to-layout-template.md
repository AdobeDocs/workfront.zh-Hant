---
title: 將使用者指派至版面範本
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員，您可以將您建立的版面範本指派給需要使用的任何使用者、工作角色、團隊或群組。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# 將使用者指派至版面範本

您可以將您建立的版面範本指派給需要使用的任何使用者、工作角色、團隊或群組。

對於未指派配置範本的使用者，會使用預設配置。 若要了解預設版面，請參閱 [關於預設Adobe Workfront版面](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

用戶也可以為自己分配佈局模板，如使用佈局模板更改「我的工作」和「工作請求」區域中所述。

您可以將多個不同的版面範本指派給相同名稱。 有關對用戶、角色、組或團隊有效的佈局模板的詳細資訊，請參閱 [佈局模板分配優先順序](#layout-template-assignment-priority) 稍後的文章。

如需版面範本的詳細資訊，請參閱 [版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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

## 將版面範本指派給使用者

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >當您對版面範本感到滿意時，建議您測試，如 [測試新的版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. 按一下 **將此項指派給** 在頁面頂端的區段中。
1. 在出現的方塊中，按一下 **添加用戶、作業角色、團隊或組**，開始鍵入用戶、作業角色、團隊或組的名稱，然後在下拉清單中顯示名稱時按一下該名稱。

   最近新增的名稱會顯示為藍色背景。 當您編輯現有的版面範本時，這個方法很有幫助，因為您可以區分剛新增的名稱和清單中已新增的名稱。

   資訊圖示 ![](assets/info-icon.png) 顯示在已分配給其他佈局模板的任何用戶、作業角色、團隊或組的名稱的右側。 您可以將滑鼠指標暫留在圖示上，查看該版面範本的名稱，並決定是否要覆寫現有指派。

1. 重複前述兩個步驟，視需要將版面範本指派給其他使用者、工作角色、團隊或群組。

   您一次最多可指派100位使用者。

1. 按一下 **完成**，然後按一下 **儲存** 左下角。

   此步驟會完成建立和指派配置範本的程式。

## 佈局模板分配優先順序 {#layout-template-assignment-priority}

您和其他Workfront管理員可以透過以下四種不同方式，將多個不同的版面範本指派給相同的使用者：

* 對個別使用者
* 對用戶具有的特定作業角色
* 對用戶所在的特定團隊
* 至使用者所在的特定群組

不過，使用者在任何指定時間都只能看到一個版面範本。 可見的範本由下列優先順序階層決定：

* **個別使用者**:指派給個別使用者之人員的版面範本會覆寫所有其他使用者。 您可以通過進行新分配來覆蓋先前分配，以便單個用戶；最近的一個優先。
* **主要作業角色**:如果人員未以單一使用者身分指派配置範本，則他們會看到為其主要工作角色指派的範本。

   只有分配給用戶的主要作業角色的佈局模板才對用戶可見。 分配給用戶所擔任的任何輔助作業角色的模板不可見。

* **主隊**:如果人員未以個別使用者或具有主要工作角色的使用者身分，將配置範本指派給其首頁團隊，則他們會看到指派給其的範本。

   只有指派給使用者之主團隊的範本才會顯示給使用者。 分配給用戶是成員的其他團隊的模板不可見。

* **首頁組**:如果人員未以個別使用者、具有主要工作角色的使用者或主團隊的成員身分，將配置範本指派給其主群組，則他們會看到指派給其主群組的範本。

   只有指派給使用者之首頁群組的範本才會顯示給使用者。 指派給其任何其他群組的範本不會顯示。

## 分配給佈局模板的大量用戶

如果您編輯分配給2000多名用戶的版面模板並進行更改，則只有前2000名用戶才會保留在版面模板上，並且會看到您所做的更改。 版面範本會從所有其他項目中移除。

如果要指派給版面範本的使用者超過2000名，建議您執行下列其中一項作業：

* 將使用者組織成群組或團隊，並將版面範本指派給這些群組或團隊。 如需詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [建立和管理團隊](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* 將作業角色指派給使用者，並將配置範本指派給其主要作業角色。 如需詳細資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
