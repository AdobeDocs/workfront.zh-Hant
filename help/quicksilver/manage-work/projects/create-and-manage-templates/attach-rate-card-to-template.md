---
content-type: overview
product-area: templates
navigation-topic: financials
title: 將費率卡附加至範本
description: 當您指定費率卡至範本時，費率卡會附加至從範本建立的所有專案。
author: Lisa
feature: Work Management
source-git-commit: ca2effb6674caf3a1b44f675a23758f734332a01
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 3%

---

# 將費率卡附加至範本

{{highlighted-preview-article-level}}

當您指定費率卡至範本時，費率卡會附加至從範本建立的所有專案。 費率卡會成為專案的預設值，但可視需求加以覆寫。

如需關於費率卡的資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

如需有關專案範本的資訊，請參閱[專案範本概觀](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯範本的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理費率卡的許可權以及編輯收費率的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須在Workfront中建立要指派給範本的費率卡。 如需詳細資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

必須為配置範本上的範本啟用&#x200B;**費率卡**&#x200B;欄位。

1. 在版面配置範本中，按一下&#x200B;**自訂使用者看到的內容**&#x200B;下的向下箭頭，然後按一下&#x200B;**範本**。
1. 在&#x200B;**詳細資料**&#x200B;區段中，選取&#x200B;**總覽**&#x200B;區域中的&#x200B;**費率卡**&#x200B;欄位。

   如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

## 將費率卡附加至範本

{{step1-to-templates}}

1. 建立新範本或編輯現有範本。
1. 在「範本詳細資料>總覽>範本關聯」區段中，在&#x200B;**費率卡**&#x200B;欄位中選取費率卡。

   只有您有許可權的費率卡才可供選擇。
您可以開始輸入費率卡的名稱，以縮小結果清單。

   ![在範本上選取費率卡](assets/select-rate-card-on-template.png)

1. 完成編輯後儲存範本。

   如需建立範本的詳細資訊，請參閱[建立專案範本](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)。

   如需有關編輯範本的詳細資訊，請參閱[編輯專案範本](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)。

## 套用範本至專案

1. 使用範本建立專案。

   從範本建立專案的方法有很多種。 如需詳細資訊，請參閱下列文章：

   * [使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [將任務轉換為專案](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [將問題轉換為專案](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   費率卡會自動儲存在專案上。 在[新增專案]方塊的[概觀] > [專案關聯]區段中，您可以移除費率卡，或在&#x200B;**費率卡**&#x200B;欄位中選取不同的費率卡。

   ![範本的費率卡出現在專案詳細資料上](assets/create-project-from-template-rate-card.png)

   費率卡及其相關費率會顯示在專案費率區域中。

   您也可以從專案移除費率卡，或在「費率」區域中附加不同的費率卡。 如需詳細資訊，請參閱[將費率卡附加至專案](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)。

   ![從專案](assets/template-rates-on-project.png)上的範本評等卡片

   >[!NOTE]
   >
   >如果範本上有個別費率，且費率卡也附加至範本，則當您從範本建立專案時，個別費率卡和費率卡都會出現在費率清單中。

1. （選擇性）若要將費率卡套用至現有專案，請將範本附加至專案。

   當您在範本預覽上使用&#x200B;**自訂並附加**&#x200B;選項時，可以在[附加範本] > [選項]區段中選取&#x200B;**費率卡**&#x200B;專案，以將費率卡新增至專案。 清除核取方塊，以排除費率卡不轉帳至專案。

   如需詳細資訊，請參閱[將範本附加至專案](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

1. （選擇性）若要將費率卡從特定專案儲存至範本，請將專案另存為範本。

   在「另存為範本」方塊的「選項」區段中，您可以選取&#x200B;**費率卡**&#x200B;專案，以將費率卡新增至範本。 清除核取方塊，以排除費率卡無法傳輸至範本。

   如需詳細資訊，請參閱[將專案另存為範本](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md)


