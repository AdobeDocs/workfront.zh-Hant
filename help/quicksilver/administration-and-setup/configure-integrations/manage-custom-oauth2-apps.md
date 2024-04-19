---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: 檢視及管理自訂OAuth2應用程式
description: 身為Adobe Workfront管理員，您可以檢視及管理您Workfront執行個體的OAuth2應用程式，此應用程式可讓其他應用程式存取Workfront。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# 檢視及管理自訂OAuth2應用程式

作為 [!DNL Adobe Workfront] 管理員，您可以檢視和管理執行個體的OAuth2應用程式 [!DNL Workfront]，可允許其他應用程式存取 [!UICONTROL Workfront].

>[!NOTE]
>
>* 在OAuth2的上下文中，「Oauth2應用程式」是指應用程式和伺服器之間的這類存取連結，例如 [!DNL Workfront]. 如需詳細資訊，請參閱 [建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* 您一次最多可以有十個OAuth2應用程式。

* 如需建立自訂OAuth2應用程式的詳細資訊，請參閱 [建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* 如需有關設定和搭配使用者認證（授權碼流程）使用OAuth2應用程式的指示，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 如需使用PKCE設定和使用OAuth2應用程式的指示，請參閱 [使用PKCE流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL Plan]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 您必須是 [!DNL Workfront] 管理員。 </p>
    <p>有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 先決條件

您必須建立 [!UICONTROL OAuth2] 應用程式，您才能檢視或管理它們。

如需詳細資訊，請參閱 [建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 管理自訂OAuth2應用程式

* [檢視和編輯自訂OAuth2應用程式](#view-and-edit-custom-oauth2-applications)
* [刪除自訂OAuth2應用程式](#delete-custom-oauth2-applications)

### 檢視和編輯自訂OAuth2應用程式 {#view-and-edit-custom-oauth2-applications}

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 將游標暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** ![](assets/edit-icon.png) 當它出現在最右邊時。
1. （選用）編輯應用程式的任何詳細資訊。

   如需與OAuth2和JWT應用程式相關的欄位，請參閱 [建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### 刪除自訂OAuth2應用程式 {#delete-custom-oauth2-applications}

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth應用程式]**.
1. 按一下** **。
1. 將游標暫留在應用程式上，然後按一下 **[!UICONTROL 刪除]** ![](assets/delete.png) 當它出現在最右邊時。

## 在OAuth2應用程式中管理使用者端密碼

* [檢視使用者端密碼詳細資訊](#view-client-secret-details)
* [新增或編輯使用者端密碼的附註](#add-or-edit-notes-for-client-secret)
* [刪除使用者端密碼](#delete-client-secret)

### 檢視使用者端密碼詳細資訊 {#view-client-secret-details}

>[!IMPORTANT]
>
>您無法檢視使用者端密碼本身。 如果您遺失使用者端密碼，您必須刪除密碼並建立新的密碼。
>
>* 若要刪除使用者端密碼，請參閱 [刪除使用者端密碼](#delete-client-secret) 本文章內容。
>* 若要建立新的使用者端密碼，請參閱 [建立Oauth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) 在 [建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. 按一下 *[!UICONTROL *主要功能表]**圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth應用程式]**.
1. 將游標暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 圖示時（位於最右側）。
1. 在「使用者端密碼」區域中檢視詳細資訊：

   * 建立日期
   * 上次使用日期
   * 附註

     若要將附註新增至使用者端密碼，請參閱 [新增或編輯使用者端密碼的附註](#add-or-edit-notes-for-client-secret).

### 新增或編輯使用者端密碼的附註 {#add-or-edit-notes-for-client-secret}

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 將游標暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 圖示時（位於最右側）。
1. 找到您要新增或編輯備註的使用者端密碼。
1. 按一下包含使用者端密碼詳細資訊的方塊。

   您現在可以新增註記文字，或編輯現有的註記文字。

   >[!NOTE]
   >
   >附註文字最多可包含64個字元。

1. 按一下開箱即用或按 **[!UICONTROL 輸入]** 以儲存註記文字。

### 刪除使用者端密碼 {#delete-client-secret}

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 將游標暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 圖示時（位於最右側）。
1. 找到您要刪除的使用者端密碼。
1. 按一下 **[!UICONTROL 刪除]** 圖示 ![](assets/delete.png) 在使用者端密碼旁。
