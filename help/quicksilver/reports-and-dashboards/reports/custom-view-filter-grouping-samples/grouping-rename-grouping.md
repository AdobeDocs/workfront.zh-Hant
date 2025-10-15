---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 群組：編輯群組中的顯示名稱
description: 您可以將清單和報告中的群組重新命名為您的使用者更熟悉的專案。
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 分組：編輯分組中的顯示名稱

<!--Audited: 01/2024-->

您可以將群組重新命名為使用者更熟悉的名稱。

例如，將標準Portfolio名稱群組套用至專案清單時，該群組的名稱會顯示為&#x200B;*Portfolio：名稱：`<name of portfolio>`*。

![依未編輯的名稱分組](assets/grouping-unedited-name-350x167.png)

您可以使用文字模式來修改此群組，以顯示較容易閱讀的名稱。

![依編輯的名稱分組](assets/grouping-edited-name-350x160.png)

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

## 編輯群組中的顯示名稱

若要變更專案群組中的顯示名稱：

1. 前往專案清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 按一下「**新增群組**」，並在「**群組依據：**」欄位中開始輸入「Portfolio名稱」，然後當它顯示在清單中時選取它。

1. 按一下&#x200B;**切換到文字模式**。
1. 執行下列任一項作業：

   * 將下列程式碼新增至&#x200B;**將您的報告分組**&#x200B;方塊中可用的現有文字：


     `group.0.displayname=Your Value`


     例如，新增下列程式碼，將顯示名稱變更為「Portfolio」：

     `group.0.displayname=Portfolio`

   * 移除群組文字模式介面中所有含有「名稱」字樣的行，然後新增該行：

     `group.0.name=Your Value`

     例如，新增下列程式碼，將顯示名稱變更為「Portfolio」：

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >您也可以將`group.0.name=`與`group.0.displayname=`行保留為空白，在這種情況下，分組會顯示您正在依據的值。


     ![依已編輯名稱分組（不含名稱）](assets/grouping-edited-name-no-name-350x162.png)

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存群組**。
1. （選擇性）更新群組名稱，然後按一下&#x200B;**儲存群組**。

   根據您的文字模式資訊修改分組的預設名稱。
