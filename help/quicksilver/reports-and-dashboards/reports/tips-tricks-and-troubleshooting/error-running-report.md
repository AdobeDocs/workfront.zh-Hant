---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「執行報表時出現錯誤訊息：'您當前未登錄。'」
description: 您必須具備下列存取權，才能執行本文「編輯我」中的步驟。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# 執行報表時出現錯誤訊息：&quot;您當前未登錄。&quot;

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
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 問題

執行報表或在控制面板中顯示報表時，會傳回下列錯誤：\
*請再試一次。您目前未登入。*

報表中不顯示任何結果。

## 原因

報表目前設為以停用使用者身分執行。

## 解決方案

您必須擁有報表的「管理」權限，才能變更報表設定。\
要調整報表並查看結果，請執行以下操作：

1. 前往報表。
1. 按一下 **報表動作** > **編輯** > **報表設定**.

1. 指定 **以下列權限運行此報告：** 欄位。\
   或\
   保留 **以下列權限運行此報告：** 欄位空白。

1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   執行此報表時，不應再次顯示錯誤。
