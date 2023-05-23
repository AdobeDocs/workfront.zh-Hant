---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：顯示父任務'
description: 您可以應用下面的任務篩選器來顯示工作任務。 工作任務是可以獨立工作的任務，不是其他任務的父任務。 在一個示例中，過濾器標識可能是父項本身的子項任務。 在這種情況下，他們不是在工作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 篩選器：顯示父任務

您可以應用下面的任務篩選器來顯示工作任務。 工作任務是可以獨立工作的任務，不是其他任務的父任務。 在一個示例中，過濾器標識可能是父項本身的子項任務。 在這種情況下，他們不是在工作。

>[!TIP]
>
>* 如果您考慮向報表添加多個篩選器，建議您使用報表生成器介面添加所有篩選器，並在添加所有其他篩選器規則後按一下切換到文本模式。 然後，您可以添加父任務篩選器的代碼，如上所述。 
* 我們還建議您為項目名稱添加分組，以便更容易閱讀報告。 有關將分組添加到報表的詳細資訊，請參閱文章 [Adobe Workfront分組概覽](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。
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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改篩選器</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 顯示沒有子項的任務（它們可能具有父項）

您可以將以下篩選器應用於任務報告以顯示沒有子項的任務。 他們可以有自己的父母，也可以是其他任務的子女。

1. 從 **主菜單** ![](assets/main-menu-icon.png)按一下 **報告。**

1. 按一下 **新建報表**。
1. 選擇 **任務報告**。
1. 按一下 **篩選器**。
1. 按一下 **添加篩選器規則**。
1. 在 **開始鍵入欄位名……** 行，開始鍵入 **子代數**。

1. 選擇 **等於（區分大小寫）** 輸入 **0** 孩子的數量。\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   或

   按一下 **切換到文本模式**，並在文本編輯窗口中複製並貼上以下文本： 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 按一下 **保存+關閉**。

   此操作將為系統中正在處理任務的所有任務提取報告。 其中一些任務可能具有父任務，但它們本身不是父任務。

## 與父代一起顯示任務（他們可能有子代）

您可以將以下篩選器應用於任務報告以顯示具有父項的任務，即這些任務是子項任務。 但是，這些任務也可能有自己的子項，因為篩選器不排除其子項。 作為其他任務父項的子項任務不被視為工作任務。

1. 從 **主菜單** ![](assets/main-menu-icon.png)，按一下**報告。
1. 按一下 **新建報表**。
1. 選擇 **任務報告**。
1. 按一下 **篩選器**。
1. 按一下 **添加篩選器規則**。
1. 在 **開始鍵入欄位名……** 行，開始鍵入 **父ID**。
1. 選擇 **不為空** 你的修飾語。

   ![](assets/filter-parent-id-not-blank-350x100.png)

   或

   按一下 **切換到文本模式**，並在文本編輯窗口中複製並貼上以下文本： 

   `parentID_Mod=notblank`

1. 按一下 **保存+關閉**。

   此操作將為系統中具有父代且是這些父代的子任務的所有任務繪製報告。 其中一些任務可能是父項本身。

## 顯示無子代和無父代的任務（獨立任務）

您可以將以下篩選器應用於任務報表以顯示獨立的工作任務。 這些任務沒有父項，也沒有自己的子項。

1. 從 **主菜單** ![](assets/main-menu-icon.png)按一下 **報告。**
1. 按一下 **新建報表**。
1. 選擇 **任務報告**。
1. 按一下 **篩選器**。
1. 按一下 **添加篩選器規則** 在 **開始鍵入欄位名……** 行開始鍵入 **子代數** 選擇 **等於（區分大小寫）** 輸入 **0** 孩子的數量。
1. 按一下 **添加另一個篩選器規則** 在 **開始鍵入欄位名……** 行開始鍵入 **父ID**，然後選擇 **為空**。

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   或

   不要執行步驟6-7，請按一下 **切換到文本模式** 並在文本編輯窗口中複製並貼上以下文本： 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 按一下 **保存+關閉**。

   此操作將為系統中沒有父代或子代的所有任務生成報告。 這些是獨立的工作任務。
