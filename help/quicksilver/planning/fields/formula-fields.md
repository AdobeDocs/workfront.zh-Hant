---
title: 公式欄位概觀
description: 在Adobe Workfront Planning中，您可以建立公式欄位，這些欄位使用函式和現有欄位來計算新的自訂值。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 7%

---

# 公式欄位概觀

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中建立自訂欄位，方法是參照現有欄位並在公式型別欄位中連線它們。

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱文章[建立欄位](/help/quicksilver/planning/fields/create-fields.md)中的「公式」一節。

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
<ul><li>選取</li> 
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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
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
   <td>   <p>管理工作區<span class="preview">和記錄型別</span> </a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## 有關公式欄位的考量事項

* 公式欄位參考屬於相同記錄型別的欄位。
* 只有在您將其他記錄型別連線到要為其建立公式欄位的記錄型別時，才能引用其他記錄型別的欄位。
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

## 支援的公式

Adobe Workfront Planning公式欄位支援Workfront計算欄位的大部分運算式。

>[!NOTE]
>
>Workfront Planning公式欄位不支援下列Workfront運算式：
>
>* SORTASCARRAY
>* SORTDESCARRAY
>* ADDHOUR
>* SWITCH
>* 格式


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
