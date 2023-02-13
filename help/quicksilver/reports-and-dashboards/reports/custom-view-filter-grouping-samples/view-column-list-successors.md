---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：在列中添加任務後續項清單'
description: 您可以向任務視圖添加列，以顯示任務的後繼者清單。 「任務後繼者」列包括後繼者的編號和名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 查看：在列中添加任務後續項清單

您可以向任務視圖添加列，以顯示任務的後繼者清單。 此 **任務後繼者** 列包括後繼項的編號和名稱。

![task_view_with_a_list_of_successors_png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## 在列中添加任務後繼程式清單

要將此列添加到任務視圖，請執行以下操作：

1. 轉到現有任務視圖。
1. 展開「檢視」下拉式功能表，然後選取 **自訂檢視**.
1. 按一下 **添加列**.
1. 按一下 **切換到文本模式**.
1. 將滑鼠移至 **顯示在此列中** 按一下 **按一下「 」以編輯文字**.

1. 移除「文字模式」方塊中的所有文字，並以下列程式碼取代：

   <pre>displayname=任務後繼項<br>listdelimeter=<br><br>listmethod=nested(subclers)。lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({supler})。{taskNumber},' - ',{succlement}。{name})<br>valueformat=HTML</pre>

1. 按一下 **保存視圖**.
