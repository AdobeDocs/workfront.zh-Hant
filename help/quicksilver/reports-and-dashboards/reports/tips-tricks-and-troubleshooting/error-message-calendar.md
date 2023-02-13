---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「日曆上的錯誤消息：'此日曆具有已停用使用者的檢視權限。'」
description: 您必須具備下列存取權，才能執行本文「編輯我」中的步驟。
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# 日曆上的錯誤訊息：&quot;此日曆具有已停用用戶的視圖權限。&quot;

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫，工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理日曆的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 問題

存取與您共用的日曆時，您會收到下列錯誤： 

*此行事曆具有已停用使用者的檢視權限。請通知管理員修正行事曆權限。*

## 原因

建立此日曆的用戶（其原始所有者）是已停用的用戶。 

## 解決方案

您可以透過下列方式解決此問題：

1. 複製原始日曆。 當您複製日曆時，您將成為日曆的所有者。 複製的日曆應顯示原始日曆中的所有資訊。\
   如需複製日曆的詳細資訊，請參閱 [複製日曆報表](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. 將複製的日曆與原始日曆的用戶共用。 所有使用者都應在新日曆上看到相同的資訊。
1. （可選和條件性）如果您有管理原始日曆的權限，請從日曆共用區域中刪除與其共用日曆的所有其他用戶。 這可避免使用者嘗試顯示錯誤日曆時的混淆。
