---
title: 編輯工作區
description: 您可以編輯現有工作區的資訊，例如重新命名。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 編輯工作區

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。

工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。

如需有關建立工作區的資訊，請參閱 [建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md).

您對工作區所做的所有變更，對至少擁有工作區檢視許可權的所有使用者都是可見的。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>您必須將Planning區域新增至版面配置範本。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 編輯工作區

{{step1-to-planning}}

1. 在新工作區標題的工作區名稱內按一下以重新命名，然後按下 **輸入**.
1. 按一下 **更多** 功能表 ![](assets/more-menu.png)工作區名稱右側，然後按一下 **編輯**.

   ![](assets/edit-workspace-box.png)

   更新以下資訊於 **編輯工作區** 方塊：

   * 新增工作區的名稱。 <!--did they add a label for this field?-->
   * **說明**：新增工作區的相關資訊。
   * 選取要與工作區關聯的圖示。

1. 按一下 **儲存** 以關閉「編輯工作區」方塊並套用您的變更。

1. （可選）若要新增工作區區段，請執行下列任一項作業：

   * 按一下 **新增區段** 位於工作區底部。
   * 將游標停留在區段名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **新增上述區段** 或 **在底下新增區段**.

1. （可選）若要變更區段位置，請執行下列任一項作業：

   * 將游標停留在區段名稱上，然後按一下 **抓取** 圖示 ![](assets/grab-icon.png)，然後將其拖放至正確的位置。
   * 將游標停留在區段名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **上移** 或 **下移**. 區段在工作區中向上或向下移動。

1. （可選）若要刪除工作區區段，請執行下列動作：

   1. 暫留在區段名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **刪除**. <!--add screen shot when UI is final?-->
   1. 選取新區段以將所有記錄型別移動至該區段，然後按一下 **刪除**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      所有記錄型別都會移至選取區段，而區段會被刪除。

1. （選用）按一下 **新增記錄型別** 以新增記錄型別至工作區。

   如需詳細資訊，請參閱 [建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md).

1. （可選）將滑鼠游標停留在記錄型別卡片上，按一下 **更多** 功能表 ![](assets/more-menu.png) 按一下「 」 **編輯** 修改記錄型別的外觀。

   如需詳細資訊，請參閱 [編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md).

1. （可選）將滑鼠游標停留在記錄型別卡片上，按一下 **更多** 功能表 ![](assets/more-menu.png) 按一下「 」 **刪除** 刪除記錄型別。

   如需詳細資訊，請參閱 [刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md))。

1. （可選）按一下記錄型別卡片以將其拖放到新位置。 您可以將記錄型別從一個工作區區段拖放至另一個工作區區段。

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （選用）按一下 **共用** 工作區右上角的「 」，與其他人共用工作區。

   如需詳細資訊，請參閱 [共用工作區](/help/quicksilver/planning/access/share-workspaces.md).
