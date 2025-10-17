---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 行事曆上的錯誤訊息：「此行事曆擁有已停用使用者的檢視許可權。」
description: 瞭解「此行事曆擁有已停用使用者的檢視許可權」錯誤訊息。
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# 行事曆上的錯誤訊息：「此行事曆擁有已停用使用者的檢視許可權。」

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
     <p>標準</p>
     <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理行事曆的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 問題

存取共用給您的行事曆時，您會收到下列錯誤： 

*此行事曆擁有已停用使用者的檢視許可權。 請讓系統管理員修正行事曆許可權。*

## 原因

建立此行事曆的使用者（其原始擁有者）是已停用的使用者。 

## 解決方案

您可以透過下列方式解決此問題：

1. 複製原始行事曆。 當您複製行事曆時，您就會成為行事曆的擁有者。 複製的行事曆應顯示原始行事曆的所有資訊。\
   如需有關複製行事曆的詳細資訊，請參閱[複製行事曆報告](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md)。

1. 與原始行事曆相同的使用者共用複製的行事曆。 所有使用者在新行事曆上應該會看到相同的資訊。
1. （選擇性和條件性）如果您有管理原始行事曆的許可權，請從行事曆共用區域移除與其共用行事曆的所有其他使用者。 這可消除使用者嘗試顯示錯誤行事曆時的困惑。
