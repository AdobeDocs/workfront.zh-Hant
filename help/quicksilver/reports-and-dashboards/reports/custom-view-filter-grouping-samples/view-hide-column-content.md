---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：隱藏列的內容」'
description: 您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來執行此操作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 查看：隱藏列的內容

您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來執行此操作。

>[!TIP]
>
>* 您可以使用隱藏的欄，依您不想在檢視中顯示的特定物件來排序。\
   >  例如，您可以按任務視圖中的任務編號排序，並在視圖中隱藏任務編號資訊。 在這種情況下，列中引用的對象有助於對視圖進行排序，但視圖中不顯示該對象的資訊。
>* 隱藏列時，請注意列中的資訊是隱藏的，但該列仍存在於視圖中。
>


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

## 範例：在任務視圖中排序和隱藏「任務編號」列：

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖**.

1. 按一下 **添加列** 並在 **顯示在此列中** 欄位，然後在清單中顯示時加以選取。

1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>此程式碼中的重要變更會隱藏欄：

   ```
   displayname
   ```

   此行必須為空白。

   ```
   valuefield
   ```

   此項已取代為 *value*，且必須空白。

   ```
   width
   ```

   :根據欄位，此值必須為 *0* 或 *1*.

1. 按一下 **儲存**，然後 **保存視圖**.
