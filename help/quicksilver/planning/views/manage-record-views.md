---
title: 管理記錄檢視
description: 使用Adobe Workfront Planning時，您可以在表格、時間軸或行事曆檢視中顯示記錄。 本文說明如何建立檢視，以及如何編輯或刪除現有檢視。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 1%

---


# 管理記錄檢視

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
* [刪除檢視](#delete-views)
* [複製檢視](#duplicate-views)
* [在檢視中啟用即時狀態指示器](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


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

<!--old: 

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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## 使用記錄檢視時的注意事項

* Workfront Planning中的檢視是記錄型別專屬檢視。 您不能將相同的檢視套用至兩種不同的記錄型別。
* 您建立的檢視只對您和共用檢視的使用者可見。
* 當您修改或刪除檢視時，該檢視會被修改並刪除，以供擁有該檢視許可權的所有使用者使用。
* 每位使用者最多可建立100個檢視。 您可以為記錄型別顯示100個以上的檢視，但一個使用者只能建立100個檢視。
* 您可以與其他人共用您建立的檢視。 如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。
* 以下元素是每個記錄檢視所獨有的：

   * 篩選器
   * 分組
   * 排序
   * 長條圖外觀（用於時間軸檢視）

  <!-- some of these are not available in all of the views - edit above-->

  例如，在表格檢視中建立篩選時，篩選結果只會在選取的檢視中顯示，而不會在與記錄型別相關的所有檢視中顯示。

  >[!NOTE]
  >
  > 某些檢視元素可能不適用於所有檢視。


## 記錄檢視之間的相似之處和差異

下表顯示表格、時間表與行事曆檢視之間的異同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格檢視 | 時間表檢視 | 行事曆檢視 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 在清單或表格中顯示記錄 | ✓ (A) |              | |
| 預設將所有欄位顯示為表格中的欄 | ✓ (A) |              |    |
| 隱藏或顯示欄位 | ✓ (A) |               |    |
| 編輯每個記錄的欄位值 | ✓ (A) |               |             |
| 在檢視中將記錄新增為新列 | ✓ (A) |               |        |
| 在檢視中新增欄位作為新欄 | ✓ (A) |               |         |
| 從外部清單複製列並將它們貼到表格中 | ✓ (A) |               |          |
| 在時間軸中顯示記錄 |            | ✓ (A) |             |
| 篩選記錄 | ✓ (A) | ✓ (A) | ✓ (A) |
| 顯示行事曆上的記錄 |           |              | ✓ (A) |
| 群組記錄 | ✓ (A) | ✓ (A) |
| 排序記錄 | ✓ (A) |              |
| 色彩代碼記錄 |           | ✓ (A) | ✓ (A) |
| Color-code分組 |           | ✓ (A) |
| 搜尋特定記錄 | ✓ (A) | ✓ (A) |
| 與其他人共用檢視 | ✓ (A) | ✓ (A) | ✓ (A) |
| 從檢視開啟記錄頁面 | ✓ (A) | ✓ (A) |    |


## 建立或編輯檢視 {#create-or-edit-views}

{{step1-to-planning}}


1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

   依預設，選取型別的所有記錄都會顯示在表格檢視中。

1. 按一下「**+檢視**」以新增檢視。
1. 從下列檢視型別中選取：

   * 表格
   * 時間軸
   * 行事曆

   會以選取的檢視建立新標籤。

   視熒幕寬度而定，**更多**&#x200B;功能表![](assets/more-menu.png)中可能會顯示其他檢視。


>[!TIP]
>
>建立記錄型別時，預設也會建立表格檢視。
>
>若要建立時間表或行事曆檢視，您為其建立檢視的記錄型別必須至少有兩個日期欄位。
>
>否則，「時間軸」和「行事曆」選項會變暗。
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. （視條件而定）建立時間表或行事曆檢視時，按一下&#x200B;**下一步**。

   依預設，Workfront會提供下列其中一個檢視名稱：

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   數字是自動產生的增量。

1. （視條件而定）針對將在時間軸或行事曆檢視中顯示的記錄，選取&#x200B;**開始**&#x200B;和&#x200B;**結束日期**。

   >[!TIP]
   >
   >    您可以從記錄日期欄位中選取，或從連線的記錄或物件型別中查詢日期欄位。 當您選取查閱欄位作為時間軸和行事曆檢視的開始和結束日期時，您必須使用日期欄位的彙總(MAX或MIN)。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. 按一下「**建立**」。

   檢視會顯示為新標籤。 檢視會以建立或與您共用的時間順序顯示。
1. （選擇性）按一下最後一個檢視旁的&#x200B;**更多**&#x200B;功能表![](assets/more-caret-down-icon-views.png)，以顯示所選記錄型別的所有檢視。

   最後一個檢視標籤之後的&#x200B;**更多**&#x200B;功能表下會顯示其他檢視。 **更多**&#x200B;功能表旁的數字會顯示其他檢視的數目。
1. （選擇性）若要在建立檢視後重新命名，請按一下檢視下拉式功能表，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png) > **重新命名**&#x200B;以更新檢視名稱

   或

   連按兩下檢視名稱，然後開始輸入新名稱。 <!--ensure there is not another saving step here?!-->

1. （可選）若要管理特定型別的檢視，請參閱下列文章：

   * [管理表格檢視](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [管理行事曆檢視](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## 刪除檢視

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

   依預設，選取型別的所有記錄都會顯示在表格檢視中。

1. 將游標暫留在檢視標籤中其中一個檢視名稱上，然後按一下檢視名稱左邊的&#x200B;**更多** ![](assets/more-menu.png)，然後按一下&#x200B;**刪除**。
首先，您可能需要按一下最後一個標籤左側的**更多**，以尋找您要刪除的檢視。

1. 按一下&#x200B;**刪除**&#x200B;確認。<!--ensure there is not another saving step here?!-->

   所有可存取記錄區域的使用者檢視都會刪除，且無法復原。

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## 複製檢視

如果您想要保留一個檢視的多個版本，並在這些版本之間做些微變更，您可以複製一個檢視。

複製檢視會建立現有檢視的相同副本。

原始檢視的共用許可權不會轉移到複製的檢視。

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
依預設，所選型別的所有記錄都會顯示在表格檢視中。

1. 將游標停留在您要複製的檢視的索引標籤上，然後按一下檢視名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**複製**。

   ![](assets/view-more-menu-with-duplicate-option.png)


   檢視重複，新檢視的名稱遵循下列模式： `Original view's name (Copy)`。 新的檢視標籤會顯示在所有檢視標籤的末尾。

## 在檢視中啟用即時顯示狀態指示器

根據預設，當您編輯記錄資訊的同時，其他使用者的頭像會顯示在所有記錄檢視的右上角。

當您顯示表格檢視時，也可以檢視另一個使用者在您檢視記錄時正在編輯的欄位。

1. 移至記錄型別頁面並開啟任何檢視。
1. （視條件而定）如果有其他使用者同時編輯所選型別的記錄，則其頭像會顯示在檢視的右上角。
1. 按一下頭像旁的下拉式功能表，選取「**顯示共同作業人員**」切換按鈕。 依預設，會選取切換。

   ![](assets/show-collaborators-toggle-selected.png)

1. （視條件而定）開啟表格檢視，另一個人正在主動編輯的欄位會以對應表格檢視中其顯示圖片外框的顏色反白。

   如果頭像的醒目提示顏色是灰色，使用者將在30秒前停止主動編輯記錄。

   ![](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >您可以從任何檢視中選取&#x200B;**顯示共同作業人員**&#x200B;切換按鈕。 目前由其他人編輯的欄位僅在表格檢視中列出。
