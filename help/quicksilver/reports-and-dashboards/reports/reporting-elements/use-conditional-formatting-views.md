---
product-area: reporting
navigation-topic: reporting-elements
title: 在視圖中使用條件格式
description: 在您與Adobe Workfront的其他用戶共用報告時，請考慮自定義報告視圖，使某些資訊更易於閱讀，或者只是脫穎而出。
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# 在視圖中使用條件格式

在您與Adobe Workfront的其他用戶共用報告時，請考慮自定義報告視圖，使某些資訊更易於閱讀，或者只是脫穎而出。

通過向報表視圖添加特殊或條件格式，可以自定義報表的「詳細資訊」頁籤。

您必須對報表具有「管理」權限，才能編輯報表並向視圖添加特殊格式。

有關建立報告的詳細資訊，請參閱文章 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

通過有條件地設定報表視圖中的列格式，您可以設定影響報表顯示方式的規則。 當滿足這些條件或規則時，應用特殊格式。

例如，如果任務完成百分比小於20%，則可以通過以粗體、紅色文本和黃色背景顏色顯示百分比數字來突出顯示該欄位。

使用有條件格式的視圖，您可以：

* 更改列的標題。
* 將列的值更改為自定義文本或影像。
* 通過更改背景的字型類型、顏色、對齊方式或顏色來設定欄位的顯示格式。

您在報告視圖中所做的更改僅在報告的「詳細資訊」頁籤中生效。 這些更改不會影響報表的「摘要」、「矩陣」或「圖表」頁籤。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>請求或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的視圖</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對報表的權限以在報表中建立或編輯視圖</p> <p>管理對視圖的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 先決條件

必須先建立報表，然後才能向其添加條件格式。

有關建立報告的資訊，請參見 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 建立有條件格式化的視圖

1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報告**。

1. 按一下要在其中建立有條件格式化視圖的報表的名稱。

   或

   按一下 **報告操作**，然後按一下 **編輯**。

1. （條件）如果編輯了報表，請選擇現有列或建立新列。
1. 按一下 **高級選項**。

1. 指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>自訂欄標籤</strong></td> 
      <td> <p>指定列的名稱。</p> <p>如果正在編輯現有列，則在此處指定名稱會更改現有列名。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>欄位格式</strong></td> 
      <td>選擇列中值的顯示格式。 根據列欄位的不同，這允許您設定日期、數字或貨幣的顯示方式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
      <td>如果希望在將報告置於儀表板上時顯示列，請選擇此欄位。 在儀表板外查看報告時，始終顯示該列。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **為此列添加規則**。

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在 **當：** 的子菜單。 例如：當任務完成百分比等於（區分大小寫）50時。
1. 在 **顯示如下欄位：** 部分指定滿足上述定義的條件時此欄位的外觀。

   指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文字顏色</strong></td> 
      <td> <p>選擇顯示文本的顏色。 有8種顏色可供選擇。</p> <p>注：如果欄位包含超連結，則文本顏色選擇不會應用於此欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字格式</strong></td> 
      <td>選擇是以粗體還是斜體顯示文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字對齊</strong></td> 
      <td>選擇是將文本對齊列內的右、中或左。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>選擇文本的背景顏色。 有8種顏色可供選擇。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示表徵圖</strong></td> 
      <td>如果要顯示表徵圖而不是此列的實際值，請從16個表徵圖中選擇。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示文字</strong></td> 
      <td> <p>選擇此選項可顯示此列的自定義標籤，而不是其實際值。 指定要顯示的文本，而不是提供的欄位中的值。</p> <p>重要提示：選擇 <strong>顯示文本</strong> 禁用內聯編輯此列中的文本的功能。<br>此外，不能更改前置任務列的值，因為它包含內置邏輯。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>套用到整行</strong></td> 
      <td>選擇此選項可將設定應用於整行，而不是僅將設定應用於選定列。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **添加規則**。\
   可以向同一列添加附加規則，或向其他列添加規則。

   規則按建立順序應用。 它們是組合的，但不會互相覆蓋，儘管列規則優先於同一單元格上的行規則。

   示例1:您可以首先建立一個規則，該規則在「項目狀態」為「正在構建」時，文本顏色為紫色和粗體。 然後，您將建立第二條規則，該規則在「任務名稱」不為空、文本顏色為紅色且斜體，背景顏色為綠色時進行說明。 在本示例中，出現以下情況：

   * 其「項目狀態」為「生成」的任務以紫色和粗體文本顯示。 如果任務名稱不為空，則任務的背景也為綠色。
   * 其「項目狀態」為「生成」以外的任務（且「任務名稱」不為空）以紅色和斜體文本顯示，背景為綠色。

   示例2:在影響整行的項目計畫完成日期上建立一個規則，如果取消項目，則將背景變灰（狀態= &quot;Dead&quot;）。 然後，建立一個列規則，當項目計畫完成日期小於今天（表示項目延遲）時，該列規則將背景變為紅色。 在本例中，如果已取消的項目有延遲完成日期，則該單元格將顯示為紅色，即使行中的其他單元格為灰色。 要更正此格式：

   * 編輯計畫完成日期的格式，並刪除延遲項目紅色背景的列規則。
   * 添加與行規則格式相同的列規則（當「項目狀態」=「Dead」時為灰色背景）。
   * 為延遲項目的紅色背景再次添加列規則。
   * 保存規則和視圖時，紅色背景不會應用於已取消的項目。


1. 按一下 **完成**。
1. 按一下 **保存+關閉**。\
   在報告中，如果滿足指定的條件，用戶將看到格式的更改。
