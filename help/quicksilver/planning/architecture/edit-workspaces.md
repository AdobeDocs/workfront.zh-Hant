---
title: 編輯工作區
description: 您可以編輯現有工作區的資訊，例如重新命名。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 編輯工作區

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。

工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。

如需有關建立工作區的資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

您對工作區所做的所有變更，對至少擁有工作區檢視許可權的所有使用者都是可見的。

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
   <td> <p>Workfront Planning沒有存取層級控制</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您必須將Planning區域新增至版面配置範本。 如需詳細資訊，請參閱<a href="/help/quicksilver/planning/access/access-overview.md">存取總覽</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

如需存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯工作區

{{step1-to-planning}}

1. （視條件而定）如果您是Workfront管理員，請按一下&#x200B;**我的工作區**&#x200B;以存取您建立的工作區，或按一下&#x200B;**其他工作區**&#x200B;以存取其他人與您共用的工作區。<!--change it to Workspaces I'm on-->

1. 按一下工作區卡以開啟工作區。

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To edit a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **Edit**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,**********-->

1. 按一下新工作區標題中工作區的名稱以重新命名，然後按&#x200B;**Enter**。
1. 按一下標題中工作區名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**編輯**。

   ![](assets/edit-workspace-box.png)

   在&#x200B;**編輯工作區**&#x200B;方塊中更新下列資訊：

   * 新增工作區的名稱。<!--did they add a label for this field?-->
   * **描述**：新增工作區的相關資訊。
   * 選取要與工作區關聯的圖示。

1. 按一下&#x200B;**儲存**&#x200B;以關閉[編輯工作區]方塊並套用您的變更。

1. （可選）若要新增工作區區段，請執行下列任一項作業：

   * 按一下工作區底部的&#x200B;**新增區段**。
   * 將游標暫留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**新增上方區段**&#x200B;或&#x200B;**新增下方區段**。

1. （可選）若要變更區段位置，請執行下列任一項作業：

   * 暫留在區段名稱上，按一下&#x200B;**抓取**&#x200B;圖示![](assets/grab-icon.png)，然後將其拖放到右側位置。
   * 將游標暫留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**上移**&#x200B;或&#x200B;**下移**。 區段在工作區中向上或向下移動。

1. （可選）若要刪除工作區區段，請執行下列動作：

   1. 暫留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**刪除**。<!--add screen shot when UI is final?-->
   1. 選取新區段以將所有記錄型別移動至該區段，然後按一下&#x200B;**刪除**。<!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      所有記錄型別都會移至選取區段，而區段會被刪除。

1. （選擇性）按一下&#x200B;**新增記錄型別**&#x200B;以將記錄型別新增至工作區。

   如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

1. （選擇性）將滑鼠停留在記錄型別卡片上，按一下右上角的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以修改記錄型別的外觀。

   如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

1. （選擇性）將游標停留在記錄型別卡片上，按一下右上角的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**刪除**&#x200B;以刪除記錄型別。

   如需詳細資訊，請參閱[刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md)。

1. （可選）按一下記錄型別卡片以將其拖放到新位置。 您可以將記錄型別從一個工作區區段拖放至另一個工作區區段。

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （選擇性）按一下工作區右上角的&#x200B;**共用**，與他人共用工作區。

   如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。
