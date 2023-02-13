---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''分組：編輯分組中的顯示名稱'
description: 您可以將群組重新命名為使用者更熟悉的名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 分組：編輯分組中的顯示名稱

您可以將群組重新命名為使用者更熟悉的名稱。

例如，將標準Portfolio名稱分組應用到項目清單時，分組的名稱將顯示為 *Portfolio:名稱：`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

您可以使用文字模式修改此分組，以顯示更容易讀取的名稱。

![](assets/grouping-edited-name-350x160.png)

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

## 編輯分組中的顯示名稱

要更改項目分組中的顯示名稱：

1. 前往專案清單。
1. 從 **分組**&#x200B;下拉式功能表，選取 **新分組**.

1. 按一下 **添加分組**，然後開始在 **首先：** 欄位，然後在清單中顯示時選取它。

1. 按一下 **切換到文本模式**.
1. 執行下列任一操作：

   * 將下列程式碼新增至 **將報表分組** 框：

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      或者，在這種情況下：

      ```
      group.0.displayname=Portfolio
      ```

   * 刪除分組的文本模式介面中包含「name」字的所有行，然後添加該行：

      ```
      group.0.name=Your Value
      ```

      或者，在這種情況下：

      ```
      group.0.name=Portfolio
      ```

      您也可以將

      ```
      group.0.name
      ```

      行空白，則分組會顯示要分組依據的值名稱。

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. 按一下 **完成**，然後 **儲存分組**.
