---
title: 管理行事曆檢視
description: 您可以在行事曆檢視中顯示記錄及其欄位。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
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

有關Maestro檢視以及如何管理檢視的資訊，請參閱 [管理記錄檢視](../views/manage-record-views.md).

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
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td role="rowheader">存取層級設定</td>
   <td> <p>Maestro沒有存取層級控制項 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理檢視的許可權</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 管理行事曆檢視 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

請考量下列事項：

* 只有當您至少有兩個日期欄位與記錄型別相關聯時，才能建立「行事曆」檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，「行事曆」檢視選項會變暗。
* 下列情境：

   * 當「開始」與「結束」日期沒有值時，記錄不會顯示在行事曆上
   * 當「開始」或「結束」日期沒有值時，記錄會顯示為單日事件
   * 當開始日期在結束日期之後時，記錄不會顯示在行事曆上。

若要管理行事曆檢視：

1. 移至您要檢視其行事曆的記錄型別頁面。
1. 建立行事曆檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   與您選取的記錄型別相關聯的記錄會在行事曆中顯示為長條。

1. 執行下列任一項作業來瀏覽行事曆：

   * 按一下左右圖示，或使用水準捲動在行事曆中前後移動。
   * 按一下 **今天** 將行事曆置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * 月