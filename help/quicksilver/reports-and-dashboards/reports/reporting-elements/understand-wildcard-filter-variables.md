---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: 萬用字元篩選變數
description: 在篩選器中使用萬用字元，可以參照一般使用者或日期，而非特定使用者或日期。 如此一來，您建置的元素就會動態顯示，結果會隨使用內容而改變。
author: Lisa
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 2%

---

# 萬用字元篩選變數

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

Adobe Workfront在建立下列元素時支援篩選變數或萬用字元：

* 清單、報表和資源計畫員中的篩選器

   如需Workfront篩選器的相關資訊，請參閱文章 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 進階搜尋

   如需進階搜尋的相關資訊，請參閱區段 [使用進階搜尋](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) 在文章中 [搜尋Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* 檢視中的計算欄
* 視圖中的條件式格式

   如需條件式格式的相關資訊，請參閱文章 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* 計算自訂欄位

   >[!NOTE]
   >
   >在計算欄中參考巢狀集合時，不支援萬用字元篩選變數。

   如需計算自訂欄位和欄的相關資訊，請參閱文章 [計算自訂欄位與計算欄](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

使用萬用字元，您可以參照一般使用者或日期，而非特定使用者或日期。 如此一來，您建置的元素就會動態顯示，結果會隨使用內容而改變。

例如，在項目報表中篩選$$USER.homeGroupID時，只會擷取與已登入之使用者的「首頁群組」相關聯的專案。

您可以在Workfront中使用日期型或使用者型篩選變數。

## 日期型萬用字元篩選變數

Workfront日期型萬用字元選項可與任何日期篩選屬性搭配使用。

如需新增日期型萬用字元至報表的相關資訊，請參閱文章 [使用日期型萬用字元來歸納報表](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>如果您建立的日期和時間計算不含時間部分，或使用日期通配符$$TODAY或$$NOW，則系統會根據協調通用時間(UTC)區域使用日期，而不是根據您的本地時區。 這可能會造成非預期的日期結果。

從下列日期型萬用字元中選擇：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>今天$</strong> </p> </td> 
   <td> <p>建議您使用此萬用字元建立日期敏感篩選器，以免明天、下週或下月再次建立篩選器。</p> <p>例如，如果要顯示今天之前到期的所有任務，則可以在任務篩選器中使用以下規則： <em>計劃開始日期少於$$TODAY</em>.</p> <p>$TODAY始終等於當天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$NOW</strong> </p> </td> 
   <td> <p>這類似於$TODAY通配符，但包括當前日期和時間。 $$NOW等於當前日期和時間。</p> <p>例如，如果要顯示截至當前時間提供的所有小時條目，則可以在小時過濾器中使用以下規則來執行此操作： <em>計劃開始日期小於$NOW</em>.</p> <p>注意：資源規劃器不支援此通配符。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要指出各個時段和各個時間點（未來或過去），您可以結合萬用字元(*)與下列項目：

| 屬性 |   |
|---|---|
| **q** | 日曆季 |
| **h** | 小時 |
| **d** | 日 |
| **w** | 週 |
| **m** | 月 |
| **y** | 年 |

{style=&quot;table-layout:auto&quot;}

| **限定符** |  |
|---|---|
| **b** | 一週的開始（星期日） |
| **e** | 一週結束（星期六） |

{style=&quot;table-layout:auto&quot;}

| **運算子** |  |
|---|---|
| **+** | 將值新增至萬用字元值 |
| **-** | 從萬用字元中減去值 |

{style=&quot;table-layout:auto&quot;}

例如，萬用字元 `$$TODAYb+2w` 是指「從本週開始算起2週」。 萬用字元*`$$NOW+2h` 是指「2小時後」

## 基於用戶的通配符篩選變數

>[!IMPORTANT]
>
>如果篩選器或報表包含以使用者為基礎的萬用字元篩選變數，結果一律會顯示目前登入之使用者所篩選的資訊。 當您與其他使用者共用此類篩選器或報表時，萬用字元會為查看報表的使用者擷取資訊。 兩個使用者會看到不同的結果。

如需新增使用者型萬用字元至報表的相關資訊，請參閱文章 [使用以使用者為基礎的萬用字元來歸納報表](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront提供下列使用者型變數：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最常見的使用者型變數為$$USER.ID。 這一律會傳回登入使用者的ID。 這是用於標識建立每個對象的用戶及其工作分配的ID。</p> <p>在報表中使用時，此萬用字元會減少您在系統中需要建立的報表數量。 您可以建立一個報表並與數個使用者共用，結果會根據登入者和查看報表而有所變更。</p> <p>例如，若要針對指派給已登入使用者的所有問題建立報表，您可以在問題篩選器中使用下列規則： <em>指派給ID等於$$USER.ID</em>.</p> <p>Workfront會在下列內建篩選器中使用此變數：</p> 
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
   <td> <p>$$USER.categoryID變數會參照與登入使用者相關聯的特定自訂表單。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$$USER.accessLevelID變數會參照與登入使用者相關聯的存取層級ID。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$$USER.accessLevelRank變數引用與登錄用戶關聯的訪問級別排名。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>$$USER.companyID變數會參照與登入使用者相關聯的公司。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID變數會參照與您的環境相關聯的客戶帳戶ID。 針對您的環境，此變數只有一個可能的值，且通常僅用於透過API建置整合時。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName變數會參照登入使用者的名字。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName變數引用登錄用戶的姓氏。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name變數會參照登入使用者的完整名稱。</p> <p>備註:   <p>此萬用字元變數僅適用於以文字模式修改篩選器時。 您無法在不支援文字模式的篩選器中使用此萬用字元。 例如，您無法在下列區域的篩選器中使用此萬用字元：</p> 
     <ul> 
      <li> <p>資源規劃工具</p> </li> 
      <li> <p>工作負載平衡器</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID變數會參照登入使用者之首頁群組的ID。 身為群組管理員，您可以使用此變數僅篩選屬於您首頁群組使用者的項目。</p> <p>例如，要查看財務組中項目上所有未完成的任務，請在任務篩選器中使用以下篩選規則：<br><em>專案：組ID等於$USER.homeGroupID </em><br><em>完成百分比小於100</em></p> <p>要查看指定組（即登錄用戶的主組）中分配給個人的所有未完成任務，請在任務篩選器中使用以下篩選規則：</p> <p><em>指派給：組ID等於$USER.homeGroupID<br>完成百分比小於100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs變數會參照與已登入使用者設定檔相關聯的所有群組（包括首頁群組）。</p> <p>此變數的功能與$$USER.homeGroupID變數的功能類似，除了結果會顯示屬於與登入使用者相關聯的任何群組之使用者的相關資訊以外。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID變數會參照登入使用者之主團隊的ID。 身為團隊經理，您可以使用此變數僅篩選屬於您首頁團隊使用者的項目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs變數會傳回與登入使用者相關聯的所有團隊清單。</p> <p>此變數的功能與$$USER.homeTeamID變數的功能類似，除了結果會顯示屬於篩選器中所識別任何團隊之使用者的相關資訊以外。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID變數會參照登入使用者的主要角色。 使用此變數，您可以報告指派給特定作業角色的任務或問題。</p> <p>例如，要查看分配給登錄用戶的「主角色」的所有任務，可以在任務篩選器中使用以下篩選規則：</p> <p><em>任務：角色ID等於$USER.roleID。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>$$USER.roleIDs變數會參照與登入使用者相關聯的所有工作角色。 使用此變數，您可以報告指派給與登入使用者相關聯的任何工作角色的任務或問題。 </p> <p>例如，要查看分配給與登錄用戶關聯的任何角色的所有任務，可以在任務篩選器中使用以下篩選規則：</p> <p><i>任務：角色ID等於$$USERID.roleIDs<br></i> </p> <p>提示：此 <i>任務：角色ID等於$$USERID.roleIDs</i> 篩選器規則存在於內建篩選器中「我的角色中未指派的任務」和「我的角色中未指派的問題」。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 物件型萬用字元篩選變數

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE變數會參照物件的類型。 </p> 
     <p>在自訂表單中，當表單的所選對象類型與計算的自訂欄位中引用的欄位不相容時，您可以使用此萬用字元來避免為這些對象類型建立重複表單的解決方法。</p> 
     <p>在計算的自訂欄位中，您可將萬用字元加入IF運算式中，以便計算能針對每個表單的物件類型輸出不同的值。 </p> 
     <p>如需詳細資訊和範例，請參閱區段 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">多物件自訂表單中的計算自訂欄位</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">將計算資料新增至自訂表單</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
