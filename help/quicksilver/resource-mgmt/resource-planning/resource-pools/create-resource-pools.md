---
product-area: resource-management
navigation-topic: resource-pools
title: 建立資源集區
description: 資源集區是使用者的集合，可協助您更輕鬆地在Adobe Workfront中管理資源。
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 9%

---

# 建立資源集區 {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="資源集區"
>abstract="資源集區是為了完成一件專案，而需要其同時存在之使用者們的集合。建立資源集區後，您可以將其與專案和範本關聯。"

資源集區是使用者的集合，可協助您更輕鬆地在Adobe Workfront中管理資源。 如需資源集區的詳細資訊，請參閱[資源集區概觀](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯對資源管理的存取權，包括管理資源集區的存取權</p> <p>編輯專案、範本和使用者的存取權</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理您要與資源集區建立關聯的專案、範本和使用者的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立資源集區 {#create-a-resource-pool}

{{step1-to-resourcing}}

1. 按一下左側面板中的&#x200B;**資源集區**。
1. 按一下&#x200B;**新增資源集區**。

   ![資源集區](assets/list-of-resource-pools.png)

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>姓名</strong></td>
      <td>這是資源集區的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明</strong></td>
      <td>這是此資源集區的簡短說明。 例如，您可以指定其使用目的。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>集區成員</strong></td>
      <td><p> 個別新增使用者至資源集區。<br>或<br>一次新增大量使用者至資源集區。 您可以新增下列與使用者或使用者集合相關聯的實體之一：
        <ul>
         <li><strong>團隊</strong>：團隊的所有成員都已新增至資源集區。</li>
         <li><strong>群組</strong>：群組的所有成員都已新增至資源集區。</li>
         <li><strong>角色</strong>：所有與該角色相關聯的使用者都已新增至資源集區。</li>
         <li><strong>公司</strong>：公司中的所有使用者都已新增至資源集區。</li>
        </ul><p>秘訣：您只能新增作用中使用者、團隊、<span>角色、</span>或公司。</p><br>您可能需要在對話方塊中向下捲動才能檢視資源集區中的所有使用者。
        <p>備註：若使用者成為群組、專案團隊、公司的成員，或在群組、專案團隊、公司或工作角色新增至資源集區後，成為工作角色的相關聯者，則新成員不會自動新增至資源集區。 <br>如果使用者屬於您新增的團隊、群組、公司和工作角色，則使用者只會新增一次到資源集區。<br>加入資源集區後停用的使用者在使用者清單中會變暗並標示為停用。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （選擇性）使用&#x200B;**還原**&#x200B;連結來移除透過群組、團隊、公司或工作角色新增的使用者。

   >[!NOTE]
   >
   >資源集區中的使用者數量沒有限制。 不過，我們建議不要將太多使用者新增至資源集區，否則資源管理可能會變成一項挑戰。 使用者清單只會顯示資源集區中的前2,000名使用者，而且會依字母順序列出。

   ![個使用者已新增至資源集區](assets/users-in-resource-pool2.png)

1. （可選）按一下使用者名稱右側的X圖示可移除使用者。 如需有關從資源集區移除使用者的詳細資訊，請參閱[從資源集區移除使用者](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)。
1. （選擇性）使用&#x200B;**搜尋**&#x200B;選項在資源集區中尋找使用者。
1. 按一下「**建立**」。
