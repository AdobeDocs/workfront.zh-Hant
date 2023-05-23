---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "篩選器：建立引用同一欄位（'AND'語句）的多個篩選器規則"
description: 在標準模式介面中，當嘗試建立引用相同欄位的多個篩選器（使用AND限定符）時，在保存報表並退出報表生成器時，其中一個篩選器將被刪除。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 篩選器：建立引用同一欄位的多個篩選器規則（「AND」語句）

在標準模式介面中，當嘗試建立引用相同欄位的多個篩選器（使用AND限定符）時，在保存報表並退出報表生成器時，其中一個篩選器將被刪除。

**示例：** 您可能只想查看包含「綠色」一詞但名稱中不包含「紅色」一詞的任務。 Adobe Workfront不允許您使用標準模式介面保存以下篩選器規則，因為它引用了相同的欄位（任務名稱），但使用了不同的修飾符，並引用了不同的值：

* 任務名稱>包含>綠色
* 任務名稱>不包含>紅色

但是，可以使用文本模式建立此篩選器。

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

要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 建立引用同一欄位的多個篩選器規則

1. 轉到任務清單。
1. 從 **篩選** 下拉菜單，選擇 **新建篩選器**。
1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 在「為報表設定篩選器規則」區域中，添加以下代碼：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >要構建類似的篩選器，請先生成第一條語句。 例如：
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >根據需要複製並貼上語句多次。 然後，您可以添加需要引用同一欄位的任意多個語句（在本例中為&quot;name&quot;），並對附加語句進行以下修改：
   >
   >1. 在兩個複製行前加上&quot;AND&quot;:1:&quot; 、 &quot;和:2:&quot; 、 &quot;和:3:「 」，等等。
   >1. 將欄位行替換為新欄位值（在&quot;=&quot;符號後）。
   >1. 用新修改量替換修改量行(_Mod)。

   >   
   >這些語句區分大小寫。

1. 按一下 **完成**，則 **保存篩選器**。
