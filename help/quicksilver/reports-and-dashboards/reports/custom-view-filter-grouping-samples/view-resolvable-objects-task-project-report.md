---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：任務或項目報表中的可解析對象」'
description: 您可以在項目或任務視圖或報告中顯示所有可解析對象的清單。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 視圖：任務或項目報表中的可解析對象

您可以在項目或任務視圖或報告中顯示所有可解析對象的清單。

有關可解析對象的詳細資訊，請參閱文章 [解析和可解析對象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

![list_of_resolevables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

對任務和項目應用此視圖是相同的。

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

## 查看任務或項目報表中的可解析對象

1. 轉到已從問題轉換的任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 的 **添加列**。

1. 按一下新列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   <pre>displayname=可解析項<br>清單分隔符=<br><br>listmethod=nested(resoluvess)。lists<br>textmode=true<br>類型=迭代<br>valuefield=name<br>valueformat=HTML<br></pre>

1. 按一下 **保存視圖**。\
   新列中將顯示所有可解析對象的清單。 清單中對象的名稱不能直接連結到對象。
