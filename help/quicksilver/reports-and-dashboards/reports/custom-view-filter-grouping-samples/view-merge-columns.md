---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：合併一個共用列中多列的資訊'
description: 您可以合併顯示在多個獨立欄中的資訊，並將其顯示在一個共用欄中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# 查看：從一個共用列中合併多列中的資訊

您可以合併顯示在多個獨立欄中的資訊，並將其顯示在一個共用欄中。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用或合併欄時的考量事項

* 您可以合併兩個相鄰列並顯示通過分行符號分隔的每個列的資訊，或者可以合併兩個相鄰列中的資訊，而不用分隔符號分隔每列的資訊。
* 您可以將本文所述的相同語法套用至已共用的欄和相鄰的欄，以合併來自多個欄的資訊。
* 此

   ```
   valueformat=HTML
   ```

   行在共用欄中是必填欄。 否則，從Adobe Workfront匯出報表時，欄不會包含任何資訊（將會是空白）。
* 合併的列中可能不支援條件式格式。

   存在下列例外：

   * 在Workfront中檢視資訊時，如果組成合併欄的欄格式彼此不同，則會保留第一欄的格式，並忽略所有其他欄的格式。
   * 將視圖導出到PDF檔案時，條件格式將應用於合併列中的第一列。
   * 將檢視匯出為Excel檔案時，合併的欄會顯示為個別欄。 個別欄也會顯示其各自的條件式格式規則。

* 包含 **檢視別名** 屬性可限制您可合併的欄數。 若要避免這些限制，請避免使用 **檢視別名** 屬性。 如果您必須包含 **檢視別名** 屬性，請確定該欄是列中的最後一個項目。

* 如果您將含有共用欄的清單匯出為Excel或Tab分隔格式，這些欄會在匯出的檔案中分開。

## 合併兩列的資料，不帶分行符號

您可以合併來自多個獨立欄的資料，以在一欄中顯示資料，且每欄的值之間沒有中斷或空格。

>[!TIP]
>
>合併兩欄時，建議您使用此方法來同時顯示同一記錄的值。 例如，在「工作項」報表中，「問題名」和「任務名」列可以合併，而不在它們之間加上分行符，因為「工作項」不能同時具有「問題名」和「任務名」。 工作項目可以是「問題」或「Workfront」中的任務。

要執行此操作：

1. 對檢視使用文字模式，將下列文字新增至您要合併的第一欄：

   ```
   sharecol=true
   ```

   當您合併清單或報表的前兩欄時，Workfront會在每行文字前面加上，其中包含第一欄中物件的相關資訊，並搭配

   ```
   column.0.
   ```

   以及包含第二欄資訊的文字行

   ```
   column.1.
   ```

   。\
   必須在第一列的列號前面加上該列的號。 欄計數一律以清單或報表最左側的欄開頭，標示為

   ```
   column.0.
   ```

   。

   如果您共用多個欄，請務必在程式碼行中新增欄碼，這些行包含每欄的共用資訊。

   **範例：** 以下是包含三個獨立列的合併列的文本模式代碼，從清單的第二列開始。 合併的值是「項目名稱」、「計畫起始日期」和「項目所有者名稱」，並且這三個值之間沒有中斷：

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.2.valuefield=plannedStartDate
   ```

   ```
   column.2.valueformat=atDate
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=owner:name
   ```

   ```
   column.3.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-no-line-breaks-350x142.png" style="width: 350;height: 142;"></pre>

1. 按一下 **儲存**，然後 **保存視圖**.

## 用分行符號合併兩列的資料

執行以下操作以合併來自多列的資料，將其顯示在一個公共列中，每個列的值之間帶有分行符號：

1. 在要合併的兩欄之間新增第三欄。

   >[!TIP]
   * 要合併的列必須相鄰。
   * 必須按一下要合併的第一列。


1. 按一下 **切換到文本模式** 並在您於步驟1新增的中間欄中新增下列程式碼：

   ```
   value=<br>
   ```

   ```
   valueformat=HTML
   ```

   ```
   width=1
   ```

   ```
   sharecol=true
   ```

1. 將下列文字新增至第一欄：

   ```
   sharecol=true
   ```

   當您合併清單或報表的前兩欄時，Workfront會在每行文字前面加上，其中包含第一欄中物件的相關資訊，並搭配

   ```
   column.0.
   ```

   ，此欄包含共用資訊，與

   ```
   column.1.
   ```

   ，以及包含第二欄相關資訊的文字行(使用

   ```
   column.2.
   ```

   .如果合併的列位於視圖的中間，則根據列在視圖中的位置對列進行編號。 欄計數一律以清單或報表最左側的欄開頭，標示為

   ```
   column.0.
   ```

   。

   如果您共用多個欄，請務必在包含共用資訊的程式碼行中新增欄碼。

   **範例：** 以下是共用列的文本模式代碼，該列包含帶分行符號的「項目名稱」、「計畫起始日期」和「項目所有者名稱」。 共用欄是專案檢視的第二欄。

   ```
   column.1.displayname=Project_StartDate_Owner
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.1.textmode=true
   ```

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.2.value=<br>
   ```

   ```
   column.2.width=1
   ```

   ```
   column.2.valueformat=HTML
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=plannedStartDate
   ```

   ```
   column.3.valueformat=atDate
   ```

   ```
   column.3.sharecol=true
   ```

   ```
   column.4.value=<br>
   ```

   ```
   column.4.width=1
   ```

   ```
   column.4.valueformat=HTML
   ```

   ```
   column.4.sharecol=true
   ```

   ```
   column.5.textmode=true
   ```

   ```
   column.5.valuefield=owner:name
   ```

   ```
   column.5.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-with-line-breaks-350x199.png" style="width: 350;height: 199;"></pre>

1. 按一下 **儲存**，然後 **保存視圖**.
