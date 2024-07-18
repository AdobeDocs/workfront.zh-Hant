---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：在欄中新增任務後續任務清單」
description: 您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 「工作後置任務」欄包含後置任務的數目以及名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 2%

---

# 檢視：在欄中新增任務後續任務清單

您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 **任務後置任務**&#x200B;欄包含後置任務的數目以及名稱。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 在欄中新增任務後續任務清單

若要將此欄新增至工作檢視：

1. 移至現有的任務檢視。
1. 展開[檢視]下拉式功能表，然後選取&#x200B;**自訂檢視**。
1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移至此資料行&#x200B;**區域中的**&#x200B;顯示，然後按一下&#x200B;**按一下以編輯文字**。

1. 移除「文字模式」方塊中的所有文字，並以下列程式碼取代：
   <pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(successors)。lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor})。{taskNumber}，' - '，{successor}。{name})<br>valueformat=HTML</pre>

1. 按一下「**儲存視圖**」。
