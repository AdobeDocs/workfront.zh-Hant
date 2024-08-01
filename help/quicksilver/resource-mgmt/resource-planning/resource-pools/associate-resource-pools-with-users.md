---
product-area: resource-management
navigation-topic: resource-pools
title: 將資源集區與使用者建立關聯
description: 您必須先建立資源集區，然後才能將其與使用者建立關聯。 當您建立資源集區時，可以將使用者與資源集區相關聯。
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# 將資源集區與使用者建立關聯

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

資源集區是使用者的集合，可協助您管理Adobe Workfront中的資源。

您必須先建立資源集區，然後才能將其與使用者建立關聯。

當您建立資源集區時，可以將使用者與資源集區相關聯。

如果您建立資源集區時沒有將使用者填入集區，則以後在編輯或建立新使用者時，可以將其與使用者相關聯。

如需有關資源集區的資訊，請參閱[資源集區概觀](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

如需有關建立資源集區的資訊，請參閱[建立資源集區](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

## 存取需求

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
   <td> <p>編輯對資源管理的存取權，包括管理資源集區的存取權</p> <p>編輯專案、範本和使用者的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理您與資源集區建立關聯的專案、範本和使用者的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 將資源集區與一個使用者建立關聯

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**使用者**。
1. 勾選清單中使用者名稱旁的方塊，然後按一下&#x200B;**編輯**。
1. 按一下&#x200B;**資源規劃**。
1. 在&#x200B;**資源集區**&#x200B;欄位中，開始輸入您想要與使用者建立關聯的資源集區名稱，然後在其出現時從清單中選取它。\
   您可以將多個資源集區與一個使用者建立關聯。\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 按一下「**儲存變更**」。

如需有關編輯使用者的詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

如需有關建立新使用者的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 大量建立資源集區與使用者的關聯

您可以大量編輯多個使用者，並同時將相同的資源集區與它們全部關聯。

若要將資源集區與數個使用者大量關聯：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**使用者**。
1. 選取清單上的數個使用者，然後按一下[編輯]。****
1. 按一下&#x200B;**資源規劃**。
1. 開始在&#x200B;**資源集區**&#x200B;欄位中輸入您想要與使用者關聯的資源集區名稱，然後在其出現時從清單中選取它。\
   您可以將多個資源集區與多個使用者建立關聯。

   >[!NOTE]
   >
   >此欄位中只會顯示所有選取使用者共用的資源集區。 如果選取的使用者沒有共用資源集區，則此欄位為空白。 如果此欄位空白，您在此指定的資源集區將會覆寫其個別資源集區。

1. 按一下「**儲存變更**」。

如需有關如何大量編輯使用者的詳細資訊，請參閱[大量編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)。
