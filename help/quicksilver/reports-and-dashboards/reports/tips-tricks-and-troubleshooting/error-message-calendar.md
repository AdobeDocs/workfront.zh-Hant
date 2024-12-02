---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 行事曆上的錯誤訊息：「此行事曆擁有已停用使用者的檢視許可權。」
description: 瞭解「此行事曆擁有已停用使用者的檢視許可權」錯誤訊息。
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 行事曆上的錯誤訊息：「此行事曆擁有已停用使用者的檢視許可權。」

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>計畫、工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理行事曆的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

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
