---
product-area: reporting
navigation-topic: reporting-elements
title: 在檢視中使用條件式格式
description: 當您與Adobe Workfront中的其他使用者共用報表時，請考慮自訂報表檢視、讓特定資訊更容易閱讀，或只是突顯出來。
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 在檢視中使用條件式格式

當您與Adobe Workfront中的其他使用者共用報表時，請考慮自訂報表檢視、讓特定資訊更容易閱讀，或只是突顯出來。

您可以新增特殊或條件式格式至報表檢視，以自訂報表的「詳細資料」標籤。

您必須擁有報表的「管理」權限，才能編輯報表，並為檢視新增特殊格式。

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

通過有條件地格式化報表視圖中的列，您可以設定影響報表顯示方式的規則。 當這些條件或規則符合時，就會套用特殊格式。

例如，如果任務完成百分比小於20%，則可以通過以粗體、紅色文本和黃色背景顏色顯示百分比數字來突出顯示該欄位。

有條件格式化視圖時，您可以：

* 變更欄的標題。
* 將欄的值變更為自訂文字或影像。
* 通過更改背景的字型類型、顏色、對齊方式或顏色來格式化欄位的顯示。

您在報表檢視中所做的變更，只會在報表的「詳細資訊」標籤中生效。 這些變更不會影響報表的「摘要」、「矩陣」或「圖表」標籤。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的檢視</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理報表權限以建立或編輯報表中的檢視</p> <p>管理檢視的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立報表，才能新增條件式格式。

如需建立報表的詳細資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 建立有條件格式的視圖

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **報表**.

1. 按一下要建立條件式格式化視圖的報表名稱。

   或

   按一下 **報表動作**，然後按一下 **編輯**.

1. （條件性）如果您編輯報表，請選取現有欄或建立新欄。
1. 按一下 **進階選項**.

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>自訂欄標籤</strong></td> 
      <td> <p>指定欄的名稱。</p> <p>如果正在編輯現有列，在此處指定名稱將更改現有列名。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>欄位格式</strong></td> 
      <td>選擇顯示列中值的格式。 這可讓您設定日期、數字或貨幣的顯示方式，視欄位為何而定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
      <td>如果要在將報表放在控制面板上時顯示欄，請選取此欄位。 當您在控制面板外部查看報表時，一律會顯示欄。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **為此欄新增規則**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在 **當：** 一節，為列設定條件語句。 例如：當任務完成百分比等於（區分大小寫）50時。
1. 在 **如下所示顯示欄位：** 區段會指定當符合上述定義的條件時，此欄位的外觀。

   指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文字顏色</strong></td> 
      <td> <p>選取顯示文字的顏色。 有8種顏色可用。</p> <p>注意：如果欄位包含超連結，則文本顏色選擇不會應用到此欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字格式</strong></td> 
      <td>選取要以粗體或斜體顯示文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字對齊</strong></td> 
      <td>選擇文本在列內靠右、靠中或靠左對齊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>選取文字的背景顏色。 有8種顏色可用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示表徵圖</strong></td> 
      <td>如果要顯示表徵圖，而不是此列的實際值，請從16個表徵圖之一中選擇。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示文字</strong></td> 
      <td> <p>選擇此選項可顯示此欄的自訂標籤，而非其實際值。 指定要顯示的文字，而非提供欄位中的值。</p> <p>重要：選取 <strong>顯示文本</strong> 禁用內嵌編輯此列中文本的能力。<br>此外，您無法更改前置列的值，因為它包含內置邏輯。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>套用到整行</strong></td> 
      <td>選取此選項可將設定套用至整列，而非僅將設定套用至選取的欄。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **新增規則**.\
   您可以新增其他規則至相同的欄，或新增規則至其他欄。

   規則的套用順序為建立規則的順序。 它們會合併，但不會互相覆寫，但欄規則優先於相同儲存格上的列規則。

   範例1:您可以先建立規則，指出「專案狀態」為「建立」時，文字顏色為紫色和粗體。 然後，您將建立第二個規則，該規則指明「任務名稱」不是空的，文本顏色為紅色，斜體，背景顏色為綠色。 在此範例中，會發生下列情況：

   * 項目狀態為「正在構建」的任務以紫色和粗體文本顯示。 如果任務名稱不為空，則任務的背景也為綠色。
   * 其「項目狀態」為「正在構建」以外的任何值（且「任務名稱」不為空）的任務將以紅色和斜體文本顯示，背景為綠色。

   範例2:在影響整行的項目計畫完成日期上建立規則，如果取消項目，則將背景變灰（狀態=「無效」）。 然後，建立一個列規則，當項目計畫完成日期小於今天時（表示項目延遲），該列規則會將背景變為紅色。 在此示例中，如果取消的項目有延遲的完成日期，則即使行中的其他單元格顯示為灰色，該單元格仍將顯示為紅色。 要更正此格式：

   * 編輯「計畫完成日期」的格式，並刪除延遲項目紅色背景的列規則。
   * 新增格式與列規則相同的欄規則（專案狀態=「無效」時為灰色背景）。
   * 針對後期專案的紅色背景再次新增欄規則。
   * 儲存規則和檢視時，紅色背景不會套用至已取消的專案。


1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   在報表上，若符合指定的條件，使用者會看到格式變更。
