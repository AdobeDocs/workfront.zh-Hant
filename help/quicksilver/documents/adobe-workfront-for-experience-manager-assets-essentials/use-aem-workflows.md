---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 使用Experience Manager Assets Essentials整合中的工作流程
description: 使用Experience Manager Assets Essentials整合中的工作流程
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 038f5f3c941ea69feb43492a30b5abea39f7c932
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 在Experience Manager Assets整合中使用工作流程

工作流程是連線Workfront和Adobe Experience Manager as a Cloud Service的一組動作。 Workfront管理員可以在Workfront中設定工作流程，然後將其指派至專案範本。 使用已為其分配工作流的項目模板建立項目時，將觸發工作流中定義的操作。

>[!NOTE]
>
>工作流程僅適用於Adobe Experience Manager as a Cloud Service整合。 無法與Adobe Experience Manager Assets Essentials整合使用。


## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>Adobe Workfront計畫*</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權*</strong>
   </td>
   <td>要求或更高版本
   </td>
  </tr>
  <tr>
   <td><strong>產品</strong>
   </td>
   <td><p>您必須有Experience Manager Assetsas a Cloud Service或Assets Essentials，且您必須以使用者身分新增至產品中的Admin Console。</p><p>您必須擁有Adobe Experience Manager中存放庫的寫入存取權，才能建立連結的資料夾。</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>訪問級別配置*</strong>
   </td>
   <td>編輯對文檔的訪問
<p>
<strong>注意： </strong>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <strong>建立或修改自訂存取層級</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>物件權限</strong>
   </td>
   <td>管理項目上的訪問權限或更高 
<p>
有關請求其他訪問的資訊，請參閱 <strong>請求對對象的訪問 </strong>.
   </td>
  </tr>
</table>

## 必要條件

開始之前，

* 您的Workfront管理員必須在Adobe Experience Manager整合中設定工作流程。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## 將工作流程新增至範本

您可以將工作流程新增至專案範本。 工作流程將套用至從範本建立的任何專案。

1. <!-- main menu snippet??--> 按一下以開啟範本 **範本** 在「主菜單」中，然後從清單中選擇模板。
1. 按一下 **Experience Manager Assets** ，即可取得Advertising Cloud的說明。

   >[!NOTE]
   >
   >如果左側導覽中未顯示Experience Manager Assets區段，表示您的Workfront管理員尚未啟用貴組織的工作流程。 <!--Is this right?-->

1. 在 **選取自動化工作流程欄位的整合**，請選取與您要用於此範本所建立專案之工作流程的整合。
1. （可選）編輯要應用於從此模板建立的項目的任何工作流值。

   例如，要在預設值以外的位置建立連結的資料夾，請輸入連結的資料夾位置。

   範本或專案中僅提供已在「設定」的「Experience Manager」區域中啟動的工作流程。

1. 您的變更會自動儲存。 <!-- do they though??-->

## 新增工作流程至專案

您可以在建立專案時新增工作流程，或將工作流程新增至現有專案。 在這兩種情況下，您都將使用專案範本來新增工作流程。

### 建立專案時新增工作流程

1. 開始建立專案。

   如需指示，請參閱 [使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. 選取專案的範本時，選取包含您要用於此專案的工作流程的範本。
1. （選用）編輯專案的任何工作流程值，如 [編輯專案中的工作流程值](#edit-workflow-values-in-a-project).

   範本或專案中僅提供已在「設定」的「Experience Manager」區域中啟動的工作流程。


### 將工作流程新增至現有專案

1. 開始將範本新增至專案。

   如需指示，請參閱 [將範本附加至專案](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. 選取專案的範本時，選取包含您要用於此專案的工作流程的範本。
1. （選用）編輯專案的任何工作流程值，如 [編輯專案中的工作流程值](#edit-workflow-values-in-a-project).

### 編輯專案中的工作流程值

您可以編輯專案層級的工作流程值。 專案層級工作流程值會覆寫專案範本上設定的值，而覆寫Adobe Experience Manager Assets整合中設定的預設值。

所有工作流程值都可在以下位置找到：

* 「建立項目」或「編輯項目」窗口的「工作流」部分。
* 左側導覽的Adobe Experience Manager區段。


   >[!NOTE]
   >
   >如果這些區域未顯示，表示您的Workfront管理員尚未為您的組織啟用工作流程。

#### 連結的資料夾

要編輯連結資料夾的工作流，請執行以下操作：

1. 切換 **[!UICONTROL 建立連結的資料夾]** 開啟。
1. 選擇資料夾路徑，以指出您要將所有連結資料夾與這項整合相關聯的位置。
1. 如果使用「建立項目」或「編輯項目」窗口，請按一下「保存」。

   或

   如果您位在Adobe Experience Manager區，您的變更會自動儲存。 <!--Do they though?-->

