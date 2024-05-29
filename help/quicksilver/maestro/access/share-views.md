---
title: 共用檢視
description: 您可以與其他人共用檢視，以確保在使用Adobe Workfront Planning時共同作業。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# 共用檢視

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中處理記錄時，與其他人共用檢視以確保共同作業。

授予工作區許可權不會授予其他使用者記錄型別頁面上檢視的許可權。 您必須授予記錄型別頁面中個別檢視的許可權，才能與其他使用者共用檢視。

當您共用檢視時，您會授予其他人存取檢視所有元素的許可權。 例如，當您將檢視的管理許可權授予他們時，他們可以修改分組、篩選、排序或長條圖外觀。

<!--
You can share a view with the following entities: 

* Workfront users
* Workfront groups
* Publicly, with users outside Workfront
-->

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
   <td> Adobe Workfront Planning沒有存取控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td> <p>管理檢視的許可權</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/maestro/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 共用檢視的許可權 <!--internally-->

您可以分享您建立的檢視或您擁有管理許可權的檢視 <!--with users or groups in Workfront-->.

>[!NOTE]
>
>系統管理員無法檢視或共用他們未自行建立的檢視。 他們只能存取或共用與他們共用的檢視。
>
>系統管理員只能擁有檢視的管理許可權。

{{step1-to-maestro}}

1. 開啟您要共用其檢視的工作區，然後按一下記錄型別卡片。

   這會開啟記錄型別頁面。

1. 在檢視標籤中，暫留在您要共用的檢視上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) 檢視名稱右側，然後按一下 **共用**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

<!--   
1. (Optional) Select from the following options to share the view: 

* **Only invited people can access**: You must specify users or groups that you want to share the view with. This is the default option.
* **Everyone in the workspace can view**: All users that have View or higher permissions to workspaces can access the view. -->


1. 在 **授予檢視存取許可權至** 欄位，開始輸入使用者或群組的名稱，然後在其顯示在清單中時按一下它。  <!--***********replace screen shot below when global sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 從下拉式功能表中選取下列其中一個許可權等級：
   * 檢視
   * 管理

     如需許可權層級以及使用者可針對每個層級執行的動作的相關資訊，請參閱 [在Adobe Workfront Planning中共用許可權的概觀](../access/sharing-permissions-overview.md).

     系統管理員一律會獲得與其共用檢視的管理許可權。

1. 按一下 **複製連結** 將檢視的連結複製到剪貼簿。
1. 與他人共用複製的連結。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取記錄型別頁面並在選取的檢視中顯示該頁面。
1. 按一下「**儲存**」。

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## 移除檢視的許可權

{{step1-to-maestro}}

1. 開啟您要停止共用其檢視的工作區，然後按一下記錄型別卡片。 這會開啟記錄型別頁面。
1. 將游標停留在您要移除共用之檢視的標簽名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **共用**.
1. 尋找您要移除的使用者或群組，然後按一下 **移除** 在使用者或群組名稱右側的「許可權」下拉式功能表中。
1. 按一下 **儲存**.
屬於已移除群組的使用者或使用者無法再存取該檢視。 對於已從存取檢視中移除的使用者，沒有通知他們已失去此存取權。

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->