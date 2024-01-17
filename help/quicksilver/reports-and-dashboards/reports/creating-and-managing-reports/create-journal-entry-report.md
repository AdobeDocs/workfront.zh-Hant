---
title: 更新區域報告
description: 「日誌專案」報表會從專案、工作、問題和其他物件的更新區域顯示系統更新，這些先前只能透過Adobe Workfront API使用。 雖然此為適用於特定使用案例的進階報表，但格式越容易解讀，您就能更輕鬆地在Workfront中報告專案活動和系統更新。
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 94c2930d155f38a56fe36e5a09bd29f27d1593f0
workflow-type: tm+mt
source-wordcount: '2765'
ht-degree: 4%

---

# 更新區域報告

「日誌專案」報表會從專案、工作、問題和其他物件的更新區域顯示系統更新，這些先前只能透過Adobe Workfront API使用。 雖然此為適用於特定使用案例的進階報表，但格式越容易解讀，您就能更輕鬆地在Workfront中報告專案活動和系統更新。

>[!TIP]
>
>「日誌專案」報表只包含物件更新區域的系統更新。 若要報告「更新」區域中剩餘的註解，您必須使用「註記」報告。\
>如需有關「附註」報表的詳細資訊，請參閱 [在備註報告中檢視所有更新](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

「日誌專案」報表可顯示：

* 已發生的狀態變更數量
* 刪除任務或問題時
* 重要自訂欄位中的值在專案生命週期中如何變更
* 在專案生命週期中變更了哪些重要日期
* 如果專案所有者已變更

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準 </p><p>或 </p><p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視物件的許可權，這些物件包含您在報表中顯示的日誌專案</p> <p>建立報表後，您將會取得報表的管理許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

您必須先確定下列事項，才能執行本文所述的動作：

* 您想要報告的任何欄位會在Workfront中進行追蹤。 您只能報告來自已追蹤更新區域的資料。

  若要瞭解如何新增您希望Workfront追蹤的欄位，請參閱 [設定系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 您要報告的任何自訂欄位都有設定 **在更新摘要中顯示欄位變更** 已啟用。

  若要瞭解如何為自訂欄位啟用此設定，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#).

## 分錄報表概觀

由於「日誌專案」報表會查詢系統更新，因此可傳回大量結果。 因此，在建立報告時，我們建議您篩選至特定物件，例如專案、方案、投資組合、群組等。

若要進一步瞭解Workfront中的不同物件型別，請參閱 [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>由於「日誌專案」報表會傳回太多資料，因此不支援匯出和已排程的報表傳送。

此報表的預設檢視包含下列欄：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>欄位名稱</strong> </td> 
   <td> <p><span style="font-weight: normal;">受影響欄位的名稱。 根據您設定報表的方式，此欄可能包含「狀態」、「擁有者ID」、「任務名稱」、「計畫完成日期」或其他欄位。</span> </p> <p><span style="font-weight: normal;">時間</span> <strong>DE</strong>：<span style="font-weight: normal;"> 會顯示在此欄中，表示所列的欄位是自訂欄位。</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>變更型別</strong> </td> 
   <td> <p>對受影響欄位進行的變更型別。 根據您設定的篩選規則和使用者採取的動作，下列內容可能會顯示在此欄位中：</p> 
    <ul> 
     <li> <p>新增</p> </li> 
     <li> <p>稽核</p> </li> 
     <li> <p>刪除</p> </li> 
     <li> <p>摘要</p> </li> 
     <li> <p>編輯</p> </li> 
     <li> <p>還原</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>主要物件代碼</strong> </td> 
   <td> <p>階層中最高的父物件。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>範圍</strong> </td> 
   <td> <p>已變更的物件型別。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>輸入日期</strong> </td> 
   <td> <p>欄位變更的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>依名稱編輯</strong> </td> 
   <td> <p>變更欄位的使用者。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要組織此報表中的資訊，您可以使用名為「專案」的內建群組。 「專案」群組提供「專案名稱」的主要群組以及「輸入日期」的次要群組。 您可以在建立報表時套用這個現有的群組，也可以在檢視報表時套用它。

若要瞭解如何設定您要用於報告的檢視、篩選器和群組，請參閱相關區段：

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [檢視已發生的狀態變更](#see-what-status-changes-occurred)
* [檢視任務或問題何時被刪除](#see-when-a-task-or-issue-was-deleted)
* [檢視自訂欄位在專案生命週期中的變更情形](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [檢視計畫完成日期在專案生命週期中的變化](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [檢視專案所有者是否已變更](#see-if-the-owner-of-a-project-changed)

## 檢視已發生的狀態變更 {#see-what-status-changes-occurred}

您可以設定「分錄」報表以顯示：

* 對專案、任務或問題做了多少狀態變更

* 變更前的狀態
* 誰變更了狀態
* 發生狀態變更的時間

如果您想要檢視專案的健康情況，也可以使用專案設定報告以顯示相同的資訊 **條件** 欄位。

此資訊可用於協助稽核及說明您與貴組織的規劃成效。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>如果您想比較條件變更之間的天數差異，可使用增強型分析。\
>若要進一步瞭解增強型分析，請參閱 [增強型分析概述](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取 **日誌專案**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder隨即載入。

1. 在 **欄（檢視）** 索引標籤中，新增下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>直條</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">欄位名稱</p> </td> 
      <td> <p>受影響欄位的名稱。 在這種情況下， <strong>狀態</strong> 應該會顯示在此欄中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>對受影響欄位進行的變更型別，例如 <strong>新增</strong>， <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">依名稱編輯</p> </td> 
      <td> <p>更新狀態的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>狀態變更的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊文字值</p> </td> 
      <td> <p>上一個狀態的索引鍵。 以下是預設專案狀態的狀態索引鍵：</p> 
       <ul> 
        <li> <p> <strong>目前</strong>：目前</p> </li> 
        <li> <p><strong>DED</strong>：廢棄</p> </li> 
        <li> <p><strong>一</strong>：保留</p> </li> 
        <li> <p><strong>計畫</strong>：規劃</p> </li> 
        <li> <p><strong>CPL</strong>：完成</p> </li> 
        <li> <p><strong>需要</strong>：已要求</p> </li> 
        <li> <p><strong>四月</strong>：已核准</p> </li> 
        <li> <p><strong>REJ</strong>：已拒絕</p> </li> 
        <li> <p><strong>IDA</strong>：構想</p> </li> 
       </ul> <p>如果您的組織已設定自訂狀態，其他狀態索引鍵可能會顯示在此欄中。 若要瞭解哪些自訂狀態與狀態索引鍵相關，請聯絡您的Workfront管理員或群組管理員。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文字值</p> </td> 
      <td> <p>更新狀態的索引鍵。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>狀態已變更之欄位的最高父物件。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範圍</p> </td> 
      <td> <p>狀態已變更的物件型別。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">問題名稱<br>（可選）</p> </td> 
      <td> <p>狀態變更的問題名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任務名稱<br>（可選）</p> </td> 
      <td> <p>狀態變更的工作名稱。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   如需新增欄的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 標籤，按一下 **新增篩選器規則**，然後新增篩選規則 **欄位名稱** > **等於** > **狀態**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >若要報告條件變更，您可以改為新增篩選規則 **欄位名稱** > **等於** > **條件**.

   如需新增篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）若要縮小報表焦點並減少載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、任務或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾元的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議您使用不同的修飾元，例如 **等於** 儘可能篩選特定專案或較高層級物件ID。

   若要瞭解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **群組** 標籤，按一下 **套用現有群組**，然後選取 **專案**.

   如需新增群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下「**儲存並關閉**」。

   新報表隨即載入。

## 檢視任務或問題何時被刪除 {#see-when-a-task-or-issue-was-deleted}

您可以設定「分錄」報表以顯示：

* 已刪除哪些任務或問題
* 刪除任務或問題的人員

若要檢視任務或問題何時被刪除：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取 **日誌專案**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder隨即載入。

1. 在 **欄（檢視）** 索引標籤中，新增下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>直條</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">範圍</p> </td> 
      <td> <p>已刪除的物件型別。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>發生的變更型別。 此 <strong>刪除</strong> 變更會顯示在此欄中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>刪除任務或問題的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">依名稱編輯</p> </td> 
      <td> <p>刪除任務或問題的使用者的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> </td> 
      <td> <p>已刪除任務或問題的專案名稱。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   如需新增欄的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 標籤，按一下 **新增篩選器規則**，然後新增下列篩選器：

   * **變更型別** > **等於** > **刪除**
   * **專案ID** > **等於** > **`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   如需新增篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）若要縮小報表焦點並減少載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、任務或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾元的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議您使用不同的修飾元，例如 **等於** 儘可能篩選特定專案或較高層級物件ID。

   若要瞭解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （選用）在 **群組** 標籤，按一下 **套用現有群組**，然後選取 **專案**.

   如需新增群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下「**儲存並關閉**」。

   新報表隨即載入。

## 檢視自訂欄位在專案生命週期中的變更情形 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

您可以追蹤專案過程中重要欄位變更。 若要這麼做，您可以設定要追蹤的日誌專案：

* 是否已新增、更新或編輯某些自訂欄位
* 這些變更發生的時間
* 誰進行了變更

若要檢視自訂欄位在專案生命週期中的變更情形：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取 **日誌專案**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder隨即載入。

1. 在 **欄（檢視）** 索引標籤中，新增下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>直條</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">欄位名稱</p> </td> 
      <td> <p>受影響的自訂欄位名稱。</p> <p><span style="font-weight: normal;">時間</span> <strong>DE</strong>：<span style="font-weight: normal;"> 會顯示在此欄中，表示所列的欄位是自訂欄位。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>對受影響欄位進行的變更型別，例如 <strong>新增</strong>， <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">依名稱編輯</p> </td> 
      <td> <p>更新自訂欄位的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>自訂欄位中的值變更的日期。</p> <p>您應該依此欄位遞減排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊數值</p> </td> 
      <td> <p>自訂欄位中的上一個數值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新數值</p> </td> 
      <td> <p>自訂欄位中目前的數字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊日期值</p> </td> 
      <td> <p>自訂欄位中的前一個日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>自訂欄位中目前的日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊文字值</p> </td> 
      <td> <p>自訂欄位中的上一個文字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文字值</p> </td> 
      <td> <p>自訂欄位中目前的文字值。</p> <p>如果自訂欄位是預先輸入欄位， <strong>新文字值</strong> 欄會顯示物件ID。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   如需新增欄的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 標籤，按一下 **新增篩選器規則**，然後新增下列篩選器：

   * **日誌專案欄位名稱** > **包含** > **DE**

     >[!TIP]
     >
     >若要將此報告限製為特定自訂欄位，請新增篩選規則 **日誌專案欄位名稱** > **等於** > **`<custom field>`**.

   * **專案ID** > **等於** > **`<project>`**

     ![](assets/qs-custom-form-changes-filter-350x92.png)

   如需新增篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）若要縮小報表焦點並減少載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、任務或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾元的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議您使用不同的修飾元，例如 **等於** 儘可能篩選特定專案或較高層級物件ID。

   若要瞭解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **群組** 標籤，按一下 **套用現有群組**，然後選取 **專案**.

   如需新增群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下「**儲存並關閉**」。

   新報表隨即載入。

## 檢視計畫完成日期在專案生命週期中的變化 {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

您可以設定「日誌專案」報表，以顯示「計畫完成日期」在專案生命週期中變更的頻率。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取 **日誌專案**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder隨即載入。

1. 在 **欄（檢視）** 索引標籤中，新增下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>直條</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">欄位名稱</p> </td> 
      <td> <p>受影響欄位的名稱。</p> <p><span style="font-weight: normal;">時間</span> <strong>DE</strong>：<span style="font-weight: normal;"> 會顯示在此欄中，表示所列的欄位是自訂欄位。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td>發生的變更型別，例如 <strong>新增</strong>， <strong>刪除</strong>，或 <strong>編輯</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">依名稱編輯</p> </td> 
      <td> <p>更新專案計畫完成日期的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>變更專案計畫完成日期的日期。</p> <p>您應該依此欄位遞減排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>計畫完成日期變更的欄位的最高父級物件。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範圍</p> </td> 
      <td> <p>計畫完成日期變更的物件。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊日期值</p> </td> 
      <td> <p>計畫完成日期的先前值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>計畫完成日期的目前值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> <p>（可選）</p> </td> 
      <td> <p>計畫完成日期變更的專案名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任務名稱</p> <p>（可選）</p> </td> 
      <td> <p>專案中計畫完成日期變更的任務名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">問題名稱</p> <p>（可選）</p> </td> 
      <td>專案中計畫完成日期變更的問題名稱。</td> 
     </tr> 
    </tbody> 
   </table>

   如需新增欄的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 標籤，按一下 **新增篩選器規則**，然後新增下列專案：

   * **欄位名稱** > **等於** > **日期**
   * **專案ID** > **等於** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   如需新增篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）若要縮小報表焦點並減少載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、任務或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾元的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議您使用不同的修飾元，例如 **等於** 儘可能篩選特定專案或較高層級物件ID。

   若要瞭解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **群組** 標籤，按一下 **套用現有群組**，然後選取 **專案**.

   如需新增群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下「**儲存並關閉**」。

   新報表隨即載入。

## 檢視專案所有者是否已變更 {#see-if-the-owner-of-a-project-changed}

您可以設定「日誌專案」報表，以顯示專案所有者（或專案經理）在專案生命週期中的變更次數。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取 **日誌專案**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder隨即載入。

1. 在 **欄（檢視）** 索引標籤中，新增下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>直條</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">欄位名稱</p> </td> 
      <td>受影響欄位的名稱。 此 <strong>ownerID</strong> 會顯示在此欄中。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>發生的變更型別，例如 <strong>新增</strong>， <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>已更新專案所有者的專案之最高父物件。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td>變更專案所有者的日期。<br>您應該依此欄位遞減排序。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">依名稱編輯</p> </td> 
      <td> <p>更新專案所有者的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">其他資訊 1</p> </td> 
      <td> <p>專案目前的專案所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">其他資訊 2</p> </td> 
      <td> <p>專案的前一個專案所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> </td> 
      <td> <p>已更新「專案所有者」欄位的專案。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   如需新增欄的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 標籤，按一下 **新增篩選器規則**，然後新增下列專案：

   * **欄位名稱** > **等於** > **ownerID**
   * **專案ID** > **等於** > **`<project name>`**

     ![](assets/qs-owner-changes-filter-350x94.png)

   如需新增篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）若要縮小報表焦點並減少載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、任務或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾元的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議您使用不同的修飾元，例如 **等於** 儘可能篩選特定專案或較高層級物件ID。

   若要瞭解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （選用）在 **群組** 標籤，按一下 **套用現有群組**，然後選取 **專案**.

   如需新增群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下「**儲存並關閉**」。

   新報表隨即載入。
