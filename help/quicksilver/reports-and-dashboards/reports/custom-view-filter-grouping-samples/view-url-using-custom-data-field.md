---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：使用自訂資料欄位的外部URL'
description: 您可以在「任務檢視」中使用名為「自訂URL」的計算自訂欄位，來顯示指向內部自訂URL的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 查看：使用自訂資料欄位的外部URL

您可以使用 **計算自訂欄位** 在 **任務視圖**.

這可協助您直接從報表，快速從檢視中的特定物件連結至應用程式的特定區域。

建立計算的自訂欄位時，您必須先建立欄位，然後建立檢視。

以下章節是任務的計算自訂欄位的範例。 自訂欄位稱為自訂URL。 自訂檢視會顯示欄位的值，以及 **URL** 欄位。

使用相同的步驟，您可以為系統中具有「自訂表單」的所有對象建立類似的計算自訂欄位和自訂視圖。

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

## 建立「自訂URL」計算自訂欄位

如需建立計算自訂欄位的相關資訊，請參閱文章 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

如果您有權建立自訂表單，則可以為名為「自訂URL」的任務建立計算的自訂欄位。 此欄位會直接連結至 **概述** 子標籤內 **任務詳細資訊** 標籤。

1. 建立計算的自訂欄位。
1. 在計算欄位中，輸入以下代碼：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&quot;)

1. 替換&quot;`<domain>`」，而不含括弧。

   此

   ```
   /overview
   ```

   部分的URL會將連結導向 **概述** 區段。

1. 建立 **計算自訂欄位**，附加 **自訂表單** 將此欄位顯示在Adobe Workfront中您要在新檢視中顯示的數個工作。

## 建立顯示任務的「自定義URL」和「URL」欄位的視圖

任務 **檢視** 在下列範例中， **計算自訂欄位** 稱為「自訂URL」，作為 **概述** 任務中的子標籤&#x200B;**詳細資料** 標籤，以及 **URL** 欄位。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

若要自訂此檢視：

1. 轉到任務清單。
1. 展開 **檢視** 下拉式清單。
1. 按一下 **自訂檢視**.
1. 移除檢視內除第一欄外的所有欄。
1. 按一下第一欄的標題。
1. 按一下 **切換到文本模式** 在介面的右上角。
1. 按一下 **按一下「 」以編輯文字**.
1. 將下方的文字模式貼入您的一欄。\
   在此範例中為「column.1」。 在「自訂URL」欄位中顯示值，作為任務的連結 **概述**. &#39;Column.2.&#39; 顯示儲存在 **URL欄位** 任務。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=自訂URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString（自訂URL）<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString（自訂URL）<br>column.1.name=自訂URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=自訂URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 按一下 **保存視圖**.
