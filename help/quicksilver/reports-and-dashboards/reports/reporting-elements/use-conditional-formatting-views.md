---
product-area: reporting
navigation-topic: reporting-elements
title: 在檢視中使用條件式格式
description: 當您在Adobe Workfront中與其他使用者共用報表時，請考慮自訂報表檢視，讓某些資訊更易於閱讀或突顯出來。
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 3%

---

# 在檢視中使用條件式格式

<!-- Audited: 11/2024 -->

當您在Adobe Workfront中與其他使用者共用報表時，請考慮自訂報表檢視，讓某些資訊更易於閱讀或突顯出來。

您可以新增特殊或條件式格式至報表檢視，以自訂報表的詳細資訊標籤。

如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

您可以視條件格式化報表檢視中的欄，以設定影響報表顯示方式的規則。 當滿足這些條件或規則時，將套用特殊格式。

例如，如果任務的完成百分比小於20%，您可以透過以粗體、紅色文字和黃色背景顏色顯示百分比數字來反白顯示欄位。

使用條件格式化檢視，您可以：

* 變更欄的標題。
* 將欄的值變更為自訂文字或影像。
* 變更字型型別、顏色、對齊方式或背景顏色，格式化欄位顯示。

您在報表檢視中所做的變更只有在報表的詳細資訊標籤中才會生效。 這些變更不會影響報告的「摘要」、「矩陣」或「圖表」標籤。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>新增：</p> 
   <ul><li>報告檢視的標準</li>
  <li> 清單檢視的投稿人或更新版本</li></ul>
   <p>目前：</p>
   <ul>
    <li> 規劃報告檢視 </li>
    <li> 要求或更高的清單檢視 </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的檢視</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以建立或編輯報表中的檢視</p> <p>管理檢視的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立報表，才能在其檢視中新增條件式格式。

如需建立報告的詳細資訊，請參閱[建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 建立條件式格式檢視

{{step1-to-reports}}

1. 按一下您要建立條件式格式檢視的報表名稱

   或

   按一下「**新增報表**」，然後選取物件型別以建立新報表。

1. （視條件而定）如果您編輯現有報表，請按一下&#x200B;**報表動作**，然後按一下&#x200B;**編輯**。

1. 在&#x200B;**欄（檢視）**&#x200B;索引標籤中，按一下以選取現有的欄，或按一下&#x200B;**新增欄**&#x200B;以建立欄。
1. 在Report Builder左上角的&#x200B;**顯示在此欄**&#x200B;欄位中，選取您要在新欄中顯示的欄位。
1. 按一下&#x200B;**進階選項**。

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>自訂欄標籤</strong></td> 
      <td> <p>指定資料行的名稱。</p> <p>如果您正在編輯現有資料欄，在此指定名稱會變更現有資料欄名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>欄位格式</strong></td> 
      <td>選擇欄中值的顯示格式。 視欄欄位而定，這可讓您設定日期、數字或貨幣的顯示方式。 並非所有欄都會顯示此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
      <td>如果您希望報表置於儀表板時欄顯示，請選取此欄位。 當您在儀表板外檢視報表時，欄始終顯示。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**為此欄新增一項規則**」。

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在&#x200B;**當：**&#x200B;區段中，設定資料行的條件陳述式。

   例如：「當任務完成百分比等於（區分大小寫） 50」。
1. 在&#x200B;**顯示如下的欄位：**&#x200B;區段中，指定當上述定義的條件符合時，此欄位會是什麼樣子。

   指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文字顏色</strong></td> 
      <td> <p>使用顏色選取器選取文字的顯示顏色。</p> <p><b>附註</b></p> <p> 如果欄位包含超連結，則文字顏色選取範圍不會套用至此欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字格式</strong></td> 
      <td>選取要以粗體或斜體顯示文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字對齊</strong></td> 
      <td>選取文字要靠欄內的右側、中央或左側對齊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>使用顏色選取器選取文字背景的顏色。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示圖示</strong></td> 
      <td>如果您想要顯示圖示而非此欄的實際值，請從16個圖示中選擇一個。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示文字</strong></td> 
      <td> <p>選擇此選項以顯示此欄的自訂標籤，而不是其實際值。 指定要顯示的文字，而不是提供的欄位中的值。</p> <p><b>重要</b></p> <p>選取<strong>顯示文字</strong>會停用內嵌編輯此欄文字的功能。<br>此外，您無法變更「前置任務」欄的值，因為它包含內建邏輯。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>套用到整行</strong></td> 
      <td>選取此選項可將設定套用至整列，而非僅將設定套用至選取的欄。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**新增規則**。\
   您可以將其他規則新增至相同欄，或將規則新增至其他欄。

   規則會依照其建立順序套用。 它們會合併，但不會互相覆寫，不過相同儲存格上的欄規則會優先於列規則。

   **範例1**

   您可以先建立一個規則，說明當專案處於建置狀態時，文字顏色為紫色和粗體。 然後，您會建立第二個規則，說明當任務的「名稱」不是空白時，文字顏色為紅色且斜體，背景顏色為綠色。 在此範例中，會發生下列情況：

   * 專案狀態為「正在建立」的任務會以紫色和粗體文字顯示。 如果任務名稱不是空白的，任務也會有綠色背景。
   * 「專案狀態」為「建置」以外任何專案（且「任務名稱」非空白）的任務會以綠色背景的紅色及斜體文字顯示。

   **範例2**

   在「專案計畫完成日期」欄中建立會影響整列的規則，如果專案已取消（例如，「專案狀態」為「廢棄」時），就會將背景變灰。 接著建立欄位規則，當專案計畫完成日期小於今天（表示專案延遲）時，將背景變成紅色。 在此範例中，如果取消的專案有延遲完成日期，則該儲存格將顯示為紅色，即使列中的其他儲存格為灰色。 若要更正此格式：

   * 編輯計畫完成日期的格式，並刪除延遲專案紅色背景的欄規則。
   * 新增格式與列規則相同的欄規則（專案狀態=廢棄時為灰色背景）。
   * 再次為延遲專案的紅色背景新增欄規則。
   * 當您儲存規則和檢視時，紅色背景不會套用至已取消的專案。

1. 按一下「**儲存**」。
1. 按一下「**儲存並關閉**」。\
   在報表中，如果符合指定的條件，使用者會看到格式變更。
