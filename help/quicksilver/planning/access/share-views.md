---
title: 共用檢視
description: 您可以與其他人共用檢視，以確保在使用Adobe Workfront Planning時共同作業。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 1%

---



# 共用檢視

{{planning-important-intro}}

您可以在Adobe Workfront Planning中處理記錄時，與其他人共用檢視以確保共同作業。

>[!IMPORTANT]
>
>* 授予工作區許可權不會授予其他使用者記錄型別頁面上檢視的許可權。 您必須授予記錄型別頁面中個別檢視的許可權，才能與其他使用者共用檢視。
>
>* 授予檢視的許可權不會變更檢視記錄的許可權。 記錄許可權是透過共用工作區所授與。
>
>* 當您共用檢視時，您會授予其他人存取檢視所有元素的許可權。 例如，當您將檢視的管理許可權授予他們時，他們可以修改分組、篩選、排序或長條圖外觀。


您可以與下列實體共用檢視：

* 內部，具有Workfront使用者和群組
* 公開，與Workfront以外的使用者一起

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

您必須具備下列專案才能存取Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront Planning計畫包含哪些專案的詳細資訊，請參閱<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定價與封裝</a>。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準</p>
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
   <td>  <p>管理檢視的許可權</p>  
   <p>只有具有工作區管理許可權的使用者才能公開共用檢視。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

+++

## 共用檢視時的注意事項

* 您可以將檢視或管理許可權授予內部Workfront使用者。

* 具有管理許可權的使用者可以修改檢視設定、共用、複製或刪除它。

* 您可以透過公開連結與組織外部的人員共用檢視。

* 當您公開共用檢視時，公司以外的任何人只要在到期日所指示的限定時間內都可以存取連結。 不需要登入即可檢視共用檢視。

* 您組織外有權存取檢視的人員無法在檢視中建立其他檢視、編輯共用檢視，或新增、刪除或編輯記錄資訊。

## 與內部檢視共用許可權

您可以將建立的檢視或您擁有管理許可權的檢視與Workfront中的使用者或群組共用。

>[!NOTE]
>
>系統管理員無法檢視或共用他們未自行建立的檢視。 他們只能存取或共用與他們共用的檢視。
>
>系統管理員只能擁有檢視的管理許可權。

{{step1-to-planning}}

1. 開啟您要共用其檢視的工作區，然後按一下記錄型別卡片。

   這會開啟記錄型別頁面。

1. 在[檢視]索引標籤中，暫留在您要共用的檢視上，然後按一下檢視名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**共用**。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   依預設，應該選取&#x200B;**內部共用**&#x200B;標籤。

1. （選擇性）在&#x200B;**擁有存取權**&#x200B;區域中，從下列選項中選取：

   * **只有受邀者才能存取**：您必須指定想要與其共用檢視的使用者或群組。 這是預設選項。
   * **工作區中的所有人都可以檢視**：所有對工作區具有「檢視」或更高許可權的使用者都可以存取檢視。

1. 在&#x200B;**授與檢視許可權給**&#x200B;欄位中，開始輸入使用者或群組的名稱，然後當它顯示在清單中時按一下它。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 從下拉式功能表中選取下列其中一個許可權等級：
   * 檢視
   * 管理

     如需許可權層級，以及使用者可針對每個層級執行的動作的相關資訊，請參閱[在Adobe Workfront Planning中共用許可權的總覽](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

     系統管理員一律會獲得與其共用檢視的管理許可權。

1. 按一下&#x200B;**複製連結**&#x200B;以將檢視的連結複製到剪貼簿。
1. 按一下「**儲存**」。

   檢視會以人員圖示![](assets/view-shared-with-others-people-icon.png)更新，表示檢視現在已與其他使用者共用。

   >[!TIP]
   >
   沒有人員或全域圖示的檢視是您建立的檢視，不會與他人共用。 非共用檢視僅對您可見。

1. 與他人共用複製的連結。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取記錄型別頁面並在選取的檢視中顯示該頁面。

## 共用許可權以公開檢視

您可以將建立的檢視或您擁有管理許可權的檢視共用給沒有Workfront授權以及可能屬於您組織外部的人員。

>[!IMPORTANT]
>
只有具有工作區管理許可權的使用者才能公開共用工作區的檢視。


若要在Workfront Planning中公開共用檢視：

{{step1-to-planning}}

1. 開啟您要共用其檢視的工作區，然後按一下記錄型別卡片。

   這會開啟記錄型別頁面。

1. 在[檢視]索引標籤中，暫留在您要共用的檢視上，然後按一下檢視名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**共用**。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. 按一下&#x200B;**公用共用**。

   ![](assets/public-sharing-tab-for-views.png)

1. 啟用&#x200B;**建立公用連結**&#x200B;設定。

   連結隨即變為可用。 此為公開連結。 共用時，擁有連結的任何人，包括組織外部的人員，都可以存取記錄型別頁面，並檢視頁面上的記錄和欄位。

1. 按一下&#x200B;**複製連結**&#x200B;圖示![](assets/copy-link-view.png)以將連結複製到剪貼簿。

1. 手動輸入日期，或使用&#x200B;**連結到期日**&#x200B;欄位中的行事曆來選取公開連結的到期日。 在選取的日期之後將無法存取記錄頁面檢視。

1. 按一下「**儲存**」。

   檢視會以全域圖示![](assets/public-shared-view-icon-highlighted.png)更新，表示檢視已公開共用。

   >[!TIP]
   >
   >沒有人員或全域圖示的檢視是您建立的檢視，不會與他人共用。 非共用檢視僅對您可見。


1. （可選）將您複製的連結貼到電子郵件、聊天訊息、檔案，或貼到Workfront註解中，以便與其他人共用。

## 移除檢視的許可權

{{step1-to-planning}}

1. 開啟您要停止共用其檢視的工作區，然後按一下記錄型別卡片。 這會開啟記錄型別頁面。
1. 將游標停留在您要移除共用之檢視的索引標簽名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**共用**。
1. 若要移除檢視的內部共用，請執行下列動作：

   1. 請確定已選取&#x200B;**內部共用**&#x200B;標籤。
   1. 尋找您要移除的使用者或群組，展開使用者或群組名稱右側的許可權下拉式功能表，然後按一下&#x200B;**移除**。

1. 若要移除檢視的公開共用，請執行下列動作：

   1. 按一下「**公用共用**」標籤。
   1. 取消選取&#x200B;**建立公開連結**&#x200B;選項。

1. 按一下「**儲存**」。

   人員無法再存取檢視。 對於已從存取檢視中移除的使用者，不會通知他們不再擁有此存取權。
