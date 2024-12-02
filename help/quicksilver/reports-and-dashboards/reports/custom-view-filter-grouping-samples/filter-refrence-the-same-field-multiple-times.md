---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選：建立參照相同欄位（「AND」陳述式）的多個篩選規則
description: 在標準模式介面中，當您嘗試建立參照相同欄位的多個篩選器時（使用AND限定詞），當您儲存報表並退出Report Builder時會刪除其中一個篩選器。
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 篩選：建立參照相同欄位（「AND」陳述式）的多個篩選規則

<!--Audited: 10/2024-->

在標準模式介面中，當您嘗試建立參照相同欄位的多個篩選器時（使用AND限定詞），當您儲存報表並退出Report Builder時會刪除其中一個篩選器。

**範例：**&#x200B;您可能只想檢視名稱中包含「綠色」字樣但不包含「紅色」字樣的工作。 Adobe Workfront不允許您使用標準模式介面儲存下列篩選規則，因為它參考相同的欄位（工作名稱），但使用不同的修飾詞和參考不同的值：

* 工作名稱>包含>綠色
* 任務名稱>不包含>紅色

不過，您可以使用文字模式建立此篩選器。

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
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

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立參考相同欄位的多個篩選規則

1. 前往工作清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。
1. 按一下&#x200B;**文字模式**。
1. 在顯示的方塊中，新增下列程式碼：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >若要建置類似的篩選器，請先建置第一個陳述式。 例如：
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >視需要多次複製並貼上陳述式。 然後，您可以視需要新增陳述式，以參考相同欄位（在此案例中為「名稱」），並對其他陳述式進行下列修改：
   >
   >1. 針對每個新欄位可能的值，在兩個複製行的前面加上&quot;AND:1:&quot;、&quot;AND:2:&quot;、&quot;AND:3:&quot;等。
   >1. 將欄位行替換為新的欄位值（在「=」符號之後）。
   >1. 以新的修正因子取代修正因子明細行(_Mod)。
   >   
   >這些陳述式會區分大小寫。

1. 按一下&#x200B;**套用**，然後按&#x200B;**另存新檔**。
