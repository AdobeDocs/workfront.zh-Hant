---
product-area: projects
navigation-topic: manage-tasks
title: 將里程碑與任務建立關聯
description: 您可以將里程碑與任務建立關聯，以指出您在專案存留期中何時達到重要步驟。 您必須先將里程碑路徑與專案相關聯，然後才能將里程碑與專案上的任務相關聯。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# 將里程碑與任務建立關聯

<!--Audited: 01/2024-->

您可以將里程碑與任務建立關聯，以指出您在專案存留期中何時達到重要步驟。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先決條件

在您將里程碑與任務關聯之前，必須存在下列專案：

* Workfront管理員必須建立里程碑路徑，如[建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)中所述。

* 您必須將里程碑路徑關聯至專案。

  如需詳細資訊，請參閱[編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

* 若要將里程碑路徑與專案產生關聯，專案必須處於「計畫」或「目前」狀態。

  >[!TIP]
  >
  >若要使用「里程碑」檢視取得專案中里程碑進度的最佳總覽，您應該建立父系任務，並將其與專案的每個主要階段建立關聯。 然後，將這些父系任務與里程碑路徑的每個里程碑相關聯。

## 將里程碑與任務相關聯

里程碑路徑與專案相關聯後，任務可指派為里程碑。

1. 前往工作，然後按一下工作名稱右側的&#x200B;**更多**&#x200B;圖示![](assets/more-icon.png)，然後&#x200B;**編輯**。

   任務和里程碑具有1:1關係。 您無法將相同的里程碑附加到多個任務。 每個任務都可以連結至單一里程碑，或者每個里程碑都可以對應至一個任務。

1. 按一下&#x200B;**設定**，然後在&#x200B;**里程碑**&#x200B;欄位中為任務選取里程碑。
1. 按一下「**儲存**」。
1. （選擇性）在工作清單中，新增&#x200B;**狀態圖示**&#x200B;欄，以識別哪些工作具有里程碑。 里程碑菱形指示器會顯示在「狀態圖示」欄中。

   如需詳細資訊，請參閱[在Adobe Workfront中建立或編輯檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)。

   ![](assets/amwt3.png)

1. （選擇性）前往專案清單，選取&#x200B;**里程碑**&#x200B;檢視以識別里程碑任務的進度。

   ![](assets/milestone-view-project-list.png)
