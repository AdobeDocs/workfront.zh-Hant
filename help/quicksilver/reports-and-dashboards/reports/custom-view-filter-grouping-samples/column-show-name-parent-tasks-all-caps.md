---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：將父任務名稱顯示為全部大寫'
description: 您可以將此列添加到任務視圖中，以在所有大寫字母中顯示父任務的名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# 視圖：將父任務名稱顯示為所有大寫

您可以將此列添加到任務視圖中，以在所有大寫字母中顯示父任務的名稱。

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>請求修改篩選器、視圖和分組 </p>
   <p>計畫修改報表</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改單個視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 將父任務的名稱顯示為所有大寫

要在任務視圖中生成此列：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **自定義視圖**。\
   或\
   從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 的子菜單。
1. 按一下&#x200B;**切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它： <pre>描述鍵=名稱<br>displayname=任務名稱<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>寬度=150<br></pre>

1. 按一下 **保存視圖**。
