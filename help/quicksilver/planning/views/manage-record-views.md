---
title: 管理記錄檢視
description: 使用Adobe Workfront Planning時，您可以在表格、時間軸或行事曆檢視中顯示記錄。 本文說明如何建立檢視及編輯現有檢視。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 1%

---


# 管理記錄檢視

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

在Adobe Workfront Planning區域中選取記錄型別後，您可以在下列檢視中顯示該型別的所有記錄：

* 表格

  如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

* 時間軸

  如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

* 行事曆

  如需詳細資訊，請參閱[管理行事曆檢視](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

本文說明有關記錄檢視的下列資訊：

* [建立及編輯檢視](#create-or-edit-record-views)
* [在檢視中啟用即時狀態指示器](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

如需有關管理Workfront Planning記錄檢視的詳細資訊，另請參閱下列文章：

* [刪除記錄檢視](/help/quicksilver/planning/views/delete-record-views.md)
* [複製記錄檢視](/help/quicksilver/planning/views/duplicate-record-views.md)
* [共用檢視](/help/quicksilver/planning/access/share-views.md)


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
<p>任何Workfront和任何Planning套件</p>
<p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 建立和刪除檢視的標準</p>
   <p>更新檢視元素的投稿人或更新者</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理檢視的許可權</p>  
   <p>檢視許可權以暫時變更檢視設定或複製檢視</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
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
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
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
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## 使用記錄檢視時的注意事項

* Workfront Planning中的檢視是記錄型別專屬檢視。 您不能將相同的檢視套用至兩種不同的記錄型別。
* 您建立的檢視只對您和共用檢視的使用者可見。
* 當您修改或刪除檢視時，該檢視會被修改並刪除，以供擁有該檢視許可權的所有使用者使用。
* 每位使用者最多可建立100個檢視。 您可以為記錄型別顯示100個以上的檢視，但一個使用者只能建立100個檢視。
* 雖然某些檢視元素可以套用至相同記錄的多個檢視，但它們對每個記錄檢視都是獨一無二的：

   * 篩選器
   * 分組（針對表格和時間表檢視）
   * 長條圖外觀（適用於時間軸和行事曆檢視）

  例如，在表格檢視中建立篩選時，篩選結果只會在選取的檢視（表格檢視）中顯示，而不會在與記錄型別關聯的所有檢視中顯示。

  >[!TIP]
  >
  >某些檢視元素並非對所有檢視都可用。


## 記錄檢視之間的相似之處和差異

下表顯示表格、時間表與行事曆檢視之間的異同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格檢視 | 時間軸檢視 | 行事曆檢視 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 在清單或表格中顯示記錄 | ✓ |              | |
| 預設將所有欄位顯示為表格中的欄 | ✓ |              |    |
| 隱藏或顯示欄位 | ✓ |               |    |
| 編輯每個記錄的欄位值 | ✓ |               |             |
| 在檢視中將記錄新增為新列 | ✓ |               |        |
| 在檢視中新增欄位作為新欄 | ✓ |               |         |
| 從外部清單複製列並將它們貼到表格中 | ✓ |               |          |
| 在時間軸中顯示記錄 |            | ✓ |             |
| 篩選記錄 | ✓ | ✓ | ✓ |
| 顯示行事曆上的記錄 |           |              | ✓ |
| 群組記錄 | ✓ | ✓ |  |
| 排序記錄 | ✓ |              |  |
| 色彩代碼記錄 | ✓ | ✓ | ✓ |
| Color-code分組 |           | ✓ |  |
| 搜尋特定記錄 | ✓ | ✓ |  |
| 與其他人共用檢視 | ✓ | ✓ | ✓ |
| 從檢視開啟記錄頁面 | ✓ | ✓ |    |
| 依年份和季度顯示記錄 |           | ✓ |    |
| 依月份顯示記錄 |           | ✓ | ✓ |
| 按周顯示記錄 |           |               | ✓ |
| 從檢視匯出資訊 | ✓ |               |    |
| 以全熒幕顯示 | ✓ | ✓ | ✓ |
| 在檢視中建立記錄 | ✓ | ✓ | ✓ |

## 建立或編輯檢視 {#create-or-edit-views}

{{step1-to-planning}}


1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

   依預設，選取型別的所有記錄都會顯示在表格檢視中。

1. 按一下目前檢視名稱旁邊的下拉式清單圖示![下拉式清單圖示](assets/drop-down-icon.png)，然後按一下&#x200B;**+新增檢視**。

1. 從下列檢視型別中選取：

   * 表格
   * 時間軸
   * 行事曆

1. 選擇檢視型別，然後按一下[建立]。**** 新檢視會新增至下拉式功能表。

   >[!TIP]
   >
   >建立記錄型別時，預設也會建立表格檢視。
   >
   >若要建立時間表或行事曆檢視，您為其建立檢視的記錄型別必須至少有兩個日期欄位。
   >
   >否則，「時間軸」和「行事曆」選項會變暗。
   >  

   ![建立檢視方塊](assets/create-view-box.png)

1. （選擇性）若要編輯現有檢視，請按一下目前檢視名稱右側的下拉式功能表，然後在&#x200B;**搜尋**&#x200B;欄位中輸入檢視名稱，然後在鍵盤上按Enter鍵。
1. （可選）從檢視下拉式功能表中，依您的偏好順序拖放檢視。

   ![記錄型別清單中的檢視型別下拉式清單](assets/view-types-drop-down-from-record-type-list.png)

1. （視條件而定）建立時間表或行事曆檢視時，按一下&#x200B;**下一步**。

   依預設，Workfront會提供下列其中一個檢視名稱：

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   數字是自動產生的增量。

1. （視條件而定）針對將在時間軸或行事曆檢視中顯示的記錄，選取&#x200B;**開始**&#x200B;和&#x200B;**結束日期**。

   >[!NOTE]
   >
   >    您可以從記錄日期欄位中選取，或從連線的記錄或物件型別中查詢日期欄位。
   >
   >連線記錄型別時，當您選取查閱欄位時，必須為日期欄位使用彙總(MAX或MIN)。 僅新增彙總可讓您使用連線的日期作為時間軸和行事曆檢視的開始和結束日期。
   >
   >如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. 按一下「**建立**」。

   檢視會顯示為新標籤。 檢視會以建立或與您共用的時間順序顯示。
1. （選擇性）按一下最後一個檢視旁的&#x200B;**更多**&#x200B;功能表![更多向下插入符號圖示檢視](assets/more-caret-down-icon-views.png)，以顯示所選記錄型別的所有檢視。

   最後一個檢視標籤之後的&#x200B;**更多**&#x200B;功能表下會顯示其他檢視。 **更多**&#x200B;功能表旁的數字會顯示其他檢視的數目。
1. （選擇性）若要在建立檢視後重新命名，請按一下檢視下拉式功能表，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png) > **重新命名**&#x200B;以更新檢視名稱

   或

   連按兩下檢視名稱，然後開始輸入新名稱。 <!--ensure there is not another saving step here?!-->

1. （選擇性）按一下&#x200B;**全熒幕**&#x200B;圖示![開啟全熒幕圖示](assets/open-full-screen-icon.png)以全熒幕開啟任何檢視，然後按一下&#x200B;**退出全熒幕**&#x200B;圖示![退出全熒幕圖示](assets/exit-full-screen-icon.png)或鍵盤上的Escape以退出全熒幕。

1. （可選）若要管理特定型別的檢視，請參閱下列文章：

   * [管理表格檢視](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [管理行事曆檢視](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## 在檢視中啟用即時顯示狀態指示器

您可以依照檢視中的即時狀態指示器，檢視其他使用者是否與您同時編輯記錄。

根據預設，當您編輯記錄資訊的同時，其他使用者的頭像會顯示在所有記錄檢視的右上角。

當您顯示表格檢視時，也可以檢視另一個使用者在您檢視記錄時正在編輯的欄位。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。



<!--## Add a view as a favorite - this is not possible yet-->
