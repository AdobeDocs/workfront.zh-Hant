---
title: 建立分類記錄型別
description: 使用範本建立工作區時，會在「作業記錄型別」與「分類」區段中建立記錄型別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 建立分類記錄型別

{{planning-important-intro}}

使用範本建立工作區時，會在下列區段中建立記錄型別：

* 運作記錄類型
* 分類法

工作區之「分類」區段中的記錄型別，會擷取相同工作區之「作業記錄型別」區段中有關記錄型別的屬性。

例如，Campaign可以是作業記錄型別。 以下是擷取促銷活動記錄型別相關屬性的分類：地區、對象、國家。

如需有關記錄型別的詳細資訊，請參閱 [記錄型別概觀](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>若要將記錄型別與Experience Manager Assets連線，您必須擁有Adobe Experience Manager Assets授權，並且貴組織的Workfront執行個體必須上線至Adobe Business Platform或Adobe Admin Console。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊Adobe Workfront Planning封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區
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

* 您必須使用範本建立工作區，才能在工作區的「分類」區段中建立記錄型別。

  如需有關工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).
* 您可以執行下列其中一項作業，在工作區的「分類」區段中建立記錄型別：
   * 使用範本建立工作區時自動建立它們。 如需詳細資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).
   * 在工作區的「分類」區段中，從頭開始手動建立分類。

* 依預設，所有新建立的分類有下列欄位：

   * 姓名
   * 說明
   * 開始日期
   * 結束日期
   * 狀態

  此外，您可以將自訂欄位新增到分類法。 如需詳細資訊，請參閱 [建立欄位](../fields/create-fields.md).

  >[!NOTE]
  >
  >    使用工作區範本時建立的分類記錄型別還有其他欄位。

## 建立分類記錄型別

建立分類記錄型別與建立記錄型別類似。

如需詳細資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).
