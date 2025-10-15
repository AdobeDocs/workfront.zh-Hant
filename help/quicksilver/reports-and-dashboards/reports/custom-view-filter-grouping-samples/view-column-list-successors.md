---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：在欄中新增任務後續任務清單
description: 您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 「工作後置任務」欄包含後置任務的數目以及名稱。
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%

---

# 檢視：在欄中新增任務後續任務清單

<!--Audited: 11/2024-->

您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 **任務後置任務**&#x200B;欄包含後置任務的數目以及名稱。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 在欄中新增任務後續任務清單

若要將此欄新增至工作檢視：

1. 前往工作清單。
1. 展開&#x200B;**檢視**&#x200B;下拉式功能表，然後按一下&#x200B;**新增檢視**。
1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 移除&#x200B;**編輯文字模式**&#x200B;方塊中的所有文字，並以下列程式碼取代：

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
