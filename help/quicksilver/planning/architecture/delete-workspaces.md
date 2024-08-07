---
title: 刪除工作區
description: 當工作區不再相關時，您可以將其刪除。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 刪除工作區

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

您可以刪除不再相關的工作區。

建議您先在其他工作區中重新建立與您要刪除的工作區相關聯的部分或全部記錄型別、記錄、欄位和檢視，然後再刪除工作區。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>您的組織必須處於Workfront Planning的早期存取階段中註冊 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>新增：標準</p>
   <p>目前：計畫</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱<a href="/help/quicksilver/planning/access/access-overview.md">存取總覽</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*如需存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 有關刪除工作區的考量事項

* 當您刪除工作區時，也會刪除所有記錄型別、記錄、其欄位和檢視。
* 已刪除的工作區及其包含的資訊無法復原。

## 刪除工作區

{{step1-to-planning}}

1. （視條件而定）如果您是Workfront管理員，請按一下&#x200B;**我的工作區**&#x200B;以存取您建立的工作區，或按一下&#x200B;**其他工作區**&#x200B;以存取其他人與您共用的工作區。<!--change it to Workspaces I'm on-->

1. 按一下要刪除之工作區的卡片。

   工作區頁面隨即顯示。

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To delete a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **De,ete**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,******to the step below****-->

1. 按一下工作區名稱旁的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**刪除**。

   ![](assets/permanently-delete-workspace-confirmation.png)

1. 在提供的空白處輸入&#39;&#39;**&#39;delete**&#39;&#39;，然後按一下&#x200B;**&#39;永久刪除**。 不區分大小寫。

   工作區已刪除且無法復原。 任何與其關聯的記錄型別、記錄、欄位和檢視也會被刪除。<!--ensure this is right at or before GA-->
