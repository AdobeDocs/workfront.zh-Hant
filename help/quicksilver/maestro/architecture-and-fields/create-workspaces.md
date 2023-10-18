---
title: 建立工作區
description: 工作區是團隊使用的操作記錄型別和分類法的集合，代表團隊的工作生命週期。 您可以在Maestro中完全自訂工作區。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 建立工作區

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

在Adobe大師，工作區是團隊計畫工作的集中位置。

工作區是團隊使用的操作記錄型別和分類法的集合，代表團隊的工作生命週期。 您可以在Maestro中完全自訂工作區。

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

## 關於工作區的考量事項

* 您可以為組織內的特定組織單位建立工作區，以符合每個單位的獨特運作方式。
* 工作區包含的記錄型別和分類應反映組織單位的工作生命週期。
* 建立工作區時，組織中的所有人都可以檢視、編輯或刪除工作區。  <!--this will change with access levels and permissions-->
* 貴組織中最多可以有1,000個工作區。
* 工作區包含每個工作區唯一的記錄型別。 <!--this might change-->

## 建立工作區

1. （視條件而定）如果系統中沒有任何工作區，請按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然後按一下 **大師** ![](assets/maestro-icon.png).

   或者，從現有工作區中，按一下工作區名稱右側的向下指向，然後按一下 **建立工作區**.

   ![](assets/workspace-drop-down-right-menu.png)

   這會開啟Maestro的「工作區」區域。
1. （選擇性和條件性）按一下 **預覽** 在下列任何預先定義的工作區範本內：

   * 行銷管理
   * 銷售管理
   * 產品管理

   系統會指出哪些作業記錄型別、分類法以及與每個範本相關聯的欄位數。

   ![](assets/previewing-a-workspace-template.png)

   如需Maestro工作區範本的相關資訊，請參閱 [工作區範本清單](../architecture-and-fields/workspace-templates.md).

1. 按一下 **使用範本** 以從選取的範本開始建立工作區

   或

   按一下 **建立工作區** 從頭開始建立工作區。

   會建立下列其中一種工作區型別：

   * 空的工作區，您可以在此處開始手動新增記錄型別。
   * 以範例記錄型別填入的工作區，您可以進一步自訂。

1. 在新工作區標題的工作區名稱內按一下以重新命名，然後按Enter鍵

   或

   按一下 **更多** 功能表 ![](assets/more-menu.png)工作區名稱右側，然後按一下 **重新命名**.

1. （選用）按一下 **新增記錄型別** 以新增記錄型別至工作區。

   如需詳細資訊，請參閱 [建立記錄型別](../architecture-and-fields/create-record-types.md).

1. （選用）按一下 **新增分類法** 將分類新增至工作區。

   如需詳細資訊，請參閱 [建立分類](../architecture-and-fields/create-a-taxonomy.md).
