---
title: 編輯記錄型別
description: 記錄型別儲存後，您可以編輯記錄型別。 記錄型別是Adobe大師(Maestro)的物件型別。
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 編輯記錄型別

>[!IMPORTANT]
>
>目前，Adobe大師是封閉式測試計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

記錄型別是Adobe大師(Maestro)的物件型別。 您可以編輯您或其他人建立的記錄型別外觀。 如需有關建立Maestro記錄型別的資訊，請參閱 [建立記錄型別](../architecture-and-fields/create-record-types.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 編輯記錄型別

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然後按一下 **大師** ![](assets/maestro-icon.png).

   根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要建立記錄型別的工作區。
1. 將滑鼠停留在記錄型別的卡片上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄型別卡片的右上角，然後按一下 **更新外觀**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. 在「更新記錄型別」方塊中，更新下列資訊：

   * **記錄名稱**：視需要編輯記錄型別名稱。 <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **外觀**：編輯與記錄型別相關圖示的顏色和形狀。 執行下列動作：
      * 選取顏色以識別記錄型別。 這是記錄型別圖示的顏色。 預設會選取「灰色」。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。

     ![](assets/update-record-type-box.png)

1. 按一下「更新記錄型別」方塊外部以儲存變更。
1. （可選）從工作區區域按一下記錄型別卡以開啟記錄型別的頁面。
1. 按一下 **更多** 記錄型別名稱右邊的功能表，然後按一下 **重新命名** 重新命名記錄型別

   或

   重新命名標頭中的記錄型別。  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   您也可以重新命名記錄型別頁面標頭中的記錄型別。

