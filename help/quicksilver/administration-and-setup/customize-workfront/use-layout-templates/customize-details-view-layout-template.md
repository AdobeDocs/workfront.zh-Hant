---
title: 使用版面配置範本自訂詳細資料檢視
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作為Workfront管理員，您可以使用版面配置範本來決定當使用者在檢視任務、問題、檔案、方案或產品組合時選擇左側面板中的詳細資訊區段時會顯示哪些資訊。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: c5053b78dd80fe9017ba96e193e59fbd9b17e7c8
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 使用版面配置範本自訂詳細資料檢視

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

作為Adobe Workfront管理員，您可以使用版面配置範本來決定當使用者按一下「詳細資訊」圖示時會出現哪些資訊 ![](assets/project-details-icon.png) 檢視任務、問題、檔案、計畫或投資組合時，於左側面板中檢視。

<!--
or billing record
-->

您也可以變更此資訊出現的資訊順序。 例如，對於使用者看到的所有任務，您可以針對使用者看到的所有任務，將自訂Forms資訊移動到詳細資訊檢視的頂端。

如需有關建立版面範本的資訊，請參閱 [建立和管理版面範本](../use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

設定版面範本後，您必須將其指派給使用者，才能讓其他人看見您所做的變更。 如需將版面配置範本指派給使用者的詳細資訊，請參閱 [將使用者指派至版面配置範本](../use-layout-templates/assign-users-to-layout-template.md).

您對物件的「詳細資訊」檢視所做的變更，也會決定使用者在下列區域中看到的欄位可用性與順序：

<!-- the New box is not affected by the LT yet. Might be in the future. Commenting this one out for now: 
* "New object" boxes, such as New Task and New Issue

  ![](assets/new-task-dialog.png)

-->

* 「編輯物件」畫面，例如「編輯任務」、「編輯問題」和「編輯專案」

  ![](assets/edit-task-screen.png)


* 大量編輯物件時，「編輯物件」畫面會顯示。 目前支援大量編輯專案。

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* 摘要 ![](assets/summary-panel-icon.png) 任務和問題清單面板

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >版面配置範本的變更只會影響指派給登入使用者的任務和問題在「摘要」面板中的欄位順序和可用性。

* 轉換方塊，例如「將問題轉換為任務」或「將問題轉換為專案」方塊。

  ![將問題轉換為任務方塊](assets/convert-issue-to-task-box.png)

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
若要為群組執行這些動作，您必須是該群組的管理員</p> <p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂使用者在詳細資料檢視中看到的內容

1. 開始使用版面範本，如所述 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下向下箭頭 ![](assets/dropdown-arrow-12x12.png) 在 **自訂使用者看到的內容**，然後按一下 **專案**， **任務**， **問題**， **計畫**，或 **Portfolio。**
<!--
, or billing record
-->

1. 在 **詳細資料** 區段，執行下列任一項作業來自訂使用者在「詳細資訊」檢視中看到的內容：

   * 拖曳任何區段標題 ![](assets/move-icon---dots.png) 以變更其順序。
   * 啟用或停用下方的選項 **概觀** 和 **自訂Forms** 以顯示或隱藏它們。

     如果您隱藏其中一個區段中的所有欄位，則會隱藏整個區段。

     預設會啟用所有欄位。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後繼續稍後修改範本。
