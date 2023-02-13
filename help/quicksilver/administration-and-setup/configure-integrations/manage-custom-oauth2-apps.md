---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: 檢視及管理自訂OAuth2應用程式
description: 身為Adobe Workfront管理員，您可以檢視及管理Workfront執行個體的OAuth2應用程式，如此可讓其他應用程式存取Workfront。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# 檢視及管理自訂OAuth2應用程式

作為 [!DNL Adobe Workfront] 管理員，您可以檢視並管理您執行個體的OAuth2應用程式 [!DNL Workfront]，允許其他應用程式存取 [!UICONTROL Workfront].

>[!NOTE]
>
>在OAuth2的內容中，「Oauth2應用程式」是指應用程式和伺服器之間的這種存取連結，例如 [!DNL Workfront]. 如需詳細資訊，請參閱 [為建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* 如需建立自訂OAuth2應用程式的相關資訊，請參閱 [為建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* 如需使用者認證（授權程式碼流程）設定和使用OAuth2應用程式的相關指示，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 有關使用PKCE配置和使用OAuth2應用程式的說明，請參見 [使用PKCE流配置和使用貴組織的自定義OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> 您必須是 [!DNL Workfront] 管理員。 </p>
    <p>如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

您必須建立 [!UICONTROL OAuth2] 組織的應用程式，然後您才能檢視或管理這些應用程式。

如需詳細資訊，請參閱 [為建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 管理自訂OAuth2應用程式

* [檢視及編輯自訂OAuth2應用程式](#view-and-edit-custom-oauth2-applications)
* [刪除自訂OAuth2應用程式](#delete-custom-oauth2-applications)

### 檢視及編輯自訂OAuth2應用程式 {#view-and-edit-custom-oauth2-applications}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** ![](assets/edit-icon.png) 在最右邊。
1. （可選）編輯應用程式的任何詳細資訊。

   如需OAuth2和JWT應用程式的相關欄位，請參閱 [為建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### 刪除自訂OAuth2應用程式 {#delete-custom-oauth2-applications}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **  **.
1. 暫留在應用程式上，然後按一下 **[!UICONTROL 刪除]** ![](assets/delete.png) 在最右邊。

## 在OAuth2應用程式中管理用戶端密碼

* [查看客戶端密碼詳細資訊](#view-client-secret-details)
* [新增或編輯用戶端密碼的附註](#add-or-edit-notes-for-client-secret)
* [刪除用戶端密碼](#delete-client-secret)

### 查看客戶端密碼詳細資訊 {#view-client-secret-details}

>[!IMPORTANT]
>
>您無法檢視用戶端密碼本身。 如果您遺失用戶端密碼，則必須將其刪除並建立新密碼。
>
>* 若要刪除用戶端密碼，請參閱 [刪除用戶端密碼](#delete-client-secret) 這篇文章。
>* 若要建立新的用戶端密碼，請參閱 [建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [為建立OAuth2應用程式 [!DNL Workfront] 整合](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. 按一下 *[!UICONTROL *主菜單]**表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 表徵圖。
1. 在「用戶端密碼」區域中檢視詳細資訊：

   * 建立日期
   * 上次使用日期
   * 附註

      若要將附註新增至用戶端密碼，請參閱 [新增或編輯用戶端密碼的附註](#add-or-edit-notes-for-client-secret).

### 新增或編輯用戶端密碼的附註 {#add-or-edit-notes-for-client-secret}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 表徵圖。
1. 找出您要新增或編輯附註的用戶端密碼。
1. 按一下包含用戶端密碼詳細資訊的方塊。

   您現在可以新增附註文字，或編輯現有的附註文字。

   >[!NOTE]
   >
   >注釋文本最多64個字元。

1. 按一下「退出」或按 **[!UICONTROL 輸入]** 來保存注釋文本。

### 刪除用戶端密碼 {#delete-client-secret}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 暫留在應用程式上，然後按一下 **[!UICONTROL 編輯]** 表徵圖。
1. 找出您要刪除的用戶端密碼。
1. 按一下 **[!UICONTROL 刪除]** 圖示 ![](assets/delete.png) 位於「用戶端密碼」旁。
