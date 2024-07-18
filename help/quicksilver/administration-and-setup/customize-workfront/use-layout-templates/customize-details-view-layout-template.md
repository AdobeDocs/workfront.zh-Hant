---
title: 使用版面配置範本自訂詳細資料檢視
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作為Workfront管理員，您可以使用版面配置範本來決定當使用者在檢視任務、問題、檔案、計畫或產品組合時選擇左側面板中的詳細資訊區段時會出現哪些資訊。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 使用版面配置範本自訂詳細資料檢視

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

作為Adobe Workfront管理員，您可以使用版面配置範本來決定當使用者在檢視任務、問題、檔案、計畫或投資組合時按一下左側面板中的詳細資訊圖示![](assets/project-details-icon.png)時會出現哪些資訊。

<!--
or billing record
-->

您也可以變更此資訊顯示的順序。 例如，對於您的使用者所看到的所有任務，您可以針對您的使用者所看到的所有任務，將自訂Forms資訊移至詳細資訊檢視的頂端。

如需有關建立版面配置範本的資訊，請參閱[建立和管理版面配置範本](../use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

您對物件的「詳細資訊」檢視所做的變更，也會決定使用者在下列區域中看到的欄位使用狀態和順序：


* 「建立物件」方塊，例如「建立任務」

  ![](assets/new-task-dialog.png)


* 編輯物件時顯示「編輯物件」畫面，例如「編輯任務」、「編輯問題」和「編輯專案」

  ![](assets/edit-task-screen.png)


* 大量編輯物件時顯示「編輯物件」畫面。 目前支援大量編輯專案。

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* 任務與問題清單的摘要![](assets/summary-panel-icon.png)面板

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >版面配置範本的變更只會影響指派給登入使用者的任務和問題，在「摘要」面板中的欄位順序和可用性。

* 「轉換」方塊，例如「將問題轉換為任務」或「將問題轉換為專案」方塊。

  ![將問題轉換為任務方塊](assets/convert-issue-to-task-box.png)

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂使用者在詳細資料檢視中看到的內容

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下&#x200B;**自訂使用者看到的內容**&#x200B;下的向下箭頭![](assets/dropdown-arrow-12x12.png)，然後按一下&#x200B;**專案**、**任務**、**問題**、**方案**&#x200B;或&#x200B;**Portfolio。**
<!--
, or billing record
-->

1. 在&#x200B;**詳細資料**&#x200B;區段中，執行下列任一項作業以自訂使用者在「詳細資料」檢視中看到的內容：

   * 拖曳任何區段標題![](assets/move-icon---dots.png)以變更其順序。
   * 啟用或停用&#x200B;**總覽**&#x200B;和&#x200B;**自訂Forms**&#x200B;下的選項以顯示或隱藏它們。

     如果您隱藏其中一個區段中的所有欄位，則會隱藏整個區段。

     預設會啟用所有欄位。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後繼續修改範本。
