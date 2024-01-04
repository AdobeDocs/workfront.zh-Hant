---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文字模式編輯篩選器
description: '注意：在文章中新增區段：/Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html；***此外，在文字模式概觀文章中草稿此區域)'
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# 使用文字模式編輯篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

您可以使用文字模式在清單或報告中編輯篩選器，以存取標準介面中無法使用的欄位，並建立更複雜的篩選器。

如需建立篩選時的更多文字模式範例，另請參閱文章中的「自訂篩選的範例」一節 [自訂檢視、篩選和分組範例：文章索引](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的報告元素</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權，以編輯報表中的篩選器</p> <p>管理篩選器的許可權以編輯它</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 先決條件

在報表或清單中開始使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在篩選器中編輯文字模式

對於報告和清單，使用文字模式編輯篩選器是相同的。 從報表或清單存取篩選器會有所不同。

>[!TIP]
>
>建議您在標準模式中建立儘可能多的篩選器，然後將篩選器轉換為文字模式以進行編輯。

如需建立篩選器的詳細資訊，請參閱 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 執行下列其中一項：

   1. 若要從報表存取篩選器，請移至報表，然後按一下 **報表動作** > **編輯** > **篩選器** 標籤。
   1. 若要從清單存取篩選器，請移至清單並從 **篩選** 下拉式選單，將滑鼠移至您要修改的篩選器上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

      篩選產生器隨即開啟。

1. 按一下 **新增篩選器規則** 若要開始新增篩選條件，請按一下 **切換到文字模式** 建立器的右上角。
1. 使用文字模式新增篩選陳述式。 每個篩選陳述式都可包含下列各行及其他資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>篩選器行/資訊</b></td> 
      <td><b>範例</b></td> 
     </tr> 
     <tr> 
      <td> <p>欄位名稱及其在Workfront資料庫中顯示的值。</p> <p>此為必填欄位。</p> <p> 如需有關物件和欄位如何在資料庫中顯示的詳細資訊，請參閱 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>若要篩選狀態為「進行中」的任務，請使用以下行：</p> <p><code>status=INP</code> </p> <p><b>秘訣</b>

   篩選狀態時，您必須使用狀態的三個字母代碼，而不是名稱。</p> </td>
   </tr> 
     <tr> 
      <td> <p>欄位名稱修飾詞以及修飾詞所代表的內容。 這表示您正在篩選的欄位必須符合哪些條件。</p> <p>此為必填欄位。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>若要指出您篩選的任務狀態必須等於進行中，請使用上述行以外的下列行：</p> <p><code>status_Mod=in</code> </p> <p>如果修正因子為範圍，則有兩個明細行可表示修正因子。</p> 
       <div> <span class="autonumber"><span><b>範例 </b></span></span> 
        <p>這是文字模式篩選器，會尋找進行中的任務、具有本月內計畫完成日期的任務，並指派給具有特定GUID的使用者：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>如需文字模式中篩選修飾元的完整清單，請參閱文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選和條件修飾元</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>陳述式運運算元。 依預設，每個篩選陳述式都由「AND」運運算元連線。 這不會顯示在文字模式介面中。 您也可以在兩個陳述式之間新增「OR」運運算元，以表示您要篩選滿足兩個條件中其中一個的物件。</p> <p>只有含有多個陳述式的篩選器才需要篩選器運運算元。</p> <p>秘訣：   
        <ul> 
         <li> <p>「或」區分大小寫，且必須一律大寫。</p> </li> 
         <li> <p>當您將運運算元從AND變更為OR時，清單專案的數量可能會增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>範例 </b></span></span> 
        <p>若要篩選處於進行中狀態或計畫完成日期為今天的任務，請使用下列專案： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>萬用字元，可讓您一般化篩選器中的資訊，並參照目前時間或登入的使用者。</p> <p>萬用字元為選用。</p> <p>秘訣：   <p>建議您儘可能使用萬用字元，讓您的篩選器更動態，而且每個使用者或類似的時間範圍都不需重複相同的篩選器。</p> <p>如需有關篩選器萬用字元的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">萬用字元篩選器變數</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>範例</b></span></span> 
        <p>若要篩選指派給目前登入之使用者的工作，請使用下列專案：</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 若要新增由「OR」運運算元連線的篩選陳述式，請執行下列動作：

   1. 新增一行程式碼並輸入OR:1: 後面接著您要篩選的物件或屬性，以及您要用來比較的值。 若要參照任何狀態（「新增」除外）的任務，請使用下列行：

      ```
      OR:1:status=NEW
      ```

   1. 新增第二行並輸入OR:1: 後面接著物件、修飾元和修飾元程式碼。 若要定義代碼明細行的修正因子，以參考除「新增」以外的所有作業狀態，請使用下列修正因子明細行：

      ```
      OR:1:status_Mod=notin
      ```

      新陳述式的每一行前面都必須加上「或：`<number>`：&quot;。

      如需有關在篩選中建立「OR」陳述式的資訊，請參閱 [在文字模式篩選器中建立「OR」陳述式](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>同一個篩選器中可以有多個「OR」陳述式。 每次有新的「OR」陳述式時，「OR：」之後的數字都會增加。
>
若要篩選狀態為「進行中」、已指派給登入使用者或具有「規劃完成日期」當天的任務，請使用下列專案：
>
`status=INP`
>
`status_Mod=in`
>
`OR:1:assignedToID=$$USER.ID`
>
`OR:1:assignedToID_Mod=in`
>
`OR:2:plannedCompletionDate=$$TODAY`
>
`OR:2:plannedCompletionDate_Mod=eq`

1. 按一下 **完成** 如果要儲存變更並繼續編輯報告或篩選器。
1. 按一下 **儲存+關閉** 儲存報告或 **儲存篩選器** 將篩選器儲存在清單中。


