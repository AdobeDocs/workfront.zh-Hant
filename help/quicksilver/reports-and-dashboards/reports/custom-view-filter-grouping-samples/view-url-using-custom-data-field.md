---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：使用自定義資料欄位的外部URL'
description: 可以使用「任務視圖」中名為「自定義URL」的計算自定義欄位來顯示指向內部自定義URL的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 視圖：使用自定義資料欄位的外部URL

可以使用 **計算的自定義欄位** 名為「自定義URL」的 **任務視圖**。

這有助於您快速從某些對象中直接從報告連結到應用程式的某些區域。

建立計算的自定義欄位時，必須先建立該欄位，然後建立「視圖」。

以下各節是計算任務自定義欄位的示例。 自定義欄位稱為自定義URL。 自定義視圖顯示欄位的值以及 **URL** 的子菜單。

使用相同的步驟，可以為系統中具有「自定義表單」的所有對象建立類似的計算自定義欄位和自定義視圖。

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

## 建立「自定義URL」計算的自定義欄位

有關建立計算的自定義欄位的資訊，請參閱文章 [將計算資料添加到自定義窗體](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

如果您有權建立自定義表單，則可以為名為「自定義URL」的任務建立計算的自定義欄位。 此欄位直接連結到 **概述** 子頁籤 **任務詳細資訊** 頁籤。

1. 建立計算的自定義欄位。
1. 在「計算」欄位中，輸入以下代碼：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,&quot;ID&quot;/overview&quot;)

1. 替換「」`<domain>`&quot;，不帶括弧。

   此

   ```
   /overview
   ```

   此URL的一部分將連結指向 **概述** 的子菜單。

1. 在建立 **計算的自定義欄位**，附加 **自定義窗體** 將此欄位顯示到要在新視圖中顯示的Adobe Workfront中的多個任務。

## 建立顯示任務的「自定義URL」和「URL」欄位的視圖

任務 **視圖** 在下面的示例中， **計算的自定義欄位** 稱為「自定義URL」，作為指向 **概述** 任務中的子頁籤&#x200B;**詳細資訊** 的 **URL** 的子菜單。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

要自定義此視圖：

1. 轉到任務清單。
1. 展開 **視圖** 下拉框。
1. 按一下 **自定義視圖**。
1. 除第一列外，刪除視圖內的所有列。
1. 按一下第一列的標題。
1. 按一下 **切換到文本模式** 的上界。
1. 按一下 **按一下可編輯文本**。
1. 將下面的文本模式貼上到您的一列中。\
   在此示例中為&quot;column.1&quot;。 在「自定義URL」欄位中顯示值，作為任務的連結 **概述**。 &#39;列。2.&#39; 顯示儲存在 **URL欄位** 任務。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=自定義URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString（自定義URL）<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString（自定義URL）<br>column.1.name=自定義URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=自定義URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 按一下 **保存視圖**。
