---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''分組：任務百分比細分2'
description: '''在此自定義任務分組中，您可以顯示按任務完成百分比值範圍分組的任務。 細目顯示10%點增量的完成百分比值：1-10%,11-20%，等等。'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 4%

---

# 分組：任務百分比細分2

在此自定義任務分組中，可以顯示按任務完成百分比值範圍分組的任務。 細目顯示10%點增量的完成百分比值：1-10%、11-20%等。

以下分組按完成百分比值將項目組織為以下分組之一：

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10_blank_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改分組</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 按任務百分比細分分組

要應用此分組，請執行以下操作：

1. 轉到任務清單。
1. 從 **分組** 下拉菜單，選擇 **新建分組**。

1. 按一下 **切換到文本模式**。
1. 刪除 **將報告分組** 的子菜單。
1. 將文本替換為以下代碼：

   <pre>group.0.linkedname=direct<br>group.0.name=細分百分比<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %",IF({percentComplete}&lt;=31,"21-310 %",IF({percentComplete}&lt;41,"31-40 %",IF({percentComplete}&lt;51,"41-50 %",IF({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71,"61-70 %",IF({percentComplete}&lt;81,"71-80 %",IF({percentComplete}&lt;91,"81-90 %",IF({percentComplete}&lt;100,"91-99 %","100 %")))))))<br>textmode=true</pre>

1. 按一下 **保存分組**。
