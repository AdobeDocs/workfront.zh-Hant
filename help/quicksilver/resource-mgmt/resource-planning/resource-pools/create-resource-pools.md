---
product-area: resource-management
navigation-topic: resource-pools
title: 建立資源池
description: 資源池是用戶的集合，可幫助您更輕鬆地在Adobe Workfront中管理資源。 有關資源池的詳細資訊，請參閱資源池概述。
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---

# 建立資源池

資源池是用戶的集合，可幫助您更輕鬆地在Adobe Workfront中管理資源。 有關資源池的詳細資訊，請參見 [資源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對資源管理的訪問，包括對管理資源池的訪問</p> <p>編輯使用者、專案和範本的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理要將資源池與</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立資源池 {#create-a-resource-pool}

1. 以具有編輯資源池訪問權限的用戶身份登錄。\
   如需詳細資訊，請參閱 [建立資源池](#create-a-resource-pool).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **資源**.
1. 按一下 **資源池** 中。\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. 按一下 **新資源池**.
1. 指定下列項目：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名稱</strong></td>
      <td>這是資源池的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明</strong></td>
      <td>以下是有關此資源池的簡短說明。 例如，您可以指定該使用目的。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>集區成員</strong></td>
      <td><p> 將用戶單獨添加到資源池。<br>或 <br>一次將大量用戶添加到資源池。 您可以新增下列與使用者或使用者集合相關聯的實體之一：
        <ul>
         <li><strong>團隊</strong>:該組的所有成員都添加到資源池。</li>
         <li><strong>群組</strong>:組的所有成員都添加到資源池。</li>
         <li><strong>角色</strong>:與該角色關聯的所有用戶都將添加到資源池。</li>
         <li><strong>公司</strong>:公司中的所有用戶都添加到資源池。</li>
        </ul><p>提示：您只能新增作用中使用者、團隊、 <span>角色，</span> 或公司。</p><p>注意：如果用戶成為組、組、公司的成員，或在組、組、公司或作業角色被添加到資源池後與作業角色關聯，則新成員不會自動添加到資源池。 <br>如果用戶屬於您添加的團隊、組、公司和作業角色，則同時，該用戶只被添加到資源池一次。<br>已新增至資源池後已停用的使用者，在使用者清單中會呈現灰色，並標示為停用。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （選用）使用 **還原** 連結以移除透過群組、團隊、公司或工作角色新增的使用者。

   >[!NOTE]
   >
   >資源池中可以有多少用戶沒有限制。 但是，我們建議不要向資源池添加太多用戶，因為如果不添加資源管理，可能會成為一項挑戰。 用戶清單只顯示資源池中的前2,000個用戶，並按字母順序列出。

   ![Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. （選用）按一下使用者名稱右側的X圖示來移除使用者。 有關從資源池中刪除用戶的詳細資訊，請參見 [從資源池中刪除用戶](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. （選用）使用 **搜尋** 在資源池中查找用戶的選項。
1. 按一下 **建立**。
