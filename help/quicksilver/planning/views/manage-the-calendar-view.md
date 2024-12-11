---
title: 管理行事曆檢視
description: 您可以在行事曆檢視中顯示記錄及其欄位。 本文說明如何建立行事曆檢視，以及如何編輯或刪除現有檢視。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# 管理行事曆檢視

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以從記錄型別頁面，在行事曆檢視中顯示記錄及其欄位。

如需Adobe Workfront Planning檢視的詳細資訊及管理方式，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

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
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
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
   <td>   <p>管理檢視的許可權</p>  
   <p>檢視許可權以暫時變更檢視設定</p> </td> 
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
   <p>View permissions to a view to temporarily change the view settings</p>
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

## 管理行事曆檢視 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

請考量下列事項：

* 只有當您至少有兩個日期欄位與記錄型別相關聯時，才能建立「行事曆」檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，「行事曆」檢視選項會變暗。

  您可以從記錄日期欄位中選取，或從連線的記錄或物件型別中查詢日期欄位。
* 存在下列情況：

   * 當「開始」與「結束」日期都沒有值時，記錄不會顯示在行事曆上
   * 當「開始」或「結束」日期沒有值時，記錄會顯示為單日事件
   * 當開始日期晚於結束日期時，記錄不會顯示在行事曆上。

若要管理行事曆檢視：

1. 移至您要檢視其行事曆的記錄型別頁面。
1. 建立行事曆檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。

   ![](assets/calendar-view-example.png)

   與您選取的記錄型別相關聯的記錄會在行事曆中顯示為長條。 長條的顏色與記錄圖示的顏色相符。

1. 執行下列任一項作業來瀏覽行事曆：

   * 按一下左右圖示，或使用水準捲動在行事曆中前後移動。
   * 按一下&#x200B;**今天**，將行事曆置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * **月**：記錄會顯示在每月行事曆中。

     <div class="preview">

      * **周**：記錄會顯示在下列區域中：

         * 橫跨多天的記錄會顯示在行事曆的頂端。
         * 持續一天或更短的記錄，會顯示在行事曆檢視的下半部分。 如果您選取顯示開始與結束日期的小時，則記錄會在記錄發生的當天的適當時間顯示。
     </div>

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * [設定](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### 新增篩選器

您可以使用篩選器來減少熒幕上顯示的資訊量。

在行事曆檢視中使用篩選器時，請考慮下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為行事曆檢視建立的篩選器與套用至相同記錄型別之任何其他檢視中的篩選器分開運作。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個行事曆檢視可以套用不同的篩選器。

* 檢視相同行事曆檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法命名您為行事曆檢視建立的篩選器。

* 移除篩選器會將篩選器從存取與您相同記錄型別以及顯示與您相同檢視的任何人移除。

* 在行事曆檢視中新增篩選器，與在表格檢視中新增篩選器相同。

  如需詳細資訊，請參閱文章[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)中的「新增篩選器」一節。

* 您可以依已連線的記錄欄位或查詢欄位進行篩選。

* 您可以依顯示多個值的查閱欄位進行篩選。

### 編輯行事曆檢視設定

編輯行事曆檢視設定與編輯時間軸檢視的設定類似。

如需詳細資訊，請參閱文章[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)中的「編輯時間表檢視設定」一節。
