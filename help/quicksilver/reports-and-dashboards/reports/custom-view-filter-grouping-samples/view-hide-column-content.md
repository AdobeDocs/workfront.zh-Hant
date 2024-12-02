---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：隱藏欄的內容
description: 您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來完成此操作。
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 檢視：隱藏欄的內容

<!--Audited: 11/2024-->

您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來完成此操作。

>[!NOTE]
>
>* 您可以使用隱藏欄，依您不想要在檢視中顯示的特定物件來排序。\
>  例如，您可以依任務檢視中的「任務編號」排序，並在檢視中隱藏「任務編號」資訊。 在這種情況下，欄中參照的物件有助於排序檢視，但該物件的資訊不會顯示在檢視中。
>* 當您隱藏欄時，請注意欄中的資訊是隱藏的，但該欄仍然存在於檢視中。
>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：<ul><li>修改檢視的貢獻者</li><li>用於修改報告的標準</li></ul></p><p>或</p>目前：<ul><li>請求修改檢視</li><li>計畫修改報表</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 範例：排序並隱藏工作檢視中的「工作編號」欄：

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表，按一下&#x200B;**新增檢視**。

1. 按一下&#x200B;**新增欄**&#x200B;並開始在&#x200B;**顯示在此欄**&#x200B;欄位中輸入「任務編號」，然後當它顯示在清單中時選取它。

1. 按一下&#x200B;**切換到文字模式**，然後&#x200B;**編輯文字**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   此程式碼中讓欄隱藏的重要變更包括：

   * `displayname=`：此行必須為空白。
   * `valuefield=`：此專案已由`value`取代，且必須為空白。
   * `width=`：根據欄位，此專案的值必須是&#x200B;**0**&#x200B;或&#x200B;**1**。

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
