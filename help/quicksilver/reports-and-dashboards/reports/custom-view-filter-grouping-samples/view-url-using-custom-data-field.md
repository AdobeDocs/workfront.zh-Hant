---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：使用自訂資料欄位的外部URL」
description: 您可以在任務檢視中使用名為「自訂URL」的計算自訂欄位，顯示內部自訂URL的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 檢視：使用自訂資料欄位的外部URL

您可以使用&#x200B;**任務檢視**&#x200B;中名為「自訂URL」的&#x200B;**計算自訂欄位**，來顯示內部自訂URL的連結。

這可協助您直接從報表快速從檢視中的特定物件連結至應用程式的某些區域。

建立計算自訂欄位時，您必須先建立欄位，然後建立檢視。

以下小節是任務的計算自訂欄位範例。 此自訂欄位稱為自訂URL。 自訂檢視會顯示欄位的值以及任務的&#x200B;**URL**&#x200B;欄位。

使用相同的步驟，您可以為系統中具有「自訂表單」的所有物件建立類似的計算自訂欄位和自訂檢視。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 建立「自訂URL」計算自訂欄位

如需有關建立計算自訂欄位的資訊，請參閱文章[將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

如果您有建立自訂表單的存取權，可以為稱為「自訂URL」的任務建立計算自訂欄位。 此欄位直接連結到&#x200B;**任務詳細資料**&#x200B;標籤內的&#x200B;**概觀**&#x200B;子標籤。

1. 建立計算自訂欄位。
1. 在「計算」欄位中輸入下列代碼：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;，&quot;/&quot;，&quot;task/&quot;，ID，&quot;/overview&quot;)

1. 將&quot;`<domain>`&quot;取代為您的實際網域名稱，不含方括弧。

   此

   ```
   /overview
   ```

   此URL的部分會將連結導向至任務左側面板中的&#x200B;**概觀**&#x200B;區段。

1. 建立您的&#x200B;**計算自訂欄位**&#x200B;後，將此欄位附加至&#x200B;**自訂表單**&#x200B;以在新檢視中顯示的Adobe Workfront中數個工作。

## 建立檢視，以顯示任務的「自訂URL」和「URL」欄位

下列範例中的工作&#x200B;**檢視**&#x200B;顯示名為「自訂URL」的&#x200B;**計算自訂欄位**，作為工作&#x200B;**詳細資料**&#x200B;標籤內&#x200B;**總覽**&#x200B;子標籤的直接連結，以及工作的&#x200B;**URL**&#x200B;欄位。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

若要自訂此檢視：

1. 前往工作清單。
1. 展開工作清單頂端的&#x200B;**檢視**&#x200B;下拉式清單。
1. 按一下&#x200B;**自訂檢視**。
1. 移除檢視內的所有欄（第一欄除外）。
1. 按一下第一欄的標題。
1. 按一下介面右上角的&#x200B;**切換至文字模式**。
1. 按一下&#x200B;**按一下以編輯文字**。
1. 將下方的文字模式貼到一欄中。\
   在此範例中，「column.1.」 顯示「自訂URL」欄位中的值，做為工作&#x200B;**總覽**&#x200B;的連結。 &#39;欄。2.&#39; 顯示儲存在任務的&#x200B;**URL欄位**&#x200B;中的值。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.link.link=direct<br>column.0.listsort=string(name)<br>column.string.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link=customDataLabelsAsString(String) url)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString（自定義URL）<br>column.1.name=自定義URL<br>column.1.querysort=URL<br>column.1.short=false<br>column.1.valuefield=自定義URL<br>column.1.valueformat=customDataLabelsAsString<br> column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>列2.寬度=150<br><br><br></pre>

1. 按一下「**儲存視圖**」。
