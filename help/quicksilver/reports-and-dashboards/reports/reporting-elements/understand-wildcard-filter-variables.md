---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: 萬用字元篩選器變數
description: 若在篩選中使用萬用字元，您可以參照一般使用者或日期，而非特定使用者或日期。 如此一來，您建置的元素就會是動態的，而結果會隨著使用元素的前後關聯而改變。
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: d6094d944b7955db8a97b5e1ce0af8cb85f82a9e
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 1%

---

# 萬用字元篩選器變數概觀

<!-- Audited: 12/2023 -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

您可以使用萬用字元來參照一般使用者或日期，而非特定使用者或日期。 如此一來，您建置的元素便為動態元素；結果會根據使用元素的前後關聯而變更。

例如，在專案報告中篩選$$USER.homeGroupID只會擷取和已登入使用者之主群組相關聯的專案。

建立下列元素時，您可以使用篩選變數（也稱為萬用字元）：

<table>
    <tr>
        <td>清單、報表和資源規劃工具中的篩選器</td>
        <td>如需Workfront篩選器的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">篩選器概觀</a>.
</td>
    </tr>
    <tr>
        <td>進階搜尋</td>
        <td>如需進階搜尋的相關資訊，請參閱區段 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">使用進階搜尋</a> 在文章中 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">搜尋Adobe Workfront</a>.
    </tr>
    <tr>
        <td>檢視中的已計算欄</td>
        <td></td>
    </tr>
    <tr>
        <td>檢視中的條件式格式</td>
        <td>如需有關條件式格式的資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">在檢視中使用條件式格式</a>.
    </tr>
    <tr>
        <td>已計算的自訂欄位</td>
        <td>在計算欄中參考巢狀集合時，不支援萬用字元篩選變數。

如需有關計算的自訂欄位和欄的資訊，請參閱文章 <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">計算自訂欄位與計算欄的比較</a>.
</td>
    </tr>
</table>

## 以日期為基礎的萬用字元篩選變數

日期型萬用字元選項可與任何日期篩選屬性結合使用。 如需有關新增日期型萬用字元至報表的資訊，請參閱文章 [使用日期型萬用字元來一般化報表](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

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
   <td> <p>建議您使用此萬用字元建立日期敏感型篩選器，以免在明天、下週或下個月再次建立篩選器。</p> <p>例如，如果您想要顯示今天之前到期的所有任務，您可以在任務篩選中使用下列規則： <em>計劃開始日期少於$$TODAY</em>.</p> <p>$$TODAY一律等於當天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>這類似於$$TODAY萬用字元，但包含目前的日期和時間。 $$NOW等於目前的日期和時間。</p> <p>例如，如果您想顯示截至目前時間提供的所有小時專案，可在小時篩選中使用下列規則來執行： <em>計劃開始日期少於$$NOW</em>.</p> <p>注意：資源規劃工具不支援這個萬用字元。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要指出不同的時段和不同的時間點（未來或過去），您可以將上述萬用字元與下列內容結合：

| 屬性 |   |
|---|---|
| **q** | 行事曆季度 |
| **h** | 小時 |
| **d** | 天 |
| **w** | 週 |
| **m** | 月 |
| **y** | 年 |

{style="table-layout:auto"}

| **限定詞** | |
|---|---|
| **b** | 期間開始（沒有指定屬性，預設為一週的開始：星期日） |
| **è** | 期間結束（沒有指定屬性，預設為一週結束：星期六） |

{style="table-layout:auto"}

| **運運算元** | |
|---|---|
| **+** | 將值新增至萬用字元值 |
| **-** | 從萬用字元值中減去值 |

{style="table-layout:auto"}

例如，萬用字元 `$$TODAYb+2w` 是指「本週初起的2週」。 萬用字元*`$$NOW+2h` 是指「從現在起的2小時」。

## 使用者型萬用字元篩選器變數

>[!IMPORTANT]
>
>如果篩選器或報表包含以使用者為基礎的萬用字元篩選器變數，結果一律會顯示依目前登入的使用者所篩選的資訊。 當您與其他使用者共用這類篩選器或報表時，萬用字元會擷取檢視報表之使用者的資訊。 這兩個使用者會看到不同的結果。
>
>如需有關新增使用者型萬用字元至報表的資訊，請參閱文章 [使用以使用者為基礎的萬用字元來歸納報表](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

您可從下列使用者型變數中選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最常見的使用者型變數為$$USER.ID。 系統會一律傳回登入使用者的ID。 此ID用於識別建立每個物件及其工作指派的使用者。</p> <p>在報告中使用時，此萬用字元會減少您需要在系統中建立的報告數量。 您可以建立一個報告並與多位使用者共用，而結果會根據登入並檢視報告的使用者而改變。</p> <p>例如，若要針對指派給已登入之使用者的所有問題建立報告，您可以在問題篩選器中使用以下規則： <em>指派至的ID等於$$USER.ID</em>.</p> <p>Workfront會在下列內建篩選器中使用此變數：</p> 
    <ul> 
     <li>我的報告</li> 
     <li>我的專案</li> 
     <li>我的任務</li> 
     <li>我的問題</li> 
     <li>我的小時</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>$$USER.categoryID變數是指與登入使用者相關聯的特定自訂表單。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$$USER.accessLevelID變數是指與登入使用者相關聯的存取層級ID。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$$USER.accessLevelRank變數是指與登入使用者相關聯的存取層級排名。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>$$USER.companyID變數是指與登入使用者相關聯的公司。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID變數是指與您的環境相關聯之客戶帳戶的ID。 針對您的環境，此變數只有一個可能的值，且通常僅用於透過API建立整合時。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName變數是指登入使用者的名字。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName變數是指登入使用者的姓氏。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name變數是指登入使用者的全名。</p> <p>注意：   <p>此萬用字元變數僅適用於在文字模式中修改篩選時。 您無法在不支援文字模式的篩選器中使用此萬用字元。 例如，您無法在下列區域的篩選中使用這個萬用字元：</p> 
     <ul> 
      <li> <p>資源規劃工具</p> </li> 
      <li> <p>工作負載平衡器</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID變數是指登入使用者主群組ID。 作為群組管理員，您可以使用此變數來僅篩選屬於主群組使用者的專案。</p> <p>例如，若要檢視財務群組中專案的所有未完成任務，請在任務篩選中使用下列篩選規則：<br><em>專案：群組識別碼等於$$USER.homeGroupID </em><br><em>完成百分比小於100</em></p> <p>若要檢視指派給特定群組（登入使用者的主群組）中個人的所有未完成任務，請在任務篩選中使用以下篩選規則：</p> <p><em>指派給：群組ID等於$$USER.homeGroupID<br>完成百分比小於100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs變數是指與登入使用者設定檔相關聯的所有群組（包括主群組）。</p> <p>此變數的功能與$$USER.homeGroupID變數類似，除了結果會顯示與登入使用者相關聯之任何群組的使用者相關資訊。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID變數是指登入使用者之主團隊ID。 作為團隊經理，您可以使用此變數來僅篩選屬於您的主團隊中的使用者的專案。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs變數會傳回與登入使用者相關聯的所有團隊清單。</p> <p>此變數的功能與$$USER.homeTeamID變數類似，除了結果會顯示屬於篩選中所識別之任何團隊之使用者的相關資訊。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID變數是指登入使用者的主要角色。 使用此變數，您可以報告指派給特定工作角色的任務或問題。</p> <p>例如，若要檢視指派給登入使用者之主要角色的所有任務，您可以在任務篩選中使用以下篩選規則：</p> <p><em>任務：角色ID等於$$USER.roleID。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>$$USER.roleIDs變數是指與登入使用者相關聯的所有工作角色。 使用此變數，您可以報告指派給與登入使用者相關聯之任何工作角色的任務或問題。 </p> <p>例如，若要檢視指派給與登入使用者相關聯之任何角色的所有任務，您可以在任務篩選中使用以下篩選規則：</p> <p><i>任務：角色ID等於$$USERID.roleIDs<br></i> </p> <p>秘訣： <i>任務：角色ID等於$$USERID.roleIDs</i> 篩選器規則存在於內建篩選器中「我的角色中的未指派任務」和「我的角色中的未指派問題」。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 物件式萬用字元篩選變數

您可以從下列物件式萬用字元中選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE變數是指物件的型別。 </p> 
     <p>在自訂表單中，當表單的選定物件型別與計算自訂欄位中參照的欄位不相容時，您可以使用此萬用字元來避免為這些物件型別建立重複表單的因應措施。</p> 
     <p>在計算自訂欄位中，做法是在IF運算式中加入萬用字元，讓計算可以為表單的每個物件型別輸出不同的值。 </p> 
     <p>如需詳細資訊和範例，請參閱區段 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">多物件自訂表單中的已計算自訂欄位</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">新增計算資料至自訂表單</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
