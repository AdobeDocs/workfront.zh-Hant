---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文字模式編輯篩選器
description: '注意：在本文新增章節：/Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html;***此外，在文本模式概述文章中起草此區域)'
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# 使用文字模式編輯篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

您可以使用文字模式編輯清單或報表中的篩選器，以存取標準介面中無法使用的欄位，並建立更複雜的篩選器。

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
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的報表元素</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限以編輯報表中的篩選器</p> <p>管理篩選器的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始在報表或清單中使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在篩選器中編輯文字模式

使用文字模式編輯篩選器對報表和清單是相同的。 從報表或清單存取檢視的方式有所不同。

>[!TIP]
>
>建議您在標準模式中盡可能多地建立篩選器，然後將篩選器轉換為文字模式加以編輯。

如需建立篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 執行下列任一項作業：

   1. 若要從報表存取篩選器，請前往報表，然後按一下 **報表動作** > **編輯** > **篩選器** 標籤。
   1. 若要從清單存取篩選器，請前往清單，然後從 **篩選** 下拉式選單中，將滑鼠移至您要修改的篩選器上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

      篩選器產生器隨即開啟。

1. 按一下 **新增篩選規則** 若要開始新增篩選條件，請按一下 **切換到文本模式** 建立器的右上角。
1. 使用文本模式添加篩選語句。 每個篩選語句可包含以下行和附加資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>篩選行/資訊</td> 
      <td>範例</td> 
     </tr> 
     <tr> 
      <td> <p>欄位名稱及其等於的值，在Workfront資料庫中顯示時。</p> <p>此行是必填的。</p> <p> 有關對象和欄位在資料庫中如何顯示的詳細資訊，請參見 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>要篩選狀態為「正在進行」的任務，請使用以下行：</p> <p><code>status=INP</code> </p> <p>提示：篩選狀態時，您必須使用狀態的三字母代碼，而非名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>欄位名稱修飾詞，以及修飾詞等於的。 這表示您要篩選的欄位必須滿足哪些條件。</p> <p>此行是必填的。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>要指示您為篩選的任務的狀態必須等於「正在進行」，請使用以下行以及上面的行：</p> <p><code>status_Mod=in</code> </p> <p>如果修改量是範圍，則有兩行用於指示修改量。</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>範例: </b></span></span> 
        <p>這是文字模式篩選器，會尋找進行中、在當月內有計畫完成日期、且指派給具有特定GUID的使用者的工作：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>如需文字模式中的篩選修飾詞完整清單，請參閱文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選條件修飾元</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>語句運算子。 依預設，每個篩選陳述式都以"AND"運算子連結。 這不會顯示在文字模式介面中。 您也可以在兩個陳述式之間新增「OR」運算子，以指出您要篩選可滿足兩個條件之一或另一個的物件。</p> <p>只有具有多個語句的篩選器才需要篩選器運算子。</p> <p>提示：   
        <ul> 
         <li> <p>「OR」區分大小寫，且必須一律大寫。</p> </li> 
         <li> <p>當您將運算子從AND變更為OR時，清單項目數可能會增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>範例: </b></span></span> 
        <p>要篩選狀態為「正在進行」或「計畫完成日期為今天」的任務，請使用以下選項： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>萬用字元可讓您歸納篩選器中的資訊，並參考目前時間或登入的使用者。</p> <p>萬用字元是選用的。</p> <p>提示：   <p>建議您盡可能使用萬用字元(*)，讓您的篩選器更具動態性，且不要為每個使用者或類似的時間範圍複製相同的篩選器。</p> <p>如需篩選萬用字元的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">萬用字元篩選變數</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>範例: </b></span></span> 
        <p>若要篩選指派給目前登入之使用者的任務，請使用下列項目：</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 要添加由&quot;OR&quot;運算子連接的篩選語句，請執行以下操作：

   1. 新增一行程式碼，並輸入OR:1: 後面接著您要篩選的物件或屬性，以及您要與其比較的值。 要引用除「新建」之外處於任何狀態的任務，請使用以下行：

      ```
      OR:1:status=NEW
      ```

   1. 添加第二行並鍵入OR:1: 後面接著物件、修飾詞和修飾詞代碼。 要為代碼行定義修改量，以引用除「新建」之外的所有任務狀態，請使用以下修改量行：

      ```
      OR:1:status_Mod=notin
      ```

      新語句的每行前面都必須加上「OR:`<number>`：」。

      如需在篩選器中建立「OR」陳述式的詳細資訊，請參閱 [在文字模式篩選器中建立「OR」陳述式](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>同一個篩選器中可以有多個「OR」陳述式。 每次您有新的「OR」陳述式時，「OR：」之後的數字就會增加。
要篩選狀態為「正在進行」或已分配給登錄用戶或具有今天計畫完成日期的任務，請使用以下選項：
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. 按一下 **完成** 如果您想要儲存變更並繼續編輯報表或篩選器。
1. 按一下 **儲存+關閉** 儲存報表或 **儲存篩選** 將篩選器儲存在清單中。
