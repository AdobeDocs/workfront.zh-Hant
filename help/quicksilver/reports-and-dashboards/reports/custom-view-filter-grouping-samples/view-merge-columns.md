---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：合併來自一個共用列中多列的資訊'
description: 您可以合併在多個獨立列中顯示的資訊，並將其顯示在一個共用列中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# 視圖：從一個共用列中的多個列合併資訊

您可以合併在多個獨立列中顯示的資訊，並將其顯示在一個共用列中。

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
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 共用或合併列時的注意事項

* 可以合併兩個相鄰列，並顯示每個列中以換行符分隔的資訊，也可以合併兩個相鄰列中的資訊，而每個列的資訊之間沒有分隔符。
* 通過將本文中描述的相同語法應用於已共用的列和相鄰列，可以合併來自兩個以上列的資訊。
* 此

   ```
   valueformat=HTML
   ```

   行在共用列中是必需的。 否則，從Adobe Workfront導出報告時，這些列不包含任何資訊（它們將為空）。
* 合併列中可能不支援條件格式設定。

   存在以下例外：

   * 在Workfront查看資訊時，如果組成合併列的列具有彼此不同的格式，則保留第一列的格式，並忽略所有其他列的格式。
   * 將視圖導出到PDF檔案時，條件格式將應用於合併列中的第一列。
   * 將視圖導出到Excel檔案時，合併的列顯示為單獨的列。 各個列還顯示它們各自的條件格式規則。

* 列 **視圖別名** 屬性可以限制可合併的列數。 要避免這些限制，請避免使用 **視圖別名** 屬性。 如果必須包括 **視圖別名** 屬性，確保它是列中列出的最後一項。

* 如果將具有共用列的清單導出為Excel或制表符分隔格式，則這些列在導出的檔案中會分開。

## 合併兩列中的資料，但不帶換行符

可以合併多個獨立列中的資料，以在一列中顯示資料，每個列的值之間沒有中斷或空格。

>[!TIP]
>
>當合併兩個不能同時顯示同一記錄值的列時，建議使用此方法。 例如，在「工作項目」報表中，可以合併「問題名稱」和「任務名稱」列，而不會在它們之間換行，因為工作項目永遠不能同時具有問題名稱和任務名稱。 工作項可以是問題，也可以是任務(在Workfront)。

要執行此操作：

1. 使用視圖的文本模式，將以下文本添加到要合併的第一列：

   ```
   sharecol=true
   ```

   合併清單或報表的前兩列時，Workfront會先於每行文本，這些文本包含第一列中與對象有關的資訊，

   ```
   column.0.
   ```

   和包含第二列資訊的文本行

   ```
   column.1.
   ```

   。\
   必須在第一列的列號之前加上該列的編號。 列計數始終以清單或報表的最左側列開始，該列標籤為

   ```
   column.0.
   ```

   。

   如果共用多列，請確保在包含每列共用資訊的代碼行中添加列號。

   **示例：** 以下是包含三個獨立列的合併列的文本模式代碼，從清單的第二列開始。 合併後的值為「項目名稱」、「計畫起始日期」和「項目責任人名稱」，並且這三個值之間沒有中斷：

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

1. 按一下 **保存**，則 **保存視圖**。

## 用換行符合併兩列中的資料

執行以下操作以合併來自多個列的資料，以在一個公用列中顯示資料，並在每個列的值之間換行：

1. 在要合併的兩列之間添加第三列。

   >[!TIP]
   * 要合併的列必須彼此相鄰。
   * 必須按一下要合併的第一列。


1. 按一下 **切換到文本模式** 並在步驟1中添加的中間列中添加以下代碼：

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

1. 將以下文本添加到第一列：

   ```
   sharecol=true
   ```

   合併清單或報表的前兩列時，Workfront會先於每行文本，這些文本包含第一列中與對象有關的資訊，

   ```
   column.0.
   ```

   ，該列與

   ```
   column.1.
   ```

   ，以及包含有關第二列的資訊的文本行

   ```
   column.2.
   ```

   。如果組合列在視圖中間，則根據列在視圖中的位置對列進行編號。 列計數始終以清單或報表的最左側列開始，該列標籤為

   ```
   column.0.
   ```

   。

   如果共用多個列，請確保在包含共用資訊的代碼行中添加列號。

   **示例：** 以下是共用列的文本模式代碼，該共用列包含「項目名稱」、「計畫起始日期」和「項目所有者名稱」（帶換行符）。 共用列是項目視圖的第二列。

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

1. 按一下 **保存**，則 **保存視圖**。
