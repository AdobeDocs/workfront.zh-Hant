---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：顯示不完整的跨項目後續項'
description: 此任務篩選器返回不完整的跨項目後續任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 篩選器：顯示不完整的跨項目後續項目

此任務篩選器返回不完整的跨項目後續任務。

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改篩選器</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 篩選跨項目後續項

要應用此篩選器：

1. 轉到任務清單。
1. 從 **篩選** 下拉菜單，選擇 **新建篩選器**。

1. 按一下&#x200B;**切換到文本模式**。
1. 在 **設定報表的篩選器規則** ，貼上以下代碼：
   <pre>完成百分比= 100<br>百分比完成_修改=ne<br>後繼者MM:projectID=FIELD:projectID<br>後繼程式MM:projectID_Mod=ne</pre>

1. 按一下 **保存篩選器**。
