---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：按錄入日期列出的項目'
description: 在此自定義項目分組中，您可以顯示按其「錄入日期」值分組的項目。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 分組：按錄入日期列出的項目

在此自定義項目分組中，您可以顯示按其「錄入日期」值分組的項目。

每個分組都顯示以下項目中具有錄入日期：

* 最後三十天
* 30-60天
* 60天或更久

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

## 按錄入日期對項目分組

要應用此分組，請執行以下操作：

1. 轉至現有項目報告或建立新項目報告。\
   有關建立報告的詳細資訊，請參閱文章 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 從 **分組** 按鈕 **添加分組**。

1. 按一下 **切換到文本模式**。
1. 刪除 **將報告分組** 的子菜單。
1. 將文本替換為以下代碼：

   ```
   group.0.linkedname=direct<br>
   ```

   ```
   group.0.name=Project Entry<br>
   ```

   ```
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))<br>
   ```

   ```
   group.0.valueformat=atDateAsMonthString<br>
   ```

   ```
   textmode=true
   ```

1. 按一下 **保存+關閉**。
