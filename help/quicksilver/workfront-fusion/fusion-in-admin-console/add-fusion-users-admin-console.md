---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 透過Adobe Admin Console將使用者新增到Adobe Workfront Fusion
description: 您可以將使用者新增至Adobe Admin Console並將其指派至Adobe Workfront Fusion，或將Adobe Admin Console中的現有使用者指派至Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 1%

---

# 新增使用者至 [!DNL Adobe Workfront Fusion] 透過 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於已上線至的組織。 [!DNL Adobe Admin Console].
>
>如果您的組織尚未上線至 [!DNL Adobe Admin Console]，請參閱 [在中新增使用者至組織 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>針對因貴組織是否已上線至而不同的程式清單， [!DNL Adobe Admin Console]，請參閱 [平台式管理差異([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

您可以將使用者新增至 [!DNL Adobe Admin Console] 並將它們指派給 [!DNL Adobe Workfront Fusion]，或在中指派現有使用者 [!DNL Adobe Admin Console] 至 [!DNL Workfront Fusion].

適用於描述以下專案的影片： [!DNL Workfront Fusion] 在 [!DNL Adobe Admin Console]，包括如何新增使用者，請參閱 [[!DNL Fusion] 在Adobe IMS上](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 管理員許可權</td> 
   <td>您必須是以下專案的[！UICONTROL產品設定管理員]： [!DNL Adobe] 適用於貴組織的產品。</td> 
  </tr>
  </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 必要條件

使用之前 [!DNL Admin Console] 的 [!DNL Workfront]，您應會收到一封邀請您加入主控台的電子郵件。

1. 如果您是初次使用 [!DNL Adobe] 而且您已經收到一封電子郵件，告訴您現在擁有管理許可權 [!DNL Adobe] 軟體與服務，按一下電子郵件中的按鈕以建立 [!DNL Adobe] 帳戶並開啟 [!DNL Admin Console].

   或

   如果您已有Adobe帳戶，請前往 [[!DNL Adobe Admin Console] 頁面](https://adminconsole.adobe.com/).


## 將新使用者新增至 [!DNL Adobe Admin Console] 和 [!DNL Workfront Fusion]

1. 從 [[!DNL Adobe Admin Console] 頁面](https://adminconsole.adobe.com/)，選取 **[!UICONTROL 產品]** 標籤進行連結，然後選取 **[!DNL Workfront Fusion]** 產品拼貼。

   ![Admin Console中的Fusion](assets/fusion-product-admin-console.png)

1. 在顯示的清單中，選取您要新增使用者的組織。

   ![Admin Console中的Fusion執行個體](assets/fusion-instances-admin-console.png)

1. 在顯示的清單中，使用 **[!UICONTROL 產品設定檔]** 標籤選取時，按一下 [!DNL Workfront Fusion] [!UICONTROL 產品設定檔] 連結。

   ![Workfront Fusion產品設定檔](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 請勿變更 [!UICONTROL 產品設定檔] 本身。

1. 使用 **[!UICONTROL 使用者]** 標籤選取於清單上方，按一下 **[!UICONTROL 新增使用者]**.

1. 在 **[!UICONTROL 將使用者新增至此產品設定檔]** 方塊中，輸入您要新增的使用者的電子郵件地址或名稱，然後在出現的清單中選取使用者。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   使用者建立於 [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. （選用）繼續前往 [在中變更使用者的存取層級 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## 在Workfront Fusion中變更使用者的存取層級

### 將使用者角色變更為管理員

授予使用者管理員角色必須在以下位置完成： [!DNL Adobe Admin Console].

1. 於 [!DNL Workfront Fusion] [!UICONTROL 產品設定檔] 在您新增使用者的頁面中，選取 **[!UICONTROL 管理員]** 標籤。

1. 按一下 **[!UICONTROL 新增管理員]**.

1. 在 **[!UICONTROL 新增產品設定檔管理員]** 方塊中，輸入您要新增的使用者的電子郵件地址或名稱，然後在出現的清單中選取使用者。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   此使用者現在是中的管理員 [!DNL Workfront Fusion].

### 將使用者角色變更為 [!UICONTROL 會員]， [!UICONTROL 會計]，或 [!UICONTROL 應用程式開發人員].

[!UICONTROL 會員]， [!UICONTROL 會計]、和 [!UICONTROL 應用程式開發人員] 角色在內處理 [!DNL Workfront Fusion].

如需指示，請參閱 [檢視或編輯使用者角色](../organizations/manage-fusion-users.md#view-or-edit-user-roles) 在文章中 [管理 [!DNL Adobe Workfront Fusion] 您組織中的使用者](../organizations/manage-fusion-users.md)

## 在中指派現有使用者 [!DNL Adobe Admin Console] 至 [!DNL Workfront Fusion]

1. 依照文章的「編輯使用者詳細資訊」一節中所述，開始編輯使用者 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 在 [!DNL Adobe Admin Console] 說明檔案。

1. 新增 **[!DNL Adobe Workfront Fusion]** 指派給使用者的產品。
