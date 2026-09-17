---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 畫布控制面板的報表篩選參考
description: 在「畫布控制面板」中篩選報表時，所使用欄位、運運算元、萬用字元和特殊規則的參考。
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 85ae49708acf2c472816ac848ce15429577b934e
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 9%
---
# 畫布控制面板的報表篩選參考

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

本文介紹篩選報表時可用的欄位、運運算元、萬用字元和特殊規則。 如需建立或編輯篩選器的步驟，請參閱[在畫布儀表板中篩選報告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-a-report.md)。

## 依欄位型別的欄位運運算元

+++ 展開以依欄位型別檢視欄位運運算元清單。 

<table>
    <tr>
        <td><b>欄位型別</b></td>
        <td><b>範例</b></td>
       <td><b>操作者</b></td>
        <td><b>萬用字元</b></td>
    </tr>
    <tr>
        <td>物件/參考名稱</td>
        <td>任何原生名稱屬性或自訂查詢</td>
              <td><ul>
        <li>等於</li>
        <li>不等於</li>
        <li>包含</li>
          <li>不包含</li>
            <li>為 Null</li>
              <li>不為 Null</li>
        </ul></td>
        <td>使用者：名稱
        <ul>
        <li>我 (已登入的使用者)</li>
        </ul>
        群組：名稱
        <ul>
          <li>我的家庭群組 (已登入的使用者群組)</li>
            <li>我的其他群組 (已登入的使用者群組)</li>
          </ul>
          團隊：名稱
                  <ul>
          <li>我的預設團隊 (已登入的使用者團隊)</li>
            <li>我的其他團隊 (已登入的使用者團隊)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>字串/文字輸入 </td>
                <td>專案：說明</td>
                      <td><ul>
             <li>等於</li>
        <li>不等於</li>
        <li>包含</li>
          <li>不包含</li>
            <li>為 Null</li>
              <li>不為 Null</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>整數/雙精度</td>
             <td>專案：計畫時數
        <br>任務：完成百分比</td>
              <td><ul>
        <li>等於</li>
        <li>不等於</li>
        <li>大於</li>
          <li>大於或等於</li>
          <li>小於</li>
          <li>小於或等於</li>
            <li>為 Null</li>
              <li>不為 Null</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> 日期/日期時間 </td>
                    <td>專案：計劃開始日期
        <br>小時：輸入日期</td>
              <td><ul>
        <li>等於</li>
        <li>不等於</li>
        </ul></td>
        <td>透過切換<b>設定相對日期</b>選項，您可以套用相對日期萬用字元，讓報表更動態，並根據一般日期期間進行自我調整。 
         <ul><li>$$今天</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>布林值 </td>
                  <td>專案：有檔案
        <br>任務：嚴重
        <br>位使用者：作用中</td>
        <td><ul>
        <li>等於</li>
        <li>不等於</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++

## 以日期為基礎的萬用字元篩選變數

日期型萬用字元選項可與任何日期篩選屬性結合使用。 如需有關新增日期萬用字元至報表的資訊，請參閱[使用日期萬用字元來一般化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

>[!NOTE]
>
>如果您建立的日期和時間計算不包含時間部分，或使用日期萬用字元$$TODAY或$$NOW，則系統會根據世界協調時間(UTC)區域使用日期，而不是根據您的當地時區。 這可能會造成非預期的日期結果。

您可以從下列日期型萬用字元中選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$今天</strong> </p> </td> 
   <td> <p>建議您使用此萬用字元建立日期敏感型篩選器，以免在明天、下週或下個月再次建立篩選器。</p> <p>例如，如果您想要顯示今天之前到期的所有任務，您可以在任務篩選中使用下列規則： <em>規劃開始日期小於$$TODAY</em>。</p> <p>$$TODAY一律等於當天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$現在</strong> </p> </td> 
   <td> <p>這類似於$$TODAY萬用字元，但包含目前的日期和時間。 $$NOW等於目前的日期和時間。</p> <p>例如，如果您想要顯示截至目前時間提供的所有小時專案，您可以在小時篩選中使用下列規則來執行： <em>規劃開始日期小於$$NOW</em>。</p> <p>注意：資源規劃工具不支援這個萬用字元。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要指出不同的時段和不同的時間點（未來或過去），您可以將上述萬用字元與下列內容結合：

| 屬性 |   |
|---|---|
| **q** | 行事曆季度 |
| **小時** | 小時 |
| **d** | 天 |
| **w** | 週 |
| **m** | 月 |
| **y** | 年 |

{style="table-layout:auto"}

| **限定詞** |   |
|---|---|
| **b** | 期間開始（沒有指定屬性，預設為一週的開始：星期日） |
| **e** | 期間結束（沒有指定屬性，預設為一週結束：星期六） |

{style="table-layout:auto"}

| **運運算元** |   |
|---|---|
| **+** | 將值新增至萬用字元值 |
| **-** | 從萬用字元值中減去值 |

{style="table-layout:auto"}

例如，萬用字元`$$TODAYb+2w`是指「從本週開始的2週」。 萬用字元`$$NOW+2h`表示「從現在起的2小時」。

## 登入的使用者萬用字元篩選變數

* 篩選使用者`name`屬性時，您將檢視&#x200B;**我（已登入使用者）**&#x200B;選項。

  ![使用者名稱屬性](assets/user-name-attribute.png)

* 篩選群組`name`屬性時，您將檢視要在篩選條件中使用的&#x200B;**我的主群組（登入使用者群組）**&#x200B;和&#x200B;**我的其他群組（登入使用者群組）**&#x200B;選項。

  ![群組名稱屬性](assets/group-name-attribute.png)

* 篩選團隊`name`屬性時，您將檢視&#x200B;**我的預設團隊（已登入使用者團隊）**&#x200B;和&#x200B;**我的其他團隊（已登入使用者團隊）**&#x200B;選項，以便在篩選條件中選擇。

  ![團隊名稱屬性](assets/team-name-attribute.png)

## 參照子物件

其他欄、篩選選項和群組屬性的可用關係通常僅限於Workfront物件階層中較高的物件，或在報表的基本實體物件上具有單一選取範圍。 但有一些例外，包括：

* 專案>任務
* 檔案核准>檔案核准階段
* 檔案核准階段>檔案核准階段參與者

使用上面列出的任何父項至子項關係時，您會在表格中看到連線到父物件的每個子記錄的一列。

<!--
<div class="preview">

## Filter on collection relationships in Preview

A collection is a field that links to a group of related records rather than to a single record. For example, the participants on a project's approval stages are a collection. When you build a filter, you can filter on collections directly, without switching to text mode.

To filter on a collection, open the Select a field panel, then select Collections. This section lists only collection relationships. Single-record relationships stay under Relationships.

![collection relationships](assets/collections.png)

After you select a collection, you can do two things:

* Filter on the collection's own fields. For example, from a portfolio's projects, you can filter on a project's status.
* Follow one single-record relationship out of the collection. For example, from a portfolio's projects, you can reach the project owner.

Collections don't support deeper navigation. You can't open a collection nested inside another collection, follow more than one relationship, or select the relationship that leads back to where you started.

The Collections section appears only when you build a filter. It doesn't appear in other field choosers, such as those for table columns, groupings, or chart fields.

</div>

-->

## 排除個人專案、任務和機器人使用者

>[!NOTE]
>
>如果「畫布控制面板」報表傳回的結果比您預期類似「傳統」報表還要多，預設情況下可能納入個人專案、個人工作或機器人使用者。 新增篩選條件以將其排除。

在畫布儀表板專案和任務報告中，`isPersonal`篩選器不會自動套用，因此預設會將個人專案和個人任務包含在結果中。 若要排除這些專案，請新增篩選條件，例如`isPersonal=false`。

同樣地，畫布控制面板使用者報表預設會包含所有使用者，包括AI共同作業人員（機器人使用者）。 若要排除機器人使用者，請新增篩選條件，例如`isBot=false`。

傳統專案和任務報告會自動排除個人專案和個人任務，而傳統使用者報告會自動排除機器人使用者。 若要改為將其納入傳統報表，請新增篩選條件，例如`isPersonal=true` （僅限個人專案）或`isPersonal_Mod=notnull` （個人和非個人專案）。
