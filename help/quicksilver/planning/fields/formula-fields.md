---
title: 公式欄位概觀
description: 在Adobe Workfront Planning中，您可以建立公式欄位，這些欄位使用函式和現有欄位來計算新的自訂值。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 5%

---

# 公式欄位概觀

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中建立自訂欄位，方法是參照現有欄位並在公式型別欄位中連線它們。

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱文章[建立欄位](/help/quicksilver/planning/fields/create-fields.md)中的「公式」一節。

<!--do we need these for an overview article?

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and any Planning package</p>
<p>Any Workflow and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

-->

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## 有關公式欄位的考量事項

* 公式欄位參考屬於相同記錄型別的欄位。
* 只有在您將其他記錄型別連線到要為其建立公式欄位的記錄型別時，才能引用其他記錄型別的欄位。
* 在公式中參考連線的記錄型別或其查閱欄位，取決於您對連線的記錄型別的許可權。 如果您沒有檢視記錄型別的許可權，則無法在公式中參考其欄位。
* 儲存公式欄位後，您無法變更其欄位型別。
* 儲存公式欄位後，您可以更新公式欄位的計算，而計算結果會自動更新相同型別的所有記錄。
* 您必須在Workfront Planning介面中顯示的公式中，新增您參考的欄位。
* 您只能參考顯示在記錄型別表格檢視或記錄詳細資訊頁面上的欄位。
* 您可以從下列格式選項中選擇，以定義公式計算值的格式：

   * 文字
   * 數字
   * 百分比
   * 貨幣
   * 標記
   * 日期

  如需詳細資訊，請參閱文章[建立欄位](/help/quicksilver/planning/fields/create-fields.md)中的「公式」一節。
* 您可以在新的公式中參考公式欄位。 在公式欄位中參照的欄位中更新值後，參照該欄位的所有後續欄位或包含該欄位的公式欄位將自動更新。

* 當您更新公式欄位或可能影響它的欄位時，警示會通知您變更的影響。 警示會顯示在下列情況中：

   * 當您更新公式欄位時（不包括名稱和說明變更），如果該欄位具有相依公式或查閱欄位。 警示會列出這些相依欄位，並詢問您是否要繼續。

   * 當您刪除用於公式運算式或作為查閱欄位的欄位時。 警示會列出相依公式和查閱欄位，並詢問您是否要繼續刪除。

## 公式欄位的限制

* 您最多可以為一個記錄型別新增20個公式欄位。

  從連線的記錄型別新增的公式查閱欄位不會計入此限制。

* 公式運算式不可超過50,000個字元。

* 公式欄位在下列情況下可能會顯示為`#ERROR!`：
   * 刪除公式中使用的欄位時。
   * 當彙總查閱欄位中使用的欄位顯示為`#ERROR!`時。

     例如，如果您顯示包含彙總查閱公式欄位的查閱欄位，且其中一個參考的公式欄位會顯示為`#ERROR!`。
   * 當公式值無法以選取的格式顯示時。

     例如，如果我為公式欄位的「格式」選取「數字」，而公式中使用的欄位是隻顯示非數字文字值的文字欄位，則公式結果將顯示為`#ERROR!`，因為它無法將文字解析為數字。


## 支援的公式

Adobe Workfront Planning公式欄位支援Workfront計算欄位的大部分運算式。

>[!NOTE]
>
>Workfront Planning公式欄位不支援下列Workfront運算式：
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* 格式

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

如需Workfront運算式的完整清單，請參閱[計算資料運算式概觀](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

此外，我們為Workfront Planning公式欄位支援下列運算式。 Workfront運算式不支援下列運算式：

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>說明和範例</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>傳回依分隔字元的串連字串。</p> <p>運算式的格式如下：

<code>ARRAYJOIN（分隔字元，陣列）</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>傳回具有唯一值的陣列。</p> <p>運算式的格式如下：

<code>ARRAYUNIQUE（陣列）</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>識別碼</strong> </td> 
   <td> <p>傳回記錄的ID。 每個記錄都有一個唯一的ID。</p> <p>運算式的格式如下：

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>由提供的JSONPath從JSON傳回資料。 如果JSON中不存在JSONPath，則會傳回空白結果。 </p> <p>運算式的格式如下：
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>將日期和時間的時區設定為特定時區。</p> <p>運算式的格式如下：

<code>SETTIMEZONE（日期，&#39;美洲/洛杉磯&#39;）</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>傳回一年中的週數。或者，您可以指定一週從星期幾開始 (使用 1 表示星期日，或使用 2 表示星期一)。如果省略，則會依預設從星期日開始。</p> <p>運算式的格式如下：

<code>WEEKOFYEAR（日期，2）</code>
或
<code>WEEKOFYEAR（日期）</code>
</p>
   </td></tr>

</table>
