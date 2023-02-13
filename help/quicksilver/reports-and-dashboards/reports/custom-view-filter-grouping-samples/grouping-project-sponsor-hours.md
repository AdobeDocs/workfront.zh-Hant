---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''分組：項目贊助人幾小時'
description: 此小時分組按記錄小時的項目贊助商組織小時。 小時分組的標準報告建立工具介面不提供「專案贊助商」欄位的對應。 必須使用文本模式介面才能訪問此欄位。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 分組：項目贊助人數小時

此小時分組按記錄小時的項目贊助商組織小時。 小時分組的標準報告建立工具介面不提供「專案贊助商」欄位的對應。 必須使用文本模式介面才能訪問此欄位。

![hour_report_grouped_by_ponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 按項目贊助方分組數小時

要應用此分組，請執行以下操作：

1. 去查一下小時清單。
1. 從 **分組** 下拉式功能表，選取 **新分組**.

1. 按一下&#x200B;**切換到文本模式**.
1. 移除 **將報表分組** 的上界。

1. 使用下列程式碼取代文字：

   <pre>group.0.linkedname=project:sponsor:名稱<br>group.0.name=<br>group.0.valuefield=project:sponsor:名稱<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. 按一下 **儲存分組**.
