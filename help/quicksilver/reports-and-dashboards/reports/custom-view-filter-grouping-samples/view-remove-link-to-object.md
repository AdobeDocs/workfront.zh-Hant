---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：刪除列中對象的連結'
description: 預設情況下，在指向對象的「詳細資訊」(Details)頁面的視圖連結中顯示的某些對象。 例如，顯示項目名稱的列是指向項目的連結；顯示用戶名稱的列是指向用戶配置檔案頁的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 視圖：刪除列中對象的連結

預設情況下，在指向對象的「詳細資訊」(Details)頁面的視圖連結中顯示的某些對象。 例如，顯示項目名稱的列是指向項目的連結；顯示用戶名稱的列是指向用戶配置檔案頁的連結。

可以在所有視圖中顯示的列中使用文本模式刪除此連結。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 示例：從任務視圖的「任務名稱」列中刪除指向任務的連結：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖** 的子菜單。

   或

   按一下 **編輯表徵圖** ![](assets/edit-icon.png)

   要編輯現有視圖，請選擇視圖。

1. 按一下 **添加列** 的子菜單。

   或

   按一下包含指向對象的連結的現有列。

1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   <pre>displayname=任務名稱<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>值表達式={name}</strong><br>valueformat=複合</pre>

   >[!TIP]
   >
   >通過調整以下內容，可以對其它對象使用類似代碼：
   >
   >   
   >   
   >   * 替換 **值欄位** 代碼行 **值表達式** 在等號後，在大括弧中保留相同的名稱。
   >   
   >   
   >
   >   
   >   
   >   * 消除所有以>開頭的行
   >   
   >     ```>   
   >     link.
   >     ```   >   
   >   
   >     from the original text of the column. For example, eliminate all the following lines:
   >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
   >   
   >   
   >



1. 按一下 **保存**，則 **保存視圖**。
