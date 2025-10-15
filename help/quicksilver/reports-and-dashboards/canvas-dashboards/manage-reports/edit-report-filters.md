---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布控制面板中編輯報告篩選器
description: 報告篩選器套用至畫布控制面板後，您就可以編輯這些篩選器。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 5205c342-7f63-438e-97c8-e74f7dfecfd0
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 9%

---

# 在畫布控制面板中編輯報告篩選器

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>&#x200B;>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>&#x200B;>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

將報表篩選器套用至畫布控制面板後，您就可以編輯報表篩選器，以更新專案進度時顯示的資料。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>標準</p> 
<p>規劃</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理儀表板的許可權</p>
  </td> 
  </tr>
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先將篩選器新增至報表，然後才能進行編輯。

## 編輯報告篩選器

>[!NOTE]
>
>有許多可用的設定工具可用來建置和編輯報表篩選器。 如需這些工具的詳細資訊，請參閱本文中的下列章節： [編輯報表篩選器時的考量事項](#considerations-when-editing-a-report-filter)。


{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 在&#x200B;**畫布控制面板**&#x200B;頁面上，按一下包含您要編輯之篩選器的報表右上角的&#x200B;**更多** ![更多圖示](assets/more-icon.png)圖示，然後選取&#x200B;**編輯**。

   ![編輯報告](assets/edit-report-box.png)

1. 在&#x200B;**設定**&#x200B;對話方塊的左側，選取&#x200B;**篩選器**&#x200B;面板。

1. 按一下&#x200B;**編輯篩選器**。

1. 選取您要編輯的欄位或修正因子，然後視需要調整目前的選取專案。

   ![新增條件](assets/add-condition.png)

1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

1. 按一下「**儲存**」。

## 編輯報表篩選器時的注意事項

### 日期型萬用字元篩選變數

日期型萬用字元選項可與任何日期篩選屬性結合使用。 如需有關新增日期型萬用字元至報表的資訊，請參閱文章[使用日期型萬用字元來一般化報表](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

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

| **限定詞** | |
|---|---|
| **b** | 期間開始（沒有指定屬性，預設為一週的開始：星期日） |
| **e** | 期間結束（沒有指定屬性，預設為一週結束：星期六） |

{style="table-layout:auto"}

| **運運算元** | |
|---|---|
| **+** | 將值新增至萬用字元值 |
| **-** | 從萬用字元值中減去值 |

{style="table-layout:auto"}

例如，萬用字元`$$TODAYb+2w`是指「從本週開始的2週」。 萬用字元*`$$NOW+2h`表示「從現在起的2小時」。

### 登入的使用者萬用字元篩選變數

* 篩選使用者`name`屬性時，您將檢視&#x200B;**我（已登入使用者）**&#x200B;選項。

  ![使用者名稱屬性](assets/user-name-attribute.png)

* 篩選群組`name`屬性時，您將檢視要在篩選條件中使用的&#x200B;**我的主群組（登入使用者群組）**&#x200B;和&#x200B;**我的其他群組（登入使用者群組）**&#x200B;選項。

  ![群組名稱屬性](assets/group-name-attribute.png)

* 篩選團隊`name`屬性時，您將檢視&#x200B;**我的預設團隊（已登入使用者團隊）**&#x200B;和&#x200B;**我的其他團隊（已登入使用者團隊）**&#x200B;選項，以便在篩選條件中選擇。

  ![團隊名稱屬性](assets/team-name-attribute.png)


### 參照子物件

其他欄、篩選選項和群組屬性的可用關係通常僅限於Workfront物件階層中較高的物件，或在報表的基本實體物件上具有單一選取範圍。 但有一些例外，包括：

* 專案>任務
* 檔案核准>檔案核准階段
* 檔案核准階段>檔案核准階段參與者

使用上面列出的任何父項至子項關係時，您會在表格中看到連線到父物件的每個子記錄的一列。

### 依欄位型別的欄位運運算元

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
