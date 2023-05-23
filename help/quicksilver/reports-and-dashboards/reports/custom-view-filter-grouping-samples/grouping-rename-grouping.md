---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：編輯分組中的顯示名稱'
description: 您可以將分組更名為用戶更熟悉的內容。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 分組：編輯分組中的顯示名稱

您可以將分組更名為用戶更熟悉的內容。

例如，將標準Portfolio名稱分組應用於項目清單時，分組的名稱將顯示為 *Portfolio:名稱：`<name of portfolio>`*。

![](assets/grouping-unedited-name-350x167.png)

可以使用文本模式修改此分組以顯示易於讀取的名稱。

![](assets/grouping-edited-name-350x160.png)

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
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改分組</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 編輯分組中的顯示名稱

要更改項目分組中的顯示名稱：

1. 轉到項目清單。
1. 從 **分組**&#x200B;下拉菜單，選擇 **新建分組**。

1. 按一下 **添加分組**，然後在中鍵入「Portfolio名稱」 **首先：** 的子菜單。

1. 按一下 **切換到文本模式**。
1. 執行下列操作之一：

   * 將以下代碼添加到中的現有文本 **將報告分組** 框中：

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      或者，在本例中：

      ```
      group.0.displayname=Portfolio
      ```

   * 刪除分組的文本模式介面中包含「name」一詞的所有行，然後添加該行：

      ```
      group.0.name=Your Value
      ```

      或者，在本例中：

      ```
      group.0.name=Portfolio
      ```

      您也可以

      ```
      group.0.name
      ```

      行為空，在這種情況下，分組顯示要分組依據的值的名稱。

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. 按一下 **完成**，則 **保存分組**。
