---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文字模式編輯篩選器
description: 您可以使用文字模式在清單或報告中編輯篩選器，以存取標準介面中無法使用的欄位，並建立更複雜的篩選器。
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# 使用文字模式編輯篩選器

<!-- Audited: 1/2025 -->

您可以使用文字模式在清單或報告中編輯篩選器，以存取標準介面中無法使用的欄位，並建立更複雜的篩選器。

如需建立篩選時的更多文字模式範例，另請參閱文章[自訂檢視、篩選和群組範例：文章索引](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters)中的[自訂篩選範例](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)一節。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
     <p>標準</p>
     <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視和群組的存取權</p> <p>編輯報告、儀表板和行事曆的存取權，以編輯報告中的報告元素</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權，以編輯報表中的篩選器</p> <p>管理篩選器的許可權以編輯它</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

如需建立篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 執行下列其中一項：

   若要從清單存取篩選器，請移至清單並按一下&#x200B;**篩選器**&#x200B;圖示，然後將游標移至您要修改之&#x200B;**篩選器**&#x200B;側面板中的篩選器，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。 **篩選器**&#x200B;側面板會顯示您選取的篩選器，或舊版篩選器產生器開啟。

   或

   若要從報告存取篩選器，請移至報告，然後按一下&#x200B;**報告動作** > **編輯** > **篩選器**&#x200B;索引標籤。

1. 執行下列其中一項：

   如果您在清單上使用&#x200B;**篩選器**&#x200B;側面板，請按一下&#x200B;**文字模式**。

   或

   如果您使用舊版篩選產生器或報表，請按一下&#x200B;**新增篩選規則**&#x200B;以開始新增篩選條件。 然後，按一下產生器右側的&#x200B;**切換至文字模式**&#x200B;然後&#x200B;**編輯文字模式**。

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
      <td> <p>欄位名稱及其在Workfront資料庫中顯示的值。</p> <p>此為必填欄位。</p> <p> 如需有關物件和欄位如何在資料庫中顯示的詳細資訊，請參閱<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>若要篩選狀態為「進行中」的任務，請使用以下行：</p> <p><code>status=INP</code> </p> <p><b>秘訣</b>

   篩選狀態時，您必須使用狀態的三個字母代碼，而不是名稱。</p> </td>
   </tr> 
     <tr> 
      <td> <p>欄位名稱修飾元以及修飾元等於。 這表示您用來篩選的欄位必須符合哪些條件。</p> <p>此為必填欄位。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>若要指出您篩選的任務狀態必須等於進行中，請使用上述行以外的下列行：</p> <p><code>status_Mod=in</code> </p> <p>如果修正因子為範圍，則有兩個明細行可表示修正因子。</p> 
       <div> <span class="autonumber"><span><b>範例</b></span></span> 
        <p>這是文字模式篩選器，會尋找進行中的任務、具有本月內計畫完成日期的任務，並指派給具有特定GUID的使用者：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>如需文字模式中篩選修飾元的完整清單，請參閱文章<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選和條件修飾元</a>。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>陳述式運運算元。 依預設，每個篩選陳述式都由「AND」運運算元連線。 這不會顯示在文字模式介面中。 您也可以在兩個陳述式之間新增「OR」運運算元，以表示您要篩選滿足兩個條件中其中一個的物件。</p> <p>只有含有多個陳述式的篩選器才需要篩選器運運算元。</p> <p>秘訣：   
        <ul> 
         <li> <p>「或」區分大小寫，且必須一律大寫。</p> </li> 
         <li> <p>當您將運運算元從AND變更為OR時，清單專案的數量可能會增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>範例</b></span></span> 
        <p>若要篩選處於進行中狀態或計畫完成日期為今天的任務，請使用下列專案： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>萬用字元，可讓您一般化篩選器中的資訊，並參照目前時間或登入的使用者。</p> <p>萬用字元為選用。</p> <p>秘訣：   <p>建議您儘可能使用萬用字元，讓您的篩選器更動態，而且每個使用者或類似的時間範圍都不需重複相同的篩選器。</p> <p>如需有關篩選萬用字元的資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">萬用字元篩選變數概觀</a>。</p> </p> </td> 
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

   1. 新增一行程式碼和型別OR:1:，後面接著您要篩選的物件或屬性，以及您要用來比較的值。 若要參照任何狀態（「新增」除外）的任務，請使用下列行：

      `OR:1:status=NEW`

   1. 新增第二行並輸入OR:1:，後面接著物件、修飾元和修飾元程式碼。 若要定義代碼明細行的修正因子，以參考除「新增」以外的所有作業狀態，請使用下列修正因子明細行：

      `OR:1:status_Mod=notin`

      新陳述式的每一行前面都必須加上「OR：`<number>`：」。

      如需有關在篩選中建立「OR」陳述式的資訊，請參閱[在文字模式篩選中建立「OR」陳述式](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md)。

      >[!NOTE]
      >
      >同一個篩選器中可以有多個「OR」陳述式。 每當您有新的「OR」陳述式時，「OR：」之後的數字就會增加。
      >
      >若要篩選狀態為「進行中」、已指派給登入使用者或具有「規劃完成日期」當天的任務，請使用下列專案：
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. 按一下「**套用**」或「**完成**」以儲存文字模式變更，並繼續編輯報告或篩選器。
1. 按一下&#x200B;**儲存+關閉**&#x200B;以儲存您的報告，或按一下&#x200B;**儲存篩選器**&#x200B;以將篩選器儲存在清單中。


