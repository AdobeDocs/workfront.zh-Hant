---
product-area: templates
navigation-topic: templates-navigation-topic
title: 建立專案範本
description: 您可以從「範本」區域建立和刪除範本。 建立新模板時，您可以輸入所有任務的資訊以及將來項目設定的所有資訊。 當您從範本建立專案時，此資訊便會傳輸至專案。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# 建立專案範本

您可以從「範本」區域建立和刪除範本。 建立新模板時，您可以輸入所有任務的資訊以及將來項目設定的所有資訊。 當您從範本建立專案時，此資訊便會傳輸至專案。

您可以透過下列方式建立新範本：

* 從頭開始，如本文所述。
* 從現有專案，將專案儲存為範本。

   如需從現有專案建立範本的詳細資訊，請參閱 [將專案儲存為範本](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* 從其他範本複製。

   如需複製現有範本的詳細資訊，請參閱 [複製專案範本](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 如果您是Workfront管理員，則可以通過導入Blueprint來建立模板。 如需詳細資訊，請參閱 [設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 存取需求

您必須具備下列條件：

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
   <td> <p>計劃 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">從Blueprint導入模板的系統管理員</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯範本的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>預設情況下，您擁有所建立模板的「管理」權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立範本

1. 從 **主菜單** ![](assets/main-menu-icon.png) 按一下 **範本**.

1. 按一下 **新範本**.

   範本未命名。

   ![新範本](assets/create-template-nwe-2022-350x102.png)

1. 在範本標題中指定新範本的名稱，然後按 **輸入。**
1. 按一下 **模板任務** 區段。
1. 按一下&#x200B;**開始添加模板任務**.

   或

   按一下 **新模板任務** 開始向模板添加任務。

   將範本任務新增至範本與將任務新增至專案相同。

   如需新增工作至專案的詳細資訊，請參閱 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >無法將循環任務添加到模板。

1. （選用）按一下 **甘特圖** 表徵圖，查看模板任務清單的可視表示。

   >[!TIP]
   >
   >不能直接從此甘特圖編輯任務。

1. 若要將資訊新增至新範本，請按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.

   如需編輯範本的相關資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 按一下 **儲存變更**.
1. （選用）如果您想要新增其他項目至範本，請參閱區段 [新增其他項目至範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) 在文章中 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 由群組關聯決定的範本設定

項目模板與組的關聯（或缺少它們）會影響項目、任務和問題首選項如何確定模板中的某些設定。 如需詳細資訊，請參閱 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) 在文章中 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
