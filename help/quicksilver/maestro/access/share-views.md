---
title: 共用檢視
description: 您可以在使用Adobe Workfront規劃功能時，與其他人共用檢視，以確保共同作業。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 023ca8c4e7c2dec2098390c1cda1e5b4eafbb840
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


<!--update the metadata and description when we turn this article live-->

# 共用檢視

{{maestro-important-intro}}

在Adobe Workfront規劃功能中使用記錄時，您可以與其他人共用檢視，以確保共同作業。

授予工作區許可權不會授予其他使用者記錄型別頁面上檢視的許可權。 您必須授予記錄型別頁面中個別檢視的許可權，才能與其他使用者共用檢視。

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
<p>貴組織必須註冊Adobe Workfront規劃功能封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> Adobe Workfront規劃功能沒有存取控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td> <p>管理檢視的許可權</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Maestro區域。 </p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/maestro/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 共用檢視的許可權

您可以共用您建立的檢視或您對其擁有管理許可權的檢視。

>[!NOTE]
>
>系統管理員無法檢視或共用他們未自行建立的檢視。 他們只能存取或共用與他們共用的檢視。

<!--for above note: System administrators can have only Manage permissions to a view.-->

{{step1-to-maestro}}

1. 開啟您要共用其檢視的工作區，然後按一下記錄型別卡片。

   這會開啟記錄型別頁面。

1. 從檢視下拉式功能表 <!--tab-->，將游標停留在您要共用的檢視上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) 檢視名稱右側，然後按一下 **共用**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. 在 **授予檢視存取許可權至** 欄位，開始輸入使用者或群組的名稱，然後在其顯示在清單中時按一下它。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 從下拉式功能表中選取下列其中一個許可權等級：
   * 檢視
   * 管理

     如需許可權層級以及使用者可針對每個層級執行的動作的相關資訊，請參閱 [在Adobe Maestro中共用許可權概觀](../access/sharing-permissions-overview.md).
1. 按一下 **複製連結** 將檢視的連結複製到剪貼簿。
1. 與他人共用複製的連結。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取記錄型別頁面並在選取的檢視中顯示該頁面。
1. 按一下「**儲存**」。
