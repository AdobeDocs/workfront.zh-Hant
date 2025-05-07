---
title: 共用工作區
description: 您可以與其他人共用工作區，以確保在Adobe Workfront Planning中工作時，進行共同作業。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 3550d7addcc0bb790f15d141d9470e0b75f940a6
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 1%

---

# 共用工作區

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以與其他人共用工作區，以確保在Adobe Workfront Planning中工作時，進行共同作業。

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>授予工作區許可權不會授予其他使用者記錄型別頁面上檢視的許可權。 您必須授予記錄型別頁面中個別檢視的許可權，才能與其他使用者共用檢視。 如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。


## 存取需求

+++ 展開以檢視存取需求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p>
<p>您的組織必須加入Adobe Unified Experience，使用者才能透過許可權請求向工作區請求和授予許可權。 </p> 
<p>必須將使用者新增至Adobe Admin Console才能取得Workfront Planning工作區的許可權。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  <p>管理工作區的許可權</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>在「生產」環境中，所有使用者（包括系統管理員）都必須指派給包含Planning區域的版面配置範本。</p>
<p><span class="preview">在「預覽」環境中，「標準使用者」和「系統管理員」預設會啟用「規劃」區域。</span></p></td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於共用工作區的考量事項

* 如需在Workfront Planning中共用物件的一般資訊，另請參閱[在Adobe Workfront Planning中共用許可權概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
* 您可以與組織內的使用者、團隊、角色、群組或公司共用工作區。
* 除了團隊、群組、公司和職務角色之外，您只能與已新增至Adobe Admin Console的使用者共用。
* 您無法與組織外部的使用者共用工作區。
* 當您共用工作區時，也會共用與工作區相關聯的所有記錄型別、記錄和欄位。
* 當您共用工作區時，檢視不會共用。 您必須個別共用檢視。

<div class="preview">

* Workspace許可權在記錄型別上顯示為繼承許可權。

</div>

## 與工作區共用許可權

下列使用者可以與其他使用者共用工作區：

* 系統管理員可以共用所有工作區，包括他們未建立的工作區。
* 所有其他使用者只能共用他們對其具有管理許可權的工作區。

要與其他人共用工作區：

{{step1-to-planning}}

1. 開啟您要共用的工作區，然後按一下畫面右上角的&#x200B;**共用**。

   工作區右上方的![共用按鈕](assets/share-button-on-workspace-top-right.png)

1. 在&#x200B;**授與此工作區的存取權**&#x200B;欄位中，開始輸入使用者、群組、團隊、公司或工作角色的名稱，然後當它顯示在清單中時按一下它。

   ![與群組共用UI](assets/sharing-ui-with-groups.png)

1. 從下拉式功能表中選取下列其中一個許可權等級：
   * 檢視
   * 參與
   * 管理

     如需許可權層級，以及使用者可針對每個層級執行的動作的相關資訊，請參閱[在Adobe Workfront Planning中共用許可權的總覽](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
1. 按一下&#x200B;**複製連結**&#x200B;以將工作區的連結複製到剪貼簿。
1. 與他人共用複製的連結。 收到連結的使用者必須是作用中使用者，並登入Workfront才能存取工作區。
1. 按一下「**儲存**」。

## 透過許可權請求向工作區授予許可權

使用者若存取連結至沒有許可權的工作區，可以要求存取工作區的許可權。 所有具有工作區管理許可權的使用者都會收到許可權要求，並可授予或拒絕許可權。

1. （視條件而定）如果您是工作區的管理員，您可能會收到其他使用者存取下列區域檢視的請求：

   * 應用程式內通知
     ![存取要求的應用程式內通知](assets/in-app-notification-for-access-request.png)
   * 電子郵件通知
     ![存取要求的電子郵件通知](assets/email-notification-for-access-request.png)
1. （視條件而定）從Workfront的通知區域，按一下應用程式內通知
或
在電子郵件通知中，按一下**檢視所有通知**，然後按一下清單中的通知。

   顯示&#x200B;**擱置中的存取要求**&#x200B;方塊。

   ![通知清單核准方塊](assets/notifications-list-approval-box.png)

1. （選擇性）對於您要核准其許可權的使用者，從使用者名稱右側的下拉式功能表中選取下列選項之一：
   * **檢視**
   * **貢獻**
   * **管理**
1. 選取您要核准或拒絕許可權的使用者，然後按一下&#x200B;**全部核准**&#x200B;或&#x200B;**全部拒絕**。
1. 按一下&#x200B;**擱置存取要求**&#x200B;左側的向左箭頭，然後按一下&#x200B;**儲存**。

   如果您已核准請求，使用者會新增至工作區的共用方塊。 請求許可權的使用者會收到一封電子郵件，確認其請求已核准。<!--will they also get an in-app notification??-->


## 移除工作區的許可權


{{step1-to-planning}}

1. 開啟您要移除許可權的工作區，然後按一下畫面右上角的&#x200B;**共用**。
1. 按一下您共用工作區的實體名稱右側的下拉式功能表，然後按一下&#x200B;**移除**。
1. 按一下「**儲存**」。

   移除的使用者無法再存取工作區或其物件。
