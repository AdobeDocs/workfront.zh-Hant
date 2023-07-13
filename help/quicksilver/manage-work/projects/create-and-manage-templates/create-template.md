---
product-area: templates
navigation-topic: templates-navigation-topic
title: 建立專案範本
description: 您可以從「範本」區域建立和刪除範本。 建立新範本時，您可以為所有任務輸入資訊，並為未來的專案設定輸入所有資訊。 然後，當您從範本建立專案時，此資訊會傳輸到專案。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# 建立專案範本

您可以從「範本」區域建立和刪除範本。 建立新範本時，您可以為所有任務輸入資訊，並為未來的專案設定輸入所有資訊。 然後，當您從範本建立專案時，此資訊會傳輸到專案。

>[!NOTE]
>
>範本及其任務沒有實際日期，而是指出任務可能從哪一天開始（從未來專案可能開始）以及任務可能需要在哪一天完成。 使用範本建立未來的專案時，專案將收到實際日期。 如需詳細資訊，請參閱 [建立專案](../create-projects/create-project.md).


您可以透過下列方式建立新範本：

* 從頭開始，如本文所述。
* 從現有專案，透過將專案儲存為範本。

  如需從現有專案建立範本的詳細資訊，請參閱 [將專案另存為範本](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* 從另一個範本複製它。

  如需複製現有範本的詳細資訊，請參閱 [複製專案範本](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 如果您是Workfront管理員，可以匯入Blueprint來建立範本。 如需詳細資訊，請參閱 [設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

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
   <td> <p>計劃 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">從Blueprint匯入範本的系統管理員</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯範本的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>依預設，您擁有對所建立範本的管理許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 建立範本

1. 從 **主要功能表** ![](assets/main-menu-icon.png) 按一下 **範本**.

1. 按一下 **建立範本**.

   範本未命名。

   ![新增範本](assets/create-template-nwe-2022-350x102.png)

1. 在範本標題中指定新範本的名稱，然後按下 **輸入。**
1. 按一下 **範本任務** 區段。
1. 按一下&#x200B;**開始新增範本任務**.

   或

   按一下 **建立範本任務** 以開始將任務新增至範本。

   將範本任務新增至範本與將任務新增至專案相同。

   如需將任務新增至專案的詳細資訊，請參閱 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >您無法將週期性任務新增至範本。

1. （可選）按一下 **甘特圖** 圖示來檢視範本任務清單的視覺化呈現。

   >[!TIP]
   >
   >您無法直接從此甘特圖編輯任務。

1. 若要新增資訊至新範本，請按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.

   如需有關編輯範本的資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 按一下 **儲存變更**.
1. （可選）如果您想要將其他專案新增至範本，請參閱區段 [新增其他專案至範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) 在文章中 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 由群組關聯決定的範本設定

專案範本與群組（或缺乏群組）的關聯會影響專案、任務和問題偏好設定決定範本中特定設定的方式。 如需詳細資訊，請參閱區段 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) 在文章中 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
