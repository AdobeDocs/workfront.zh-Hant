---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：隱藏列的內容」'
description: 您可能希望隱藏視圖列中的資訊。 可通過修改列的文本模式來執行此操作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 視圖：隱藏列的內容

您可能希望隱藏視圖列中的資訊。 可通過修改列的文本模式來執行此操作。

>[!TIP]
>
>* 可以使用隱藏列按不希望在視圖中顯示的特定對象排序。\
   >  例如，您可以在任務視圖中按任務編號排序，並從視圖中隱藏任務編號資訊。 在這種情況下，列中引用的對象有助於對視圖進行排序，但該對象的資訊不會顯示在視圖中。
>* 隱藏列時，請注意列中的資訊已隱藏，但該列仍存在於視圖中。
>


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

## 示例：對任務視圖中的「任務編號」列進行排序和隱藏：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 並開始在 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>排序順序=1<br>sortType=asc<br>textmode=true<br><strong>值=</strong>值格式=int<br><strong>寬度=0</strong></pre>此代碼中使列隱藏的重要更改包括：

   ```
   displayname
   ```

   此行必須為空。

   ```
   valuefield
   ```

   已替換為 *值*，且必須為空。

   ```
   width
   ```

   :根據欄位的不同，此值必須為 *0* 或 *1*。

1. 按一下 **保存**，則 **保存視圖**。
