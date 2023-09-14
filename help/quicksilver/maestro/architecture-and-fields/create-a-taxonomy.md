---
title: 建立分類記錄型別
description: 分類是可重複使用的記錄型別，可擷取Adobe Workfront Maestro中作業記錄型別的相關屬性。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 建立分類記錄型別

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

分類法是擷取AdobeMaestro中作業記錄型別相關屬性的記錄型別。

例如，Campaign可以是作業記錄型別。 以下是擷取促銷活動記錄型別相關屬性的分類：地區、對象、國家。

如需有關Maestro記錄型別的詳細資訊，請參閱 [記錄型別和分類概觀](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## 建立分類的相關考量事項

* 您必須先建立工作區，才能在工作區中建立分類。

  如需有關工作區的資訊，請參閱 [建立工作區](../architecture-and-fields/create-workspaces.md).
* 您可以執行下列任一項作業來建立分類記錄型別：
   * 使用範本建立工作區時自動建立它們。 如需詳細資訊，請參閱 [建立工作區](../architecture-and-fields/create-workspaces.md).
   * 從頭開始手動建立。
   * 從外部清單貼上資訊，以手動方式建立它們。

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* 所有新建立的分類都隨附下列欄位：

   * 名稱 <!--if there won't be any more fields, consider rephrasing this-->

  此外，您可以將自訂欄位新增到分類法。 如需詳細資訊，請參閱 [建立欄位](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    使用工作區範本時建立的分類有其他欄位。

## 建立分類法

建立分類類似於從頭開始或從工作區範本建立作業記錄型別。

如需詳細資訊，請參閱文章中的「從頭開始建立記錄型別」一節 [建立記錄型別](../architecture-and-fields/create-record-types.md).

如需從範本建立工作區時自動建立分類的相關資訊，請參閱 [建立工作區](../architecture-and-fields/create-workspaces.md).
