---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"篩選：建立參考相同欄位（''AND''陳述式）的多個篩選規則」'
description: 在標準模式介面中，嘗試建立參考相同欄位的多個篩選器（使用AND限定符）時，當您儲存報表並退出Report Builder時，會刪除其中一個篩選器。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 篩選：建立參考相同欄位的多個篩選規則（「AND」陳述式）

在標準模式介面中，嘗試建立參考相同欄位的多個篩選器（使用AND限定符）時，當您儲存報表並退出Report Builder時，會刪除其中一個篩選器。

**範例：** 您可能只想查看包含&quot;green&quot;一詞但名稱中不包含&quot;red&quot;一詞的任務。 Adobe Workfront不允許使用標準模式介面保存以下篩選規則，因為它引用了相同的欄位（任務名稱），但使用了不同的修改量並引用了不同的值：

* 任務名稱>包含>綠色
* 任務名稱>不包含>紅色

不過，您可以使用文字模式建立此篩選。

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

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立參考相同欄位的多個篩選規則

1. 轉到任務清單。
1. 從 **篩選** 下拉式功能表，選取 **新增篩選**.
1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 在「設定報表規則」區域中，新增下列程式碼：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >若要建立類似的篩選器，請先建立第一個陳述式。 例如：
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >視需要複製並貼上陳述式的次數。 然後，您可以新增您需要參考相同欄位的任意陳述式（在本例中為「name」），並對其他陳述式進行下列修改：
   >
   >1. 在兩個複製行前面加上&quot;AND&quot;:1:&quot;, &quot;和:2:&quot;, &quot;和:3:「」，等，表示每個新欄位可能的值。
   >1. 將欄位行取代為新欄位值（在&quot;=&quot;符號後）。
   >1. 用新修改量替換修改量行(_Mod)。

   >   
   >這些陳述區分大小寫。

1. 按一下 **完成**，然後 **儲存篩選**.
