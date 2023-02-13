---
product-area: templates
navigation-topic: templates-navigation-topic
title: 刪除專案範本
description: 建議您停用您不再使用的範本，而不是刪除範本，以便保留專案的歷史資訊。 如需停用範本的相關資訊，請參閱編輯專案範本。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# 刪除專案範本

建議您停用您不再使用的範本，而不是刪除範本，以便保留專案的歷史資訊。 如需停用範本的相關資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>刪除模板時，不會以任何方式修改使用該模板的項目。 不過，您無法再在專案的「範本」欄位中看到原始範本的名稱。 此外，您無法再以任務視圖查看項目上任務的模板任務的名稱。 刪除與項目最初關聯的模板後，項目上的「模板」欄位和任務上的「模板任務」欄位將保持空白。

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
   <td> <p>編輯對範本的存取，包括對刪除的存取</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理範本的權限，包括刪除範本的權限</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 刪除範本的考量事項

* 附加範本時，新增至專案的工作會保留在專案中。 但是，會刪除與任務相關聯的模板任務資訊。
* 範本的名稱不再列於 **範本** 欄位 **概述** 頁簽。

* 您可以從資源回收筒中恢復最近刪除的模板。 有關從資源回收筒中恢復物料的資訊，請參閱 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 刪除範本

1. 從 **主菜單** ![](assets/main-menu-icon.png)，按一下 **範本**. 這會開啟範本清單

1. 按一下範本名稱左側的核取方塊，然後按一下，以選取您要刪除的範本 **刪除>是，刪除它** 以確認刪除。

   或

   按一下範本的名稱以存取，然後按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) ，然後 **刪除模板>是，刪除它**.

   不再提供範本與專案相關聯。
