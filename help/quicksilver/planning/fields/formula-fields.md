---
title: 公式欄位概觀
description: 在Adobe Workfront Planning中，您可以建立公式欄位，這些欄位使用函式和現有欄位來計算新的自訂值。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: d7af8c5888147e847b4e239b629373b4b72541f7
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 4%

---

# 公式欄位概觀

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中建立自訂欄位，方法是參照現有欄位並在公式型別欄位中連線它們。

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱文章[建立欄位](/help/quicksilver/planning/fields/create-fields.md)中的「公式」一節。

## 存取需求

+++ 展開以檢視存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選擇</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區與記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr>

</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

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

<div class="preview">

* 當您更新公式欄位或可能影響它的欄位時，警示會通知您變更的影響。 警示會顯示在下列情況中：

   * 當您更新公式欄位時（不包括名稱和說明變更），如果該欄位具有相依公式或查閱欄位。 警示會列出這些相依欄位，並詢問您是否要繼續。

   * 當您刪除用於公式運算式或作為查閱欄位的欄位時。 警示會列出相依公式和查閱欄位，並詢問您是否要繼續刪除。

</div>



<div class="preview">

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

</div>

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
