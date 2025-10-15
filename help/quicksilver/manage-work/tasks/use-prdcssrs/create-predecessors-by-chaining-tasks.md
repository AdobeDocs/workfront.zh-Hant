---
product-area: projects
navigation-topic: use-predecessors
title: 透過鏈結任務建立前置任務關係
description: 您可以在Adobe Workfront中以多種方式建立前置任務關係。 一種方法是透過鏈結任務。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 透過鏈結任務建立前置任務關係

您可以在Adobe Workfront中以多種方式建立前置任務關係。 一種方法是透過鏈結任務。

如需前置任務的相關資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

透過鏈結任務，您可以允許系統在所選任務上自動建立前置任務關係，而不是在自己手動建立每個任務上的關係。 任務之間仍然可以使用不同的前置任務關係型別。

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
   <td><p>標準</p> 
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 鏈結任務以建立前置任務關係

1. 移至包含您要鏈結之任務的專案。
1. 按一下左側面板中的&#x200B;**工作**。
1. （視條件而定）選取工作清單右上角的&#x200B;**自動儲存**，然後選取您要鏈結的工作。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >當您手動儲存對任務的變更或使用「時間表計畫」模式儲存任務時，無法在任務清單中鏈結任務。

1. 以滑鼠右鍵按一下選取的工作，然後按一下&#x200B;**鏈結**。
1. 從下列相依性型別中選取：

   * **完成 — 開始**
   * **完成 — 完成**
   * **開始 — 開始**
   * **開始 — 完成**

   如需前置任務相依性型別的詳細資訊，請參閱[任務相依性型別概觀](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. （選擇性）如果某些工作先前已鏈結，請按一下&#x200B;**取消鏈結**。

   >[!CAUTION]
   >
   >大量編輯任務時，只有使用取消鏈結選項會移除循序前置任務。

   您選取的任務現在由前置任務關係連結。
