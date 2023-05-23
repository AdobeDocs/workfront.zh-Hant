---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：任務視圖中工期和計畫工時的基準差異'
description: 此視圖在任務視圖 — 編輯我中顯示以下內容。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 視圖：任務視圖中工期和計畫工時的基準差異

此視圖在任務視圖中顯示以下內容：

* 包含基線任務資訊的任務資訊。
* 「持續時間」(Duration)與「預設基線持續時間」(Default Baseline Duration)之間的差。
* 計畫工時與預設基準計畫工時之間的差異。

>[!NOTE]
>
> 以下視圖中顯示的資料將實際任務值與與「預設基線」任務關聯的值進行比較。

 

![baseline_variance_in_a_task_view_png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## 在任務視圖中查看工期和計畫工時的基準差異

1. 轉到任務清單。
1. 在 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 刪除視圖中除第一個列外的所有列。
1. 選擇第一列後，按一下 **切換到文本模式**。
1. 複製下面的文本，並將其貼上到視圖的第一列：

   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=任務名<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=複合<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayname=任務持續時間<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=持續時間<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=defaultBaselineTask:durationFieldLong<br>column.2.valueformat=複合<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Dflt基線任務：工期<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Duration Variance"column.3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=持續時間差異<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.strt.0<br>column.3.valueexpression=CONCAT(SUB({duration},{defaultBaselineTask})。{duration})/480，「天」)<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=持續時間差異<br>column.4.descriptionkey=workred<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workremired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=複合<br>column.4.viewalias=工作要求<br>column.4.width=100<br>column.4.displayname=工作請求<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=必需工作<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.strt.0<br>column.5.valuefield=defaultBaselineTask:workFieldLong<br>column.5.valueformat=複合<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Dflt基線任務：工作請求<br>column.6.descriptionkey=workred<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=工作量差異<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.strt.0<br>column.6.valueexpression=CONCAT(SUB({workRequired},{defaultBaselineTask})。{workRequired})/60"小時")<br>column.6.valueformat=HTML<br>column.6.viewalias=工作要求<br>column.6.width=100<br>column.6.displayname=工作量差異</pre>

1. 按一下 **保存視圖**。\
   ![](assets/view--baseline-variance-for-duration-and-planned-work-350x78.png)
