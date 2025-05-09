---
product-area: templates
navigation-topic: templates-navigation-topic
title: 建立專案範本
description: 您可以從「範本」區域建立及刪除範本。 建立新範本時，您可以為所有任務和未來專案設定輸入資訊。 然後，此資訊將傳輸至您從範本建立的任何專案。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 2%

---

# 建立專案範本

<!-- Audited: 1/2024 -->

您可以從「範本」區域建立及刪除範本。 建立新範本時，您可以為所有任務和未來專案設定輸入資訊。 然後，此資訊將傳輸至您從範本建立的任何專案。

>[!NOTE]
>
>範本及其任務沒有實際日期，而是指出任務可能從哪一天（從未來專案可能開始的時間）開始，以及任務可能需要在哪一天完成。 使用範本來建立未來專案時，專案將收到實際日期。 如需詳細資訊，請參閱[建立專案](../create-projects/create-project.md)。


您可以透過下列方式建立新範本：

* 從頭開始，如本文所述。
* 從現有專案，透過將專案另存為範本。

  如需從現有專案建立範本的詳細資訊，請參閱[將專案另存為範本](../../../manage-work/projects/manage-projects/save-project-as-template.md)。

* 透過從另一個範本複製它。

  如需有關複製現有範本的詳細資訊，請參閱[複製專案範本](../../../manage-work/projects/create-and-manage-templates/copy-template.md)。

* 透過匯入Blueprint。 您必須是Workfront管理員才能匯入Blueprint。 如需詳細資訊，請參閱[設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準 </p><p>或 </p><p>目前：計畫 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">您必須是系統管理員才能從Blueprint匯入範本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯範本的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>依預設，您擁有您所建立範本的管理許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立範本

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**範本**。

1. 按一下&#x200B;**新增範本**。

   範本未命名。

   ![新範本](assets/create-template-nwe-2022-350x102.png)

1. 在範本標題中指定新範本的名稱，然後按&#x200B;**Enter。**
1. 按一下左側面板中的&#x200B;**範本任務**&#x200B;區段。
1. 按一下&#x200B;**開始新增範本工作**。

   或

   按一下&#x200B;**新增範本任務**&#x200B;以開始新增任務至您的範本。

   將範本任務新增至範本與將任務新增至專案相同。

   如需將任務新增至專案的詳細資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

   >[!NOTE]
   >
   >您無法將週期性任務新增到範本。

1. （選擇性）按一下工作清單右上角的&#x200B;**甘特圖**&#x200B;圖示，檢視範本工作清單的視覺化表示法。

   >[!TIP]
   >
   >您無法直接從此甘特圖編輯任務。

1. 若要新增資訊到您的新範本，請按一下&#x200B;**更多**&#x200B;功能表![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**編輯**。

   如需有關編輯範本的資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

1. 按一下「**儲存變更**」。
1. （選擇性）如果您想要新增其他專案至範本，請參閱文章[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)中的[新增其他專案至範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template)小節。

## 由群組關聯決定的範本設定

專案範本與群組（或缺少群組）的關聯會影響專案、任務和問題偏好設定如何決定範本中的某些設定。 如需詳細資訊，請參閱文章[建立及修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)中的[建立及修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates)小節。
