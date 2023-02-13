---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：顯示父任務'
description: 您可以套用下列任務篩選器以顯示工作任務。 工作任務是可以獨立工作的任務，而不是其他任務的父任務。 在一個示例中，篩選器標識了可能是父代的子任務。 在這種情況下，它們不工作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 篩選：顯示父任務

您可以套用下列任務篩選器以顯示工作任務。 工作任務是可以獨立工作的任務，而不是其他任務的父任務。 在一個示例中，篩選器標識了可能是父代的子任務。 在這種情況下，它們不工作。

>[!TIP]
>
>* 如果您考慮新增多個篩選器至報表，建議您使用Report Builder介面新增所有篩選器，並在新增所有其他篩選規則後按一下「切換至文字模式」 。 然後，您可以為父任務篩選器添加代碼，如上所述。 
* 我們也建議您為「專案名稱」新增分組，讓報告更容易閱讀。 如需將群組新增至報表的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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

## 顯示沒有子項的任務（可以有父項）

您可以將下列篩選器套用至任務報表，以顯示沒有子項的任務。 他們可以有自己的父母，也可以是其他任務的子女。

1. 從 **主菜單** ![](assets/main-menu-icon.png)，按一下 **報表。**

1. 按一下 **新增報表**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則**.
1. 在 **開始鍵入欄位名稱……** 行，開始鍵入 **子代數**.

1. 選擇 **等於（區分大小寫）** 為修改量輸入 **0** 孩子的數量。\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   或

   按一下 **切換到文本模式**，並在文字編輯視窗中複製並貼上下列文字： 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 按一下 **儲存+關閉**.

   這會提取系統中正在執行工作之所有工作的報表。 其中有些任務可能有父項，但它們本身不是父項任務。

## 與父代一起顯示任務（他們可以有子代）

您可以將下列篩選器套用至任務報表，以顯示具有父項的任務，這表示這些任務是子項任務。 但是，這些任務也可能有自己的子項，因為篩選器不會排除其子項。 其他任務的父項任務不視為工作任務。

1. 從 **主菜單** ![](assets/main-menu-icon.png)，按一下**報表。
1. 按一下 **新增報表**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則**.
1. 在 **開始鍵入欄位名稱……** 行，開始鍵入 **父ID**.
1. 選擇 **非空白** ，以取得Advertising Cloud的說明。

   ![](assets/filter-parent-id-not-blank-350x100.png)

   或

   按一下 **切換到文本模式**，並在文字編輯視窗中複製並貼上下列文字： 

   `parentID_Mod=notblank`

1. 按一下 **儲存+關閉**.

   這會提取系統中所有有父項且是這些父項的子項任務的報表。 其中一些任務可能是父項本身。

## 顯示無子項和無父項的任務（獨立任務）

您可以將下列篩選器套用至任務報表，以顯示獨立的工作任務。 這些任務沒有父母，也沒有自己的子女。

1. 從 **主菜單** ![](assets/main-menu-icon.png)，按一下 **報表。**
1. 按一下 **新增報表**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則** 和 **開始鍵入欄位名稱……** 開始鍵入 **子代數** 選取 **等於（區分大小寫）** 為修改量輸入 **0** 孩子的數量。
1. 按一下 **新增其他篩選規則** 和 **開始鍵入欄位名稱……** 開始鍵入 **父ID**，然後選取 **空白**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   或

   按一下「 」，而非步驟6至步驟7 **切換到文本模式** 和在文字編輯視窗中，複製並貼上下列文字： 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 按一下 **儲存+關閉**.

   這會提取系統中沒有父項或子項的所有任務的報表。 這些是獨立的工作任務。
