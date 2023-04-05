---
title: 使用版面範本自訂「詳細資料」檢視
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Workfront管理員，您可以使用版面範本來判斷當使用者在檢視工作、問題、檔案、方案或產品組合時，選取左側面板的「詳細資訊」區段時，會顯示哪些資訊。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 92fb1ee0b641d2f4b527e17df272e4c37c0feaef
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 使用版面範本自訂「詳細資料」檢視

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

身為Adobe Workfront管理員，您可以使用配置範本，判斷使用者按一下「詳細資訊」圖示時會顯示哪些資訊 ![](assets/project-details-icon.png) 在左側面板中查看任務、問題、文檔、程式或產品組合。

<!--
or billing record
-->

您也可以變更顯示此資訊的資訊順序。 例如，對於您的使用者看到的所有工作，您可以將自訂Forms資訊移至使用者看到之所有工作的詳細資料檢視頂端。

您對物件的「詳細資訊」檢視所做的變更，也會決定使用者在下列區域中看到之欄位的可用性和順序：

* 「新對象」框，如「新任務」和「新問題」

   ![](assets/new-task-dialog.png)

* 「編輯對象」螢幕，如「編輯任務」、「編輯問題」和「編輯項目」

   ![](assets/edit-task-screen.png)


* 批量編輯對象時，「編輯對象」螢幕會顯示。 目前，大量編輯專案支援此功能。

   ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* 摘要 ![](assets/summary-panel-icon.png) 任務和問題清單面板

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >版面範本的變更只會影響指派給登入使用者之工作和問題的「摘要」面板中欄位的順序和可用性。

* 「轉換」方塊，例如「將問題轉換為任務」或「將問題轉換為專案」方塊。

   ![將問題轉換為任務框](assets/convert-issue-to-task-box.png)

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂使用者在「詳細資訊」檢視中看到的內容

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下向下箭頭 ![](assets/dropdown-arrow-12x12.png) 在 **自訂使用者看見的項目**，然後按一下 **專案**, **任務**, **問題**, **方案**，或 **Portfolio。**
<!--
, or billing record
-->

1. 在 **詳細資料** 區段，執行下列任一操作以自訂使用者在「詳細資料」檢視中看到的內容：

   * 拖曳任何區段標題 ![](assets/move-icon---dots.png) 來改變他們的順序。
   * 在下啟用或停用選項 **概述** 和 **自訂Forms** 來顯示或隱藏。

      如果隱藏其中一個區段中的所有欄位，則會隱藏整個區段。

      預設會啟用所有欄位。

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後稍後繼續修改範本。
