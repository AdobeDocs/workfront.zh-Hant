---
product-area: resource-management
navigation-topic: resource-pools
title: 從資源集區中移除使用者
description: 雖然資源集區中的使用者數量沒有限制，但使用者清單只會顯示前2000位使用者（按字母順序列出）。
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: 00afc0cbc58fce34059302dfeb8847cfacb9c7e4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# 從資源集區中移除使用者

{{highlighted-preview}}

雖然資源集區中的使用者數量沒有限制，但使用者清單只會顯示前2000位使用者（按字母順序列出）。

建議您移除已停用或已移動角色或部門的使用者，以確保您在所有資源集區中一律擁有精確的使用者清單。

如需資源集區的詳細資訊，請參閱[資源集區概觀](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>專業及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對資源管理的存取權，包括管理資源集區的存取權</p> <p>檢視或更高的使用者存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 從資源集區移除使用者

當資源集區中不再需要這些使用者時，您可以從資源集區中移除這些使用者。

若要從資源集區移除使用者：

{{step1-to-resourcing}}

1. 按一下左側面板中的&#x200B;**資源集區**。
1. 選取資源集區，然後按一下&#x200B;**編輯**。
或\
   按一下資源集區的名稱。

1. 開始在&#x200B;**搜尋此資源集區**&#x200B;欄位中輸入您要移除的使用者名稱。\
   或\
   如果您想要移除與這些實體相關聯的所有使用者，請開始輸入公司、工作角色、團隊或群組的名稱。

   <span class="preview">預覽環境中的範例影像：<span>
   <span class="preview">![從資源集區移除使用者](assets/remove-users-from-resource-pool.png)<span>

   生產環境中的影像範例：
   ![搜尋資源集區](assets/search-inside-new-resource-pool-350x314.png)

1. 按一下使用者層級的「x」圖示，從資源集區移除使用者。 它們會從所有出現的清單中移除。\
   或\
   若要移除與工作角色、群組、團隊或公司相關聯的所有使用者，請按一下工作角色、群組、團隊或公司層級的&#x200B;**移除**。 這會從資源集區中移除與該工作角色、群組、團隊或公司相關聯的所有使用者。

1. 按一下「**儲存**」。
