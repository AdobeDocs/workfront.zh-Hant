---
title: 公式欄位概觀
description: 在Adobe大師，您可以建立公式欄位，這些欄位使用函式和現有欄位來計算新的自訂值。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---


# 公式欄位概觀

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO miniTOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以在Adobe Maestro中建立自訂欄位，方法是參考現有欄位並使用公式將其連線。 您可以建立自訂公式型別欄位來完成此操作。

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱 [建立欄位](../fields/create-fields.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## 有關公式欄位的考量事項

* 公式欄位參考屬於相同記錄型別的欄位。 建立公式欄位時，您無法參考其他記錄型別的欄位。 <!--is this still accurate??-->
* 儲存公式欄位後，您無法變更其欄位型別。
* 儲存公式欄位後，您可以更新公式欄位的計算，而計算結果會自動更新相同型別的所有記錄。
* 當公式中的欄位顯示在Maestro介面時，您必須新增您在公式中參考的欄位。
* 在公式中使用連結記錄型別的查詢欄位將在稍後提供。

## 支援的公式

Maestro公式欄位支援Workfront計算欄位的所有運算式。 如需詳細資訊，請參閱 [計算資料運算式的概觀](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

此外，我們為Maestro公式欄位支援下列運算式：


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
   <td><strong>ID</strong> </td> 
   <td> <p>傳回記錄的ID。</p> <p>運算式的格式如下：

<code>{ID}</code>
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
   <td> <p>傳回一年中的周數。您可以選擇是否指定一週從哪一天開始（使用1代表星期日，或2代表星期一）。 如果省略，周從星期日開始（預設）。</p> <p>運算式的格式如下：

<code>WEEKOFYEAR（日期，2）</code>
或
<code>WEEKOFYEAR（日期）</code>
</p>
   </td></tr>

</table>





