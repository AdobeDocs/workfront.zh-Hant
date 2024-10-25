---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選器：顯示不完整的跨專案前置任務」
description: 此任務篩選器傳回不完整的跨專案前置任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 篩選器：顯示不完整的跨專案前置任務

此任務篩選器傳回不完整的跨專案前置任務。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 篩選跨專案前置任務

若要套用此篩選：

1. 前往工作清單或工作報告。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. （視條件而定）如果您從清單存取篩選器，請按一下&#x200B;**文字模式**；如果您從報表存取篩選器，請按一下&#x200B;**切換至文字模式**。
1. 在新區域中，貼上下列程式碼：
   <pre>前置任務MM：projectID=FIELD：projectID<br>前置任務MM：projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. （視條件而定）如果您從報表存取篩選器，請按一下&#x200B;**儲存篩選器**；如果您從工作清單存取篩選器，請按一下&#x200B;**套用**，然後按一下&#x200B;**另存為新篩選器**。
