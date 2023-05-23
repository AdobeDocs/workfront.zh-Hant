---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：當狀態與不同組關聯時按相同名稱狀態顯示物料。'
description: 您可以使用3字母鍵NST將任務狀態分配給A組命名的新狀態。 您可能已將另一個任務狀態分配給B組，該任務狀態也名為New Status（新建狀態），其3字母鍵為NES。 儘管2個狀態的名稱可以相同，但3個字母的代碼始終唯一。 有關組狀態的詳細資訊，請參閱建立或編輯組狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 篩選器：在狀態與不同組關聯時按相同名稱狀態顯示物料

您可以將任務狀態分配給已命名的A組 *新建狀態* 帶3個字母的鍵 *NST*。 您可能已將另一個任務狀態分配給B組(也名為 *新建狀態* 帶3個字母的鍵 *NES* 儘管2個狀態的名稱可以相同，但3個字母的代碼始終唯一。\
有關組狀態的詳細資訊，請參閱 [建立或編輯組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

使用篩選器生成器，無法在兩個具有相同名稱的狀態之間進行標識。 必須使用「文本模式」來區分兩個狀態。

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

## 當狀態與不同組關聯時按相同名稱狀態顯示物料

1. 例如，轉到要自定義任務清單的篩選器。\
   這同樣適用於項目和問題。
1. 按一下 **添加篩選器規則** 為 **狀態** 的子菜單。\
   例如，在任務報告中，添加 **狀態等於新狀態**，如果只顯示狀態為 **新建狀態**。

   >[!TIP]
   >
   >請注意，對於名為「新建狀態」的狀態，您只有一個選項。

1. 按一下 **切換到文本模式**。\
   應顯示以下代碼：

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此處僅顯示一個狀態。 狀態行顯示某個狀態的3個字母鍵之一。

1. 添加以下2行代碼以添加篩選器中缺少的狀態：

   <pre>或:1:狀態=NES<br>或:1:status_Mod=in</pre>

1. 按一下 **完成**，則 **保存篩選器**。

   該清單顯示A組中狀態為「新狀態」和B組狀態為「新狀態」的任務。
