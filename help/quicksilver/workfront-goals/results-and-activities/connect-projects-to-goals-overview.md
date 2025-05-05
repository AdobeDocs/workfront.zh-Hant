---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 在Adobe Workfront目標中新增專案
description: 您可以將專案連結到目標，以根據專案的實際進度指出目標進度。 專案會成為目標的進度指示器。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---

# 在Adobe Workfront目標中新增專案

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

您可以將專案連結到目標，以根據專案的實際進度指出目標進度。 專案會成為目標的進度指示器。

藉由將專案連線至目標，您可以將組織的策略計畫（目標）與人員每天執行和完成的實際工作（專案）聯絡起來。

>[!IMPORTANT]
>
>在專案的業務案例區域中建立的專案層級目標未連結到Workfront目標中建立的策略目標。 如需業務案例專案目標的相關資訊，請參閱[建立業務案例目標](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。


## 存取需求

您必須具備下列條件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>Ultimate計畫 </li></ul>
   </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求，下列其中一項： </p>
<ul>
<li>Select或Prime Adobe Workfront計畫以及額外的Adobe Workfront目標授權。</li>
<li>Ultimate Workfront計畫，預設包含Workfront目標。 </li></ul>
 <p>或</p>
 <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 將專案連線至目標的相關考量事項

* 您可以將符合下列條件的專案新增至目標：

   * 您至少必須擁有檢視許可權。

     >[!NOTE]
     >
     >如果您在將專案附加到目標後失去檢視專案的許可權，您仍可以看到目標的專案資訊，但您無法再存取專案。

   * 專案不得處於廢棄狀態。

* 您可以將多個專案與一個目標建立關聯。
* 您可以將相同專案與多個目標建立關聯。
* 您無法從附加專案的目標手動更新專案進度。 Workfront會改為計算專案的完成百分比，而Workfront目標會使用此完成百分比來計算目標進度。 這會在專案百分比更新後即時更新目標。
* 專案持續時間可在目標的時段之外。 如果專案持續的時間超過目標的截止日期，您仍可關閉目標並視為已完成，但目標完成百分比不會是100%。 專案的完成百分比不再更新目標。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 當您刪除附加到目標的專案時，該專案也會從目標中刪除。

  >[!CAUTION]
  >
  >如果在您刪除專案之前目標為作用中，且目標上沒有其他進度指標，則目標會變為非作用中。


## 將專案新增至目標

1. 按一下&#x200B;**主功能表** ![主功能表圖示](assets/main-menu-icon.png) (為Shell繪製此專案：或按一下左上角的&#x200B;**主功能表** ![主功能表行](assets/three-line-main-menu-icon.png) （如果有的話）。)，然後&#x200B;**目標**。
1. 從目標清單中，按一下目標的名稱以開啟目標頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 從&#x200B;**新進度指示器**&#x200B;下拉式功能表，按一下&#x200B;**新增現有專案**。

   「將專案新增至目標」方塊隨即顯示。
1. （選擇性）按一下清單右上角的個別圖示，以修改專案清單的顯示方式，更新&#x200B;**檢視**、**篩選器**&#x200B;或&#x200B;**群組**。
1. （選擇性）按一下&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)，然後開始輸入專案名稱以在清單中快速找到它。
1. 選取您要新增至目標的專案，然後按一下[新增]。**&#x200B;**

   選取的專案會新增至目標，並顯示在&#x200B;**專案**&#x200B;群組下的目標頁面進度指標區段。

   啟動目標後，當專案進度更新時，目標的進度會自動更新。 如需啟用目標的相關資訊，請參閱[在Adobe Workfront目標中啟用目標](../goal-management/activate-goals.md)。

## 找到目標的專案資訊

<p>
目標頁面的進度指標區段中的目標層級會顯示下列專案資訊：

</p>

<table>
  <tr>
   <td>專案名稱
   </td>
   <td>專案名稱的任何變更也會反映在連線的專案中。
   </td>
  </tr>
  <tr>
   <td>專案所有者
   </td>
   <td>專案所有者的任何變更也會反映在連線的專案中。
   </td>
  </tr>
    <tr>
   <td>實際進度
   </td>
   <td> <p>專案的完成百分比。 您無法從目標手動更新專案完成百分比。 Workfront會根據任務的完成百分比自動計算此值。 </p>
   </td>
  </tr>
  <tr>
   <td>進度
   </td>
   <td>橫條圖示的專案完成百分比。 除非目標關閉，否則專案完成百分比的任何變更都會自動更新目標進度。
   </td>
  </tr>

</table>

## 尋找專案的目標資訊

下列目標資訊會顯示在專案清單或報表中：

| 目標資訊 | 說明 |
|---|---|
| 目標 | 所有具有相關聯專案的目標清單。 |
| 目標階層 | 目標所屬的階層。 只有目標和目標的父級會顯示在此欄位中。 子目標不顯示。 |
| 連結的目標數 | 連結至一個專案的目標數。 |
