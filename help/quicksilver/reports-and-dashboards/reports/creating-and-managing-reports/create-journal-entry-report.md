---
title: 更新區域報告
description: 更新區域報告
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# 更新區域報告

「日記帳分錄」報表會從項目、任務、問題和其他對象的「更新」區域顯示系統更新，這些對象以前只能通過Adobe Workfront API使用。 雖然這是針對特定使用案例的進階報表，但格式越簡單，您就能更輕鬆地報告Workfront中的專案活動和系統更新。

>[!TIP]
>
>「日記帳分錄」報表僅包含對象「更新」區域中的系統更新。 若要報告「更新」區域中剩餘的注釋，必須使用「注釋」報告。\
>如需附註報表的詳細資訊，請參閱 [在「附註」報表中檢視所有更新](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

「日記帳分錄」報表可以顯示：

* 發生了多少個狀態更改
* 刪除任務或問題時
* 重要自訂欄位中的值在專案生命週期中的變更方式
* 在項目的生命週期中，有哪些重要日期發生了更改
* 如果專案的擁有者已變更

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看包含在報表中顯示的日記帳分錄的對象的權限</p> <p>建立報表後，您將取得該報表的管理權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先確定下列事項，才能執行本文所述的動作：

* 您要報告的任何欄位都會在Workfront中追蹤。 您只能報告所追蹤之「更新」區域的資料。

   若要了解如何新增您要Workfront追蹤的欄位，請參閱 [配置系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 您要報告的任何自訂欄位皆已設定 **在更新摘要中顯示欄位變更** 已啟用。

   若要了解如何為自訂欄位啟用此設定，請參閱區段 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 在文章中 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 日記帳分錄報表概覽

由於「日記帳分錄」報表查詢系統更新，因此可以返回大量結果。 因此，我們建議您在建立報表時，篩選特定物件（例如專案、方案、產品組合、群組等）。

若要進一步了解Workfront中的不同物件類型，請參閱 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>由於「日記帳分錄」報表傳回的資料太多，因此不支援匯出和計畫的報表傳送。

此報表的預設檢視包含下列各欄：

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
   <td> <p><span style="font-weight: normal;">受影響欄位的名稱。 根據您設定報表的方式，此列可包含狀態、所有者ID、任務名稱、計畫完成日期或其他欄位。</span> </p> <p><span style="font-weight: normal;">當</span> <strong>DE</strong>:<span style="font-weight: normal;"> 顯示在此欄中，它表示列出的欄位是自訂欄位。</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>更改類型</strong> </td> 
   <td> <p>對受影響欄位所做的變更類型。 根據您設定的篩選規則和使用者採取的動作，此欄位中可能會出現下列項目：</p> 
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
   <td> <p>已更改的對象類型。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>輸入日期</strong> </td> 
   <td> <p>欄位變更的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>按名稱編輯</strong> </td> 
   <td> <p>變更欄位的使用者。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要組織此報告中的資訊，您可以使用內建的分組專案。 「項目」分組為您提供項目名稱的主要分組和錄入日期的輔助分組。 您可以在建立報表時套用此現有分組，或在檢視報表時套用。

若要了解如何設定報表的檢視、篩選和群組，請參閱相關區段：

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [查看發生了哪些狀態更改](#see-what-status-changes-occurred)
* [查看任務或問題的刪除時間](#see-when-a-task-or-issue-was-deleted)
* [查看自訂欄位在專案生命週期中的變更方式](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [查看計畫完成日期在項目生命週期中如何更改](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [查看項目的所有者是否已更改](#see-if-the-owner-of-a-project-changed)

## 查看發生了哪些狀態更改 {#see-what-status-changes-occurred}

您可以設定「日記帳分錄」報表以顯示：

* 對項目、任務或問題進行了多少次狀態更改

* 變更前的狀態
* 更改了狀態的人員
* 狀態更改發生時

如果您想查看專案的運作狀況，也可以設定報表，使用專案顯示相同的資訊 **條件** 欄位。

此資訊可用於幫助進行審計，並說明您和您的組織的規劃情況。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>如果您想比較條件變更之間的天數差異，可以使用增強分析。\
>若要進一步了解增強分析，請參閱 [增強的分析概觀](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選取 **日記帳分錄**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   報告建立工具會載入。

1. 在 **欄（檢視）** 頁簽，添加以下列：

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
      <td> <p>受影響欄位的名稱。 在這種情況下， <strong>狀態</strong> 應會顯示在此欄中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>對受影響欄位所做的變更類型，例如 <strong>新增</strong>, <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名稱編輯</p> </td> 
      <td> <p>更新狀態的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>狀態更改的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊文字值</p> </td> 
      <td> <p>上一個狀態的鍵。 以下是預設項目狀態的狀態鍵：</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>:目前</p> </li> 
        <li> <p><strong>DED</strong>:死亡</p> </li> 
        <li> <p><strong>ONH</strong>:暫掛</p> </li> 
        <li> <p><strong>PLN</strong>:規劃</p> </li> 
        <li> <p><strong>CPL</strong>:完成</p> </li> 
        <li> <p><strong>請求</strong>:已請求</p> </li> 
        <li> <p><strong>4月</strong>:已核准</p> </li> 
        <li> <p><strong>REJ</strong>:已拒絕</p> </li> 
        <li> <p><strong>IDA</strong>:構想</p> </li> 
       </ul> <p>如果您的組織已設定自訂狀態，則此欄中可能會顯示其他狀態索引鍵。 若要了解哪些自訂狀態與狀態金鑰相關，請聯絡您的Workfront管理員或群組管理員。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文字值</p> </td> 
      <td> <p>更新狀態的金鑰。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>狀態發生更改的欄位的最高父對象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範圍</p> </td> 
      <td> <p>狀態已更改的對象類型。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">問題名稱<br>（可選）</p> </td> 
      <td> <p>狀態發生更改的問題的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任務名稱<br>（可選）</p> </td> 
      <td> <p>狀態發生更改的任務的名稱。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關添加列的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 按一下 **新增篩選規則**，然後新增篩選規則 **欄位名稱** > **等於** > **狀態**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >若要報告條件變更，您可以改為新增篩選規則 **欄位名稱** > **等於** > **條件**.

   如需新增篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可選）若要縮小報表的焦點並縮短載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、工作或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾詞的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議使用不同的修飾詞，例如 **等於** 可以篩選特定專案或較高層級物件ID時。

   若要了解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分組** 按一下 **應用現有分組**，然後選取 **專案**.

   有關添加分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下 **儲存+關閉**.

   新報表載入。

## 查看任務或問題的刪除時間 {#see-when-a-task-or-issue-was-deleted}

您可以設定「日記帳分錄」報表以顯示：

* 已刪除哪些任務或問題
* 刪除任務或問題的人員

查看任務或問題的刪除時間：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選取 **日記帳分錄**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   報告建立工具會載入。

1. 在 **欄（檢視）** 頁簽，添加以下列：

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
      <td> <p>已刪除的對象類型。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>發生的變更類型。 此 <strong>刪除</strong> 此欄中會顯示變更。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>刪除任務或問題的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名稱編輯</p> </td> 
      <td> <p>刪除任務或問題的用戶的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> </td> 
      <td> <p>已刪除任務或問題的項目名稱。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關添加列的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 按一下 **新增篩選規則**，然後新增下列項目：

   * **變更類型** > **等於** > **刪除**
   * **專案ID** > **等於** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   如需新增篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可選）若要縮小報表的焦點並縮短載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、工作或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾詞的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議使用不同的修飾詞，例如 **等於** 可以篩選特定專案或較高層級物件ID時。

   若要了解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （選用）在 **分組** 按一下 **應用現有分組**，然後選取 **專案**.

   有關添加分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下 **儲存+關閉**.

   新報表載入。

## 查看自訂欄位在專案生命週期中的變更方式 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

您可以在專案期間追蹤重要欄位變更。 要執行此操作，您可以設定要跟蹤的日記帳分錄：

* 如果已新增、更新或編輯某些自訂欄位
* 這些變更發生時
* 誰做了更改

查看自定義欄位在項目生命週期中的變化：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選取 **日記帳分錄**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   報告建立工具會載入。

1. 在 **欄（檢視）** 頁簽，添加以下列：

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
      <td> <p>受影響的自訂欄位名稱。</p> <p><span style="font-weight: normal;">當</span> <strong>DE</strong>:<span style="font-weight: normal;"> 顯示在此欄中，它表示列出的欄位是自訂欄位。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>對受影響欄位所做的變更類型，例如 <strong>新增</strong>, <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名稱編輯</p> </td> 
      <td> <p>更新自訂欄位的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>自訂欄位中值變更的日期。</p> <p>您應依此欄位以降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊數值</p> </td> 
      <td> <p>自訂欄位中的前一個數字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新數值</p> </td> 
      <td> <p>自訂欄位中的目前數字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊日期值</p> </td> 
      <td> <p>自訂欄位中的上一個日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>自訂欄位中的目前日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊文字值</p> </td> 
      <td> <p>自訂欄位中的上一個文字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文字值</p> </td> 
      <td> <p>自訂欄位中的目前文字值。</p> <p>如果自訂欄位是字型預覽欄位，則 <strong>新文字值</strong> 欄顯示對象ID。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關添加列的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 按一下 **新增篩選規則**，然後新增下列項目：

   * **日記帳分錄欄位名稱** > **包含** > **DE**

      >[!TIP]
      >
      >若要將此報表限制為特定自訂欄位，請新增篩選規則 **日記帳分錄欄位名稱** > **等於** > **`<custom field>`**.

   * **專案ID** > **等於** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   如需新增篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可選）若要縮小報表的焦點並縮短載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、工作或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾詞的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議使用不同的修飾詞，例如 **等於** 可以篩選特定專案或較高層級物件ID時。

   若要了解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分組** 按一下 **應用現有分組**，然後選取 **專案**.

   有關添加分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下 **儲存+關閉**.

   新報表載入。

## 查看計畫完成日期在項目生命週期中如何更改 {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

您可以設定「日記帳分錄」報表，以顯示計畫完成日期在項目生命週期中的更改頻率。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選取 **日記帳分錄**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   報告建立工具會載入。

1. 在 **欄（檢視）** 頁簽，添加以下列：

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
      <td> <p>受影響欄位的名稱。</p> <p><span style="font-weight: normal;">當</span> <strong>DE</strong>:<span style="font-weight: normal;"> 顯示在此欄中，它表示列出的欄位是自訂欄位。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td>發生的變更類型，例如 <strong>新增</strong>, <strong>刪除</strong>，或 <strong>編輯</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名稱編輯</p> </td> 
      <td> <p>更新項目計畫完成日期的用戶名。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td> <p>更改項目計畫完成日期的日期。</p> <p>您應依此欄位以降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>計畫完成日期更改的欄位的最高父對象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範圍</p> </td> 
      <td> <p>計畫完成日期更改的對象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">舊日期值</p> </td> 
      <td> <p>計畫完成日期的前一個值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>計畫完成日期的當前值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> <p>(可選)</p> </td> 
      <td> <p>計畫完成日期更改的項目名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任務名稱</p> <p>(可選)</p> </td> 
      <td> <p>計畫完成日期更改的項目中任務的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">問題名稱</p> <p>(可選)</p> </td> 
      <td>項目中計畫完成日期更改的問題的名稱。</td> 
     </tr> 
    </tbody> 
   </table>

   有關添加列的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 按一下 **新增篩選規則**，然後新增下列項目：

   * **欄位名稱** > **等於** > **日期**
   * **專案ID** > **等於** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   如需新增篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可選）若要縮小報表的焦點並縮短載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、工作或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾詞的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議使用不同的修飾詞，例如 **等於** 可以篩選特定專案或較高層級物件ID時。

   若要了解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分組** 按一下 **應用現有分組**，然後選取 **專案**.

   有關添加分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下 **儲存+關閉**.

   新報表載入。

## 查看項目的所有者是否已更改 {#see-if-the-owner-of-a-project-changed}

您可以設定「日記帳分錄」報表，以顯示項目所有者（或項目經理）在項目生命週期中的更改次數。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選取 **日記帳分錄**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   報告建立工具會載入。

1. 在 **欄（檢視）** 頁簽，添加以下列：

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
      <td>受影響欄位的名稱。 此 <strong>ownerID</strong> 顯示於此欄中。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改類型</p> </td> 
      <td> <p>發生的變更類型，例如 <strong>新增</strong>, <strong>刪除</strong>，或 <strong>編輯</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要物件代碼</p> </td> 
      <td> <p>已更新項目所有者的項目的最高父對象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">輸入日期</p> </td> 
      <td>變更專案擁有者的日期。<br>您應依此欄位以降序排序。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名稱編輯</p> </td> 
      <td> <p>更新專案擁有者的使用者名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">其他資訊 1</p> </td> 
      <td> <p>專案的目前專案擁有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">其他資訊 2</p> </td> 
      <td> <p>專案的上一個專案擁有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">專案名稱</p> </td> 
      <td> <p>已更新「項目所有者」欄位的項目。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關添加列的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **篩選器** 按一下 **新增篩選規則**，然後新增下列項目：

   * **欄位名稱** > **等於** > **ownerID**
   * **專案ID** > **等於** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   如需新增篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可選）若要縮小報表的焦點並縮短載入時間，請新增提示。

   或

   建立其他篩選規則以包含特定專案、工作或問題。

   >[!IMPORTANT]
   >
   >建立使用修飾詞的篩選規則 **包含** 實際上會增載入入時間。 因此，我們建議使用不同的修飾詞，例如 **等於** 可以篩選特定專案或較高層級物件ID時。

   若要了解如何新增提示，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （選用）在 **分組** 按一下 **應用現有分組**，然後選取 **專案**.

   有關添加分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 按一下 **儲存+關閉**.

   新報表載入。
