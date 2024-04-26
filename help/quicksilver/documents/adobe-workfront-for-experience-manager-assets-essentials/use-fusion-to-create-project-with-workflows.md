---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 使用Workfront Fusion建立具有Adobe Experience Manager工作流程的Workfront專案
description: 如果您透過Workfront Fusion建立專案，並想在專案中加入Adobe Experience Manager工作流程，您必須使用特定的Fusion模組設定，如本文所述。
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 13f689c4ee404c07be6b9cf9c526bef8dca878ff
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 使用Workfront Fusion將Workfront問題轉換為包含Adobe Experience Manager工作流程的專案

如果您透過Workfront Fusion建立專案，並想在專案中加入Adobe Experience Manager工作流程，您必須使用特定的Fusion模組設定，如本文所述。

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
   <td><b>Adobe Experience Manager<b>：
   <ul>
   <li>
   <p>您必須擁有Experience Manager Assetsas a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。</p>
   </li
   ><li>
   <p>您必須擁有Adobe Experience Manager存放庫的寫入許可權。</p>
   </li>
   </ul>
  <b>Workfront Fusion</b>：<p>新增：</p>
   <ul>
   <li>
   <p>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p>
   </li>
   <li> 
   <p>[！UICONTROL Ultimate] [!DNL Workfront] 計畫： [!DNL Workfront Fusion] 已包括在內。</p>
   </li>
   </ul>
   <p>或</p>
   <p>目前：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p>
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
</table>

## 先決條件

開始之前，

* 您的Workfront管理員必須在Adobe Experience Manager整合中設定工作流程。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* 您必須使用Adobe Experience Manager整合連結資料夾工作流程來設定專案範本。
* 您必須在Workfront中建立OAuth應用程式，才能設定此模組的連線。

  如需指示，請參閱 [建立Oauth應用程式](#create-an-oauth-application) 本文章內容。

## 模組設定

在Workfront Fusion中，如果您想要建立包含Adobe Experience Manager工作流程的專案，必須使用「Workfront >其他動作」模組。

1. 新增 **Workfront** > **其他動作** 模組至您的情境。
1. 在 **連線** 欄位中，選取連線至此模組將使用之帳戶的Workfront連線。

   如需建立連線的指示，請參閱 [連線 [!DNL Workfront] 至 [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) 在Workfront模組文章中。

   如需建立使用者端ID和使用者端密碼的指示，請參閱建立連線。 [建立Oauth應用程式](#create-an-oauth-application) 本文章內容。

1. 在 **記錄型別** 欄位，選取 `Issue`.
1. 在 **動作** 欄位，選取 `convertToProject`.
1. 在 **ID** 欄位，輸入或對應您要轉換為專案的問題的ID。
1. 啟用 **顯示進階設定**.
1. 捲動至模組底部，然後找出 **專案（進階集合）** 欄位。
1. 將下列文字貼入 **專案（進階集合）** 欄位。

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. 取代 `Folder tree ID here` 資料夾ID識別碼。

   若要尋找資料夾樹狀結構ID，請參閱 [尋找資料夾樹狀目錄ID](#locate-folder-tree-ids) 本文章內容。

   若要使用多個資料夾樹狀結構，請使用逗號分隔ID：

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. 取代 `New project name here` 與新專案將具有的名稱。
1. 取代 `Template ID here` ，並使用您用於新專案的範本ID。

   您可以從先前的模組(例如「Workfront >搜尋模組」)對應範本ID，或在Workfront中範本頁面的URL中找到它。

1. 按一下 **確定** 以儲存模組組態。

## 尋找資料夾樹狀目錄ID

若要尋找資料夾樹狀結構ID：

>[!NOTE]
>
>這些指示會使用Chrome瀏覽器。

1. 在Workfront中，開啟您要用於此專案的範本。 此範本必須包含您想用於專案的Adobe Experience Manager設定。
1. 開啟瀏覽器的開發人員工具。
1. 開啟 **網路** 定位字元。
1. 在 **篩選** 方塊，輸入 `object-workflow`.
1. 在「名稱」欄中，按一下出現的英數ID。

   ![尋找資料夾ID 1](assets/finding-folder-id-1.png)

1. 按一下 **預覽** 定位鍵移至英數字元ID右側。
1. 開啟下列收合的部分：
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   每個資料夾樹狀結構都以數字表示。 0 （零）代表清單中的第一個資料夾，1代表第二個資料夾，依此類推。 如果範本只包含一個資料夾樹狀結構，則編號為0。

1. 開啟您要用於新專案的資料夾樹狀結構。 記下 `_id` 欄位值。 如果您要使用多個資料夾樹狀結構，請記下所有 `_id` 要使用的資料夾樹狀結構的欄位值。

   ![尋找資料夾ID 2](assets/finding-folder-id-2.png)

   這些是 `aemNativeFolderTreeIDs`  您將會輸入至的值 **專案（進階集合）** 中的欄位 **Workfront** > **其他動作** Fusion模組

## 建立Oauth應用程式

您必須在Workfront中設定OAuth應用程式，以便此模組連線。 您只需要對Fusion中的指定Workfront連線執行此操作一次。

1. 在Workfront中，開始建立OAuth應用程式，如所述 [使用使用者認證建立OAuth2應用程式（授權代碼流程）](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) 在文章中建立OAuth2應用程式 [!DNL Workfront] 整合。
1. 將使用者端ID和使用者端密碼複製到安全位置。
1. 在 **重新導向URI** 欄位，輸入下列內容：

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. 按一下「**儲存**」。

在Fusion中設定模組的連線時，您將使用此使用者端ID和使用者端密碼。

如需建立連線的指示，請參閱 [連線 [!DNL Workfront] 至 [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) 在Workfront模組文章中。

