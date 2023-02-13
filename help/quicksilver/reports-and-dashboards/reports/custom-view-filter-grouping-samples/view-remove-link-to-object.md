---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '檢視：刪除列中對象的連結'
description: 預設情況下，顯示在指向對象的「詳細資訊」(Details)頁面的視圖連結中的某些對象。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 查看：刪除列中對象的連結

預設情況下，顯示在指向對象的「詳細資訊」(Details)頁面的視圖連結中的某些對象。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。

您可以在所有檢視中顯示的欄中使用文字模式來移除此連結。

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

## 範例：從任務視圖的「任務名稱」列中刪除指向任務的連結：

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖** 來建立新視圖。

   或

   按一下 **編輯圖示** ![](assets/edit-icon.png)

   要編輯現有視圖，請選擇視圖。

1. 按一下 **添加列** 來新增欄。

   或

   按一下具有對象連結的現有列。

1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：

   <pre>displayname=任務名<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=複合</pre>

   >[!TIP]
   >
   >通過調整以下內容，您可以對其他對象使用類似的代碼：
   >
   >   
   >   
   >   * 取代 **valuefield** 使用 **valueexpression** 和在等號後方的大括弧中加上相同的名稱。
   >   
   >   
   >
   >   
   >   
   >   * 消除以>開頭的所有行

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. 按一下 **儲存**，然後 **保存視圖**.
