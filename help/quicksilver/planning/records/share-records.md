---
title: 共用記錄
description: 您可以與其他人共用記錄以增加共同作業。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# 共用記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<!--take out preview and production references at release-->

{{planning-important-intro}}

若要與其他使用者共同作業，您可以與其他使用者共用記錄。

您可以透過下列方式共用Adobe Workfront Planning記錄：

* 當頁面開啟時，從瀏覽器複製記錄頁面的連結。

* 在記錄型別的表格檢視中檢視記錄時，複製指向記錄頁面的連結。

* 您可以共用工作區<!--<span class="preview">and record type</span>--> ，以與其他使用者共用工作區中的所有記錄。 如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。

<!-- replace the last sentence above with this: 

For more information see the following articles:

* [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)


<div class="preview">

* [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

</div>

-->

本文說明如何從記錄型別的表格檢視複製記錄頁面的連結。

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
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 投稿人、輕度或標準 </p>
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
   <td>  <p>使用連結檢視或更高的工作區許可權以共用<!--<span class="preview">and record type</span>-->記錄 </p>
   <p>管理工作區<!--<span class="preview">and record type</span>-->的許可權以共用工作區中的記錄 </p>
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

-->

## 從記錄型別表格檢視共用記錄連結

{{step1-to-planning}}

您上次存取的工作區會開啟。
1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從表格右上角的&#x200B;**檢視**&#x200B;下拉式功能表中，選取表格檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 以滑鼠右鍵按一下記錄列

   或

   將游標停留在記錄名稱上，按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**複製連結**。

   ![](assets/contextual-menu-for-record-row.png)

   連結已複製到您的剪貼簿。

1. 將連結貼到電子郵件或聊天視窗中，以便與其他使用者共用。 使用者收到連結時，會開啟記錄頁面。

   >[!TIP]
   >
   >記錄頁面中的欄位與記錄的「表格」檢視中可用的欄位相同。


   <!--add there when it will be available: if they have access to this record-->

## 透過共用工作區來共用工作區中的所有記錄

當您與其他人共用工作區時，可以共用工作區中的所有記錄。

只有具有工作區管理許可權的使用者才能與其他人共用。

如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。


<!--
<div class="preview">

## Share all records in a record type by sharing the record type

In the Production environment, records inherit permissions from the workspace. 

In the Preview environment, records inherit permissions from the record type. 

By default, record types inherit permissions from the workspace. 

However, you can do any of the following:

* Turn off inherited permissions from the workspace on a record type. This removes permissions from the records. 
* Manually grant permissions to users to a record type, even when they have no permissions to the workspace. This automatically gives them View permissions to the workspace. This grants permissions to users to the records. 

Only users with Manage permissions to a workspace can share its record types and records with others. 

For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>

-->