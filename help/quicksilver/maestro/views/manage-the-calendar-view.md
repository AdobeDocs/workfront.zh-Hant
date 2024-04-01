---
title: 管理行事曆檢視
description: 您可以在行事曆檢視中顯示記錄及其欄位。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 7fe24704cead460762322b4f26bf37431e9744ca
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# 管理行事曆檢視

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

您可以從記錄型別頁面，在行事曆檢視中顯示記錄及其欄位。

如需Adobe Workfront Planning功能檢視及管理檢視方式的詳細資訊，請參閱 [管理記錄檢視](../views/manage-record-views.md).

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
<p>貴組織必須註冊Adobe Workfront Planning測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <p>系統管理員只能存取他們建立或與他們共用的檢視。 </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級設定</td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理檢視的許可權</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 管理行事曆檢視 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

請考量下列事項：

* 只有當您至少有兩個日期欄位與記錄型別相關聯時，才能建立「行事曆」檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，「行事曆」檢視選項會變暗。
* 存在下列情況：

   * 當「開始」與「結束」日期都沒有值時，記錄不會顯示在行事曆上
   * 當「開始」或「結束」日期沒有值時，記錄會顯示為單日事件
   * 當開始日期晚於結束日期時，記錄不會顯示在行事曆上。

若要管理行事曆檢視：

1. 移至您要檢視其行事曆的記錄型別頁面。
1. 建立行事曆檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   與您選取的記錄型別相關聯的記錄會在行事曆中顯示為長條。 長條的顏色與記錄圖示的顏色相符。

1. 執行下列任一項作業來瀏覽行事曆：

   * 按一下左右圖示，或使用水準捲動在行事曆中前後移動。
   * 按一下 **今天** 將行事曆置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * 月
1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
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

  如需詳細資訊，請參閱文章中的「新增篩選器」一節 [管理表格檢視](/help/quicksilver/maestro/views/manage-the-table-view.md).

* 您可以依已連線的記錄欄位或查詢欄位進行篩選，但不能針對允許連結至多個記錄的欄位進行篩選。
