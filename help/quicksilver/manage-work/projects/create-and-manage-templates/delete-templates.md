---
product-area: templates
navigation-topic: templates-navigation-topic
title: 刪除專案範本
description: 我們建議您停用不再使用的範本，而不是刪除它們，以便您可以保留有關您專案的長期歷史資訊。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 87bf2a4485d3b0c29fcfe8e00dcca57874cdec04
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 刪除專案範本

我們建議您停用不再使用的範本，而不是刪除它們，以便您可以保留有關您專案的長期歷史資訊。 如需停用範本的相關資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

>[!IMPORTANT]
>
>當您刪除範本時，使用該範本的專案不會以任何方式修改。 不過，您不會再在專案的「範本」欄位中看到原始範本的名稱。 此外，您無法再在任務檢視中檢視專案上任務的範本任務名稱。 刪除最初與專案關聯的範本後，專案上的範本欄位和任務上的範本工作列位保持空白。

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
   <td> <p>編輯包含刪除許可權的範本存取權</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理範本的許可權，包括刪除範本的許可權</p></td> 
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 刪除範本的考量事項

* 當範本附加時新增到專案中的任務仍保留在專案上。 但是，與任務關聯的範本任務資訊會被刪除。
* 範本的名稱不再列在專案的&#x200B;**總覽**&#x200B;子索引標籤上的&#x200B;**範本**&#x200B;欄位中。

* 您可以從資源回收筒復原最近刪除的範本。 如需有關從資源回收筒復原專案的資訊，請參閱[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 刪除範本

{{step1-to-templates}}

這會開啟範本清單

1. 按一下範本名稱左邊的核取方塊，選取您要刪除的範本，然後按一下&#x200B;**刪除>是，刪除**&#x200B;以確認刪除。

   或

   按一下範本名稱以存取它，然後按一下&#x200B;**更多**&#x200B;功能表![更多圖示](assets/more-icon.png)，然後&#x200B;**刪除範本>是，刪除它**。

   範本無法再與專案建立關聯。
