---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：組合任務和問題詳細資訊（在小時清單中）'
description: 此小時視圖使用共用列標籤組合了「任務」和「發放名稱」列，以及「任務」和「發放計畫小時數」。 由於工時條目只能屬於任務或問題，因此兩個對象不能同時出現在同一列中。 視圖的每一行都填充來自任務或問題的資訊。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# 視圖：工時清單中的組合任務和問題詳細資訊

此小時視圖使用

```
sharecol
```

標籤。 由於工時條目只能屬於任務或問題，因此兩個對象不能同時出現在同一列中。 視圖的每一行都填充來自任務或問題的資訊。

瞭解有關

```
sharecol
```

標籤，請參閱 [視圖：從一個共用列中的多個列合併資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)。\
![custom_view_hours_with_task_and_issue_information_png](assets/custom-view-hours-with-350x48.png)

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

## 在「工時」清單中查看組合任務和問題詳細資訊

要應用此視圖，請執行以下操作：

1. 轉到小時清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.1.querysort=項目：名稱<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project.name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=任務或問題<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task)。string(name)<br>column.2.name=任務或問題<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=task:name<br>column.2.valueformat=HTML<br>column.2.width=100<br>column.3.descriptionkey=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=opTask:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=opTask:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask)。string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.shortview=false<br>column.3.strt.0<br>column.3.valuefield=opTask:name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=task：工作<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.4.namekeyargkey.1=工作<br>column.4.displayname=計畫工作量<br>column.5.displayname=計畫工作量<br>column.5.viewalias=opTask:workrequired<br>column.5.linkedname=opTask<br>column.5.valuefield=opTask:workRequired<br>column.5.valueformat=複合<br>column.5.querysort=opTask:workRequired<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=所需工作<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=小時<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble（小時）<br>column.6.namekey=hours.abbr<br>column.6.querysort=小時<br>column.6.shortview=false<br>column.6.strt.0<br>column.6.valuefield=小時<br>column.6.valueformat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string（說明）<br>column.8.namekey=description.abbr<br>column.8.querysort=說明<br>column.8.shortview=false<br>column.8.strt.0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150</pre>

1. 按一下 **保存視圖**。
