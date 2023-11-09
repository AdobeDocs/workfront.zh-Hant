---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 在Experience Manager Assets Essentials整合中使用工作流程
description: 在Experience Manager Assets Essentials整合中使用工作流程
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 706e531be6f6269a927f94fee4d2c37d9367c9af
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# 在Experience Manager Assets整合中使用工作流程

工作流程是一組將Workfront連線至Adobe Experience Manager as a Cloud Service的動作。 Workfront管理員可以在Workfront中設定工作流程，然後將它們指派給專案範本。 使用指派了工作流程的專案範本建立專案時，會觸發工作流程中定義的動作。

>[!NOTE]
>
>工作流程僅適用於Adobe Experience Manager as a Cloud Service整合。 無法將其與Adobe Experience Manager Assets Essentials整合。


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
   <td><p>您必須擁有Experience Manager Assetsas a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。</p><p>您必須擁有Adobe Experience Manager存放庫的寫入許可權。</p>
   </td>
  </tr>
  <tr>
   <td><strong>存取層級設定*</strong>
   </td>
   <td>編輯檔案的存取權
<p>
<strong>注意： </strong>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <strong>建立或修改自訂存取層級</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>物件許可權</strong>
   </td>
   <td>管理專案存取許可權或以上許可權 
<p>
如需請求其他存取許可權的詳細資訊，請參閱 <strong>要求物件的存取權 </strong>.
   </td>
  </tr>
</table>

## 必要條件

開始之前，

* 您的Workfront管理員必須在Adobe Experience Manager整合中設定工作流程。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## 將工作流程新增至範本

您可以將工作流程新增至專案範本。 工作流程將套用至從範本建立的任何專案。

1. 按一下以開啟範本 **範本** 在「主要功能表」中，然後從清單中選取範本。
1. 按一下 **Experience Manager Assets** ，位於左側導覽面板中。

   >[!NOTE]
   >
   >如果左側導覽中看不到Experience Manager Assets區段，表示您的Workfront管理員尚未為貴組織啟用工作流程。 <!--Is this right?-->

1. 在 **選取自動化工作流程欄位的整合**，選取您要用於從此範本建立之專案的工作流程整合。
1. （選用）編輯您想要套用至從此範本建立之專案的任何工作流程值。

   如需特定工作流程的指示，請參閱 [編輯專案中的工作流程值](#edit-workflow-values-in-a-project) 本文章內容。

   只有已在「設定」的Experience Manager區域中啟動的工作流程，才能用於範本或專案。

1. 您的變更會自動儲存。 <!-- do they though??-->

## 將工作流程新增至專案

您可以在建立專案時新增工作流程，或將工作流程新增至現有專案。 在這兩種情況下，您都會使用專案範本來新增工作流程。

### 建立專案時新增工作流程

1. 開始建立專案。

   如需指示，請參閱 [使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. 為專案選取範本時，請選取包含您要用於此專案的工作流程的範本。
1. （選用）編輯專案的任何工作流程值，如所述 [編輯專案中的工作流程值](#edit-workflow-values-in-a-project).

   只有已在「設定」的Experience Manager區域中啟動的工作流程，才能用於範本或專案。


### 將工作流程新增至現有專案

1. 開始新增範本至專案。

   如需指示，請參閱 [將範本附加至專案](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. 為專案選取範本時，請選取包含您要用於此專案的工作流程的範本。
1. （選用）編輯專案的任何工作流程值，如所述 [編輯專案中的工作流程值](#edit-workflow-values-in-a-project).

   只有已在「設定」的Experience Manager區域中啟動的工作流程，才能用於範本或專案。

### 編輯專案中的工作流程值

您可以在專案層級編輯工作流程值。 專案層級工作流程值會覆寫在專案範本上設定的值，這些值會覆寫在Adobe Experience Manager資產整合中設定的預設值。

所有工作流程值都可在下列位置找到：

* 「建立專案」或「編輯專案」視窗的「工作流程」區段。
* 左側導覽的Adobe Experience Manager區段。


  >[!NOTE]
  >
  >如果看不到這些區域，表示您的Workfront管理員尚未為您的組織啟用工作流程。

#### 連結的資料夾

若要編輯連結資料夾的工作流程：

1. 切換 **[!UICONTROL 建立連結的資料夾]** 視需要開啟或關閉。
1. （視條件而定）如果您正在啟用連結的資料夾，請選擇資料夾路徑，以指出所有與此整合相關聯的連結資料夾的位置。
1. 按一下 **[!UICONTROL 儲存]** 如果您使用 [!UICONTROL 建立專案] 或 [!UICONTROL 編輯專案] 視窗。

   或

   如果您在 [!DNL Adobe Experience Manager area]，您的變更會自動儲存。 <!--Do they though?-->


#### 發佈資產

若要編輯資產發佈的工作流程：

1. 切換 **自動發佈資產** 視需要開啟或關閉。
1. （視條件而定）如果您正在啟用發佈，請選取您要發佈至發佈服務、Brand Portal或兩者。
1. 按一下 **[!UICONTROL 儲存]** 如果您使用 [!UICONTROL 建立專案] 或 [!UICONTROL 編輯專案] 視窗。

   或

   如果您在 [!DNL Adobe Experience Manager area]，您的變更會自動儲存。 <!--Do they though?-->


