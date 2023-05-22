---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式編輯篩選器
description: 「注意：在本文中添加一節：/內容/報告和儀表板/報告/報告Elements/create-customize-fitlers.html;***此外，在文本模式概述文章中草擬此區域)
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: be47bc4da5e3921a7c36e19831acde91aad55db1
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# 使用文本模式編輯篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

可以使用文本模式在清單或報表中編輯篩選器，以訪問標準介面中不可用的欄位並建立更複雜的篩選器。

有關建立篩選器時的更多文本模式示例，另請參閱文章中的「自定義篩選器的示例」一節 [自定義視圖、篩選器和分組示例](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的報表元素</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限以編輯報表中的篩選器</p> <p>管理篩選器的權限以編輯它</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 先決條件

開始在報表或清單中使用文本模式之前，請始終確保您熟悉Workfront文本模式語法。

有關詳細資訊，請參閱：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式語法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定義視圖、篩選器和分組示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在篩選器中編輯文本模式

使用文本模式編輯篩選器對於報告和清單是相同的。 從報表或清單訪問篩選器的方式不同。

>[!TIP]
>
>我們建議您在標準模式下盡可能多地構建過濾器，然後將過濾器轉換為文本模式以編輯它。

有關生成篩選器的詳細資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

有關建立報告的資訊，請參見 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 執行下列任一項作業：

   1. 要從報表訪問篩選器，請轉到報表，然後按一下 **報告操作** > **編輯** > **篩選器** 頁籤。
   1. 要從清單訪問篩選器，請轉到清單和 **篩選** 下拉菜單，將滑鼠移到要修改的篩選器上，然後按一下 **編輯** 表徵圖 ![](assets/edit-icon.png)。

      篩選器生成器開啟。

1. 按一下 **添加篩選器規則** 要開始添加篩選器的條件，請按一下 **切換到文本模式** 在生成器的右上角。
1. 使用文本模式添加篩選器語句。 每個篩選器語句可能包含以下行和附加資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>篩選行/資訊</b></td> 
      <td><b>範例</b></td> 
     </tr> 
     <tr> 
      <td> <p>欄位名稱及其等於的值(在Workfront資料庫中顯示)。</p> <p>此行是必填項。</p> <p> 有關對象和欄位在資料庫中的顯示方式的詳細資訊，請參見 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API資源管理器</a>。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>要篩選狀態為「正在進行」的任務，請使用以下行：</p> <p><code>status=INP</code> </p> <p><b>提示</b>

   篩選狀態時，必須使用狀態的三字母代碼，而不是名稱。</p> </td>
   </tr> 
     <tr> 
      <td> <p>欄位名稱修飾符和修飾符的等於項。 這表示要篩選的欄位必須滿足哪些條件。</p> <p>此行是必填項。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>要指示篩選的任務的狀態必須等於「正在執行」，除上面的行外，還請使用以下行：</p> <p><code>status_Mod=in</code> </p> <p>如果修改量是一個範圍，則有兩行可指示修改量。</p> 
       <div> <span class="autonumber"><span><b>示例 </b></span></span> 
        <p>這是一個文本模式篩選器，它查找在當月內具有計畫完成日期且分配給具有特定GUID的用戶的正在執行的任務：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>有關文本模式下的篩選器修飾符的完整清單，請參閱文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選器和條件修飾符</a>。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>語句運算子。 預設情況下，每個filter語句都由「AND」運算子連接。 這不會顯示在文本模式介面中。 還可以在兩個語句之間添加一個「OR」運算子，以指示要篩選滿足兩個條件中一個或另一個條件的對象。</p> <p>只有具有多個語句的篩選器才需要篩選器運算子。</p> <p>提示：   
        <ul> 
         <li> <p>「OR」區分大小寫，必須始終大寫。</p> </li> 
         <li> <p>將運算子從AND更改為OR時，清單項數可能會增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>示例 </b></span></span> 
        <p>要篩選狀態為「正在進行」或「計畫完成日期為今天」的任務，請使用以下命令： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>通配符，允許您泛化篩選器中的資訊並引用當前時間或登錄的用戶。</p> <p>通配符是可選的。</p> <p>提示：   <p>我們建議盡可能使用通配符，使篩選器更具動態性，並且不要為每個用戶或類似的時間幀複製相同的篩選器。</p> <p>有關篩選通配符的資訊，請參見 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">通配符篩選器變數</a>。</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>示例</b></span></span> 
        <p>要篩選分配給當前登錄用戶的任務，請使用以下命令：</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 要添加由&quot;OR&quot;運算子連接的篩選器語句，請執行以下操作：

   1. 添加新的代碼行並鍵入OR:1: 後跟要篩選的對象或屬性以及要與之比較的值。 要引用除「新建」之外處於任何狀態的任務，請使用以下行：

      ```
      OR:1:status=NEW
      ```

   1. 添加第二行並鍵入OR:1: 後跟對象、修飾符和修飾符代碼。 要為代碼行定義修改量，該代碼行引用除「新建」之外的所有任務狀態，請使用以下修改量行：

      ```
      OR:1:status_Mod=notin
      ```

      新語句的每行前必須有「OR:`<number>`:&quot;

      有關在篩選器中建立「OR」語句的資訊，請參見 [在文本模式篩選器中建立&quot;OR&quot;語句](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md)。

<!--WRITER - reformat note below -->

>[!NOTE]
>
>可以在同一篩選器中包含多個「OR」語句。 每次您有新的&quot;OR&quot;語句後，&quot;OR:&quot;後的數字都會增加。
要篩選狀態為「正在進行」或已分配給已登錄用戶或具有今天計畫完成日期的任務，請使用以下命令：
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. 按一下 **完成** 的子菜單。
1. 按一下 **保存+關閉** 保存報表或 **保存篩選器** 框中選擇自定義樣式。


