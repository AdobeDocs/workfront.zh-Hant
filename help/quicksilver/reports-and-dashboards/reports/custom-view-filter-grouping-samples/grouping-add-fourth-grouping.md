---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：將第四個分組添加到清單'
description: 在矩陣報表中可以有4個分組。 有關矩陣報表的詳細資訊，請參閱建立矩陣報表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 分組：將第四個分組添加到清單

在矩陣報表中可以有4個分組。 有關矩陣報表的詳細資訊，請參見 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

通過標準介面，標準報表中只能有3個分組。 要在標準報表中添加第4個分組，必須使用文本模式。

![四分組_in_a_standard_report.png](assets/four-groupings-in-a-standard-report-350x59.png)

例如，您可能有一個按項目名稱、進展狀態和計畫完成日期分組的任務報告，但您也希望按「分配方名稱」對報告進行分組。

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

## 將第四個分組添加到清單

要添加第四個分組，請執行以下操作：

1. 轉到任務清單。
1. 從 **分組**&#x200B;下拉菜單，選擇 **新建分組**。

1. 按一下 **切換到文本模式**。
1. 在可用空間中，添加以下代碼：

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. 按一下 **完成**，則 **保存分組**。
