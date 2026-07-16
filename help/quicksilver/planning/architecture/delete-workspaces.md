---
title: 刪除工作區
description: 當工作區不再相關時，您可以將其刪除。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yzpirNfY0Hsp0cbClQA8dFqhgqbpK8ZryIyeq4tBAgw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 2%

---

# 刪除工作區

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

您可以刪除不再相關的工作區。

建議您先在其他工作區中重新建立與您要刪除的工作區相關聯的部分或全部記錄型別、記錄、欄位和檢視，然後再刪除工作區。

## 存取權要求

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
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
或
<li><p>任何工作流程與任何Planning套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--
Old:

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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 有關刪除工作區的考量事項

* 當您刪除工作區時，也會刪除所有記錄型別、記錄、其欄位和檢視。
* 已刪除的工作區及其包含的資訊無法復原。

## 刪除工作區

{{step1-to-planning}}

1. （視條件而定）如果您是Workfront管理員，請按一下下列其中一項：

   * **我所在的工作區**&#x200B;存取您建立的工作區
   * **所有工作區**，以存取與您共用的工作區或您建立的工作區

   >[!NOTE]
   >
   >您無法刪除&#x200B;**範例工作區**&#x200B;索引標籤上的工作區。 我們建議使用多工作區範本套件來建立類似於「範例工作區」標籤上的工作區。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

1. （選擇性）按一下「**全部顯示**」以顯示其他工作區。 **顯示全部**&#x200B;連結只有在您有兩列以上的工作區卡片時才會顯示。
1. （選用） ClicK **顯示較少**&#x200B;以限制熒幕上顯示的工作區數目。
1. 若要刪除工作區，請執行下列任一項作業：

   * 將滑鼠停留在工作區卡片上，然後按一下卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)
或
   * 按一下[工作區]頁面右上角的&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)，依名稱搜尋工作區，然後按一下工作區卡片以開啟工作區，再按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)。

   >[!TIP]
   >
   >您可以使用下列鍵盤組合，從任何Workfront Planning頁面開啟全域搜尋方塊並搜尋工作區：
   >
   >* Windows版CTRL+K
   >* 適用於Mac的⌘+K

1. 按一下&#x200B;**刪除**。

   ![永久刪除工作區確認](assets/permanently-delete-workspace-confirmation.png)

1. 在提供的空白處輸入&#39;&#39;**&#39;delete**&#39;&#39;，然後按一下&#x200B;**&#39;永久刪除**。 不區分大小寫。

   工作區已刪除且無法復原。 任何與其關聯的記錄型別、記錄、欄位和檢視也會被刪除。<!--ensure this is right at or before GA-->


