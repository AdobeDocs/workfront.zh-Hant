---
title: 編輯記錄型別
description: 記錄型別儲存後，您可以編輯記錄型別。 記錄型別是Adobe Workfront計畫的物件型別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 編輯記錄型別

{{maestro-important-intro}}

記錄型別是Adobe Workfront計畫的物件型別。 您可以編輯您或其他人建立的記錄型別外觀。 如需建立Workfront計畫記錄型別的相關資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>若要將Adobe Workfront規劃記錄型別與Experience Manager Assets連線，您必須擁有Adobe Experience Manager Assets授權，並且貴組織的Workfront執行個體必須上線至Adobe商業平台或Adobe Admin Console。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊Adobe Workfront計畫封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Workfront計畫沒有存取層級控制項</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 編輯記錄型別

{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要編輯其記錄型別的工作區。
1. 將滑鼠停留在記錄型別的卡片上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄型別卡片的右上角，然後按一下 **更新外觀**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. 在 **更新記錄型別** 方塊中，更新下列資訊：

   * **記錄名稱**：視需要編輯記錄型別名稱。 <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **外觀**：編輯與記錄型別相關圖示的顏色和形狀。 執行下列動作：
      * 選取顏色以識別記錄型別。 這是記錄型別圖示的顏色。 預設會選取「灰色」。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。

     ![](assets/update-record-type-box.png)

1. 按一下 **更新記錄型別** 方塊以儲存您的變更。
1. （可選）從工作區區域按一下記錄型別卡以開啟記錄型別的頁面。
1. 按一下 **更多** 記錄型別名稱右邊的功能表，然後按一下 **重新命名** 重新命名記錄型別

   或

   重新命名標頭中的記錄型別。  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   您也可以重新命名記錄型別頁面標頭中的記錄型別。
1. （可選）展開記錄型別名稱右側的向下箭頭，並選取要編輯的其他記錄型別。
