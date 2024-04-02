---
product-area: templates
navigation-topic: templates-navigation-topic
title: 刪除專案範本
description: 我們建議您停用不再使用的範本，而不是刪除它們，以便您可以保留有關您專案的長期歷史資訊。 如需關於停用範本的資訊，請參閱編輯專案範本。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 7bef757c24adc7791cb3b258ae6c33f3c0eec818
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 刪除專案範本

我們建議您停用不再使用的範本，而不是刪除它們，以便您可以保留有關您專案的長期歷史資訊。 如需停用範本的相關資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>當您刪除範本時，使用該範本的專案不會以任何方式修改。 不過，您不會再在專案的「範本」欄位中看到原始範本的名稱。 此外，您無法再在任務檢視中檢視專案上任務的範本任務名稱。 刪除最初與專案關聯的範本後，專案上的範本欄位和任務上的範本工作列位保持空白。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯包含刪除許可權的範本存取權</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理範本的許可權，包括刪除範本的許可權</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 刪除範本的考量事項

* 當範本附加時新增到專案中的任務仍保留在專案上。 但是，與任務關聯的範本任務資訊會被刪除。
* 範本的名稱不再列於 **範本** 欄位於 **概觀** 專案的子標籤。

* 您可以從資源回收筒復原最近刪除的範本。 如需有關從資源回收筒復原專案的資訊，請參閱 [還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 刪除範本

{{step1-to-templates}}

這會開啟範本清單

1. 按一下範本名稱左邊的核取方塊，然後按一下，以選取您要刪除的範本 **刪除>是，刪除** 以確認刪除。

   或

   按一下範本名稱以存取它，然後按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) ，然後 **刪除範本>是，刪除它**.

   範本無法再與專案建立關聯。
