---
title: 將使用者指派至版面範本
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作為Adobe Workfront管理員，您可以將已建立的版面配置範本指派給任何需要使用的使用者、工作角色、團隊或群組。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 將使用者指派至版面配置範本

{{preview-fast-release-general}}

您可以將已建立的版面配置範本指派給任何需要使用的使用者、工作角色、團隊或群組。

若使用者未獲指派配置範本，則會使用預設配置。 若要瞭解預設配置，請參閱[關於預設Adobe Workfront配置](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

使用者也可以將版面配置範本指派給自己，如使用版面配置範本變更我的工作和工作請求區域中所述。

您可以將多個不同的配置範本指派給相同的名稱。 如需有關哪個配置範本對使用者、角色、群組或團隊有效的詳細資訊，請參閱本文稍後的[配置範本指派優先順序](#layout-template-assignment-priority)。

如需配置範本的詳細資訊，請參閱[配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
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

## 將版面配置範本指派給使用者

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。

   >[!TIP]
   >
   >當您滿意您的版面配置範本時，建議您進行測試，如[測試新的版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)中所述。

1. 按一下頁面頂端區段中的&#x200B;**將此指派給**。
1. 在出現的方塊中，按一下&#x200B;**新增使用者、工作角色、團隊或群組**，開始輸入使用者、工作角色、團隊或群組的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   最近新增的名稱會以藍色背景顯示。 當您編輯現有版面配置範本時，這會很有幫助，因為您可以區分您剛才新增的名稱與清單中已有的名稱。

   資訊圖示![資訊圖示](assets/info-icon.png)會顯示在已指派給其他配置範本的任何使用者、工作角色、團隊或群組名稱的右側。 您可以將滑鼠停留在圖示上以檢視該配置範本的名稱，並決定是否要覆寫現有的指派。

1. 視需要重複前兩個步驟，將版面配置範本指派給其他使用者、工作角色、團隊或群組。

   您一次最多可以指派100個使用者。

1. 按一下&#x200B;**完成**，然後按一下左下角的&#x200B;**儲存**&#x200B;或&#x200B;<span class="preview">**儲存並關閉**</span>。

   此步驟會完成建立及指派配置圖範本的程式。

## 版面配置範本指派優先順序 {#layout-template-assignment-priority}

您和其他Workfront管理員可以透過以下四種方式，將多個不同的配置範本指派給相同的使用者：

* 至個別使用者
* 至使用者擁有的特定工作角色
* 使用者所在的特定團隊
* 至使用者所在的特定群組

但是，使用者在任何給定時間都只能看到一個版面範本。 可見的範本由以下優先順序階層決定：

* **個別使用者**：以個別使用者的身分指派給此人的版面配置範本會覆寫其他所有使用者。 您可以透過新的指派來覆寫先前為個別使用者進行的指派；最近的指派優先。
* **主要工作角色**：如果人員未獲指派配置範本為單一使用者，他們會看到為其主要工作角色指派的範本。

  使用者只會看見指派給使用者主要工作角色的版面配置範本。 指派給使用者所擁有的任何次要職務角色的範本不可見。

* **主團隊**：如果人員未被指派為個人使用者或具有主要工作角色的使用者配置範本，他們會看到指派給其主團隊的範本。

  使用者只會看到指派給使用者主團隊的範本。 指派給使用者所屬之其他團隊的範本不可見。

* **首頁群組**：如果人員未被指派為個人使用者、具有主要工作角色的使用者或首頁團隊的成員，他們會看到指派給其首頁群組的範本。

  使用者只會看見指派給使用者「首頁」群組的範本。 指定給其他群組的範本不可見。

## 指派給版面配置範本的大量使用者

<!--If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
如果要將超過2000名使用者指派給版面配置範本，建議您執行下列任一項作業：

* 將使用者組織成群組或專案團隊，並將版面配置範本指派給這些群組或專案團隊。 如需詳細資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)和[建立及管理團隊](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)。

* 將職位角色指派給使用者，並將版面配置範本指派給其主要職位角色。 如需詳細資訊，請參閱[建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。
