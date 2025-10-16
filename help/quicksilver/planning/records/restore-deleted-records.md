---
title: 還原已刪除的記錄
description: 您可以從Adobe Workfront Planning的「最近刪除」區域中復原已刪除的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 還原已刪除的記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

您可以從Adobe Workfront Planning的「最近刪除」區域中復原已刪除的記錄。

如需有關刪除記錄的資訊，請參閱[刪除記錄](/help/quicksilver/planning/records/delete-records.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p> <p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>貢獻或更高的許可權到工作區和記錄型別  </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr>   
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 復原已刪除記錄的相關考量事項

* 您可以還原已刪除您或其他使用者的記錄。
* 記錄會儲存在「最近刪除」的資料匣中30天。 30天後，記錄會從Workfront Planning中永久刪除。
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。 還原已刪除的記錄將會從連線的記錄中還原資訊。
* 您可以大量還原記錄。
* 刪除記錄時，會將下列資訊儲存在「最近刪除」的資料匣中：
   * **名稱**：這是記錄的[主要]欄位中的資訊。 如需有關記錄主要欄位的詳細資訊，請參閱[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   * **已刪除日期**：刪除記錄的時間和日期。
   * **最近刪除的時間**：刪除記錄後的時間。 在目前日期前30天以上被刪除的記錄不會顯示在「最近刪除」的資料匣中。
   * **由**&#x200B;刪除：刪除紀錄的使用者名稱。

## 還原已刪除的記錄

1. 移至您刪除記錄的記錄型別頁面。
1. 按一下任何記錄型別頁面檢視右上角的&#x200B;**復原**&#x200B;圖示![復原圖示](assets/undo-icon.png)，然後按一下&#x200B;**最近刪除**。

   顯示&#x200B;**最近刪除的**&#x200B;方塊。

   ![最近刪除的方塊](assets/recently-deleted-box.png)

1. 選取您要刪除的記錄，然後按一下&#x200B;**還原** > **還原**。 您可以選取多個記錄。

   如果還原成功，您會在畫面底部收到成功通知。
1. 移至表格檢視並檢閱還原的記錄。
