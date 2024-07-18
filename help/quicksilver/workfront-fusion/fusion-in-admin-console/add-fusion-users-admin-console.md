---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 透過Adobe Admin Console將使用者新增到Adobe Workfront Fusion
description: 您可以將使用者新增到Adobe Admin Console並將他們指派到Adobe Workfront Fusion，或將Adobe Admin Console中的現有使用者指派到Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# 透過[!DNL Adobe Admin Console]將使用者新增至[!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>此頁面上說明的程式僅適用於已上線到[!DNL Adobe Admin Console]的組織。
>
>如果您的組織尚未加入[!DNL Adobe Admin Console]，請參閱[在 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md)中將使用者新增至組織。
>
>如需根據貴組織是否已加入[!DNL Adobe Admin Console]而不同的程式清單，請參閱[平台式管理差異([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md)。

您可以將使用者新增至[!DNL Adobe Admin Console]並將他們指派至[!DNL Adobe Workfront Fusion]，或將[!DNL Adobe Admin Console]中的現有使用者指派至[!DNL Workfront Fusion]。

如需[!DNL Adobe Admin Console]中說明[!DNL Workfront Fusion]的影片，包括如何新增使用者，請參閱Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}上的[[!DNL Fusion] 。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 管理員許可權</td> 
   <td>您必須是組織[!DNL Adobe]個產品的[！UICONTROL產品設定管理員]。</td> 
  </tr>
  </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

&#42;&#42;如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 先決條件

在針對[!DNL Workfront]使用[!DNL Admin Console]之前，您應該會收到一封邀請您加入主控台的電子郵件。

1. 如果您是[!DNL Adobe]的新手，並且已收到一封電子郵件，告知您現在擁有管理貴組織的[!DNL Adobe]軟體與服務的管理許可權，請按一下電子郵件中的按鈕以建立[!DNL Adobe]帳戶並開啟[!DNL Admin Console]。

   或

   如果您已有Adobe帳戶，請移至[[!DNL Adobe Admin Console] 頁面](https://adminconsole.adobe.com/)。


## 新增使用者至[!DNL Adobe Admin Console]和[!DNL Workfront Fusion]

1. 從[[!DNL Adobe Admin Console] 頁面](https://adminconsole.adobe.com/)，選取頂端導覽列中的&#x200B;**[!UICONTROL Products]**&#x200B;索引標籤，然後選取&#x200B;**[!DNL Workfront Fusion]**&#x200B;產品拼貼。

   Admin Console](assets/fusion-product-admin-console.png)中的![Fusion

1. 在顯示的清單中，選取您要新增使用者的組織。

   Admin Console](assets/fusion-instances-admin-console.png)中的![Fusion執行個體

1. 在顯示的清單中，選取&#x200B;**[!UICONTROL 產品設定檔]**&#x200B;索引標籤後，按一下[!DNL Workfront Fusion] [!UICONTROL 產品設定檔]連結的名稱。

   ![Workfront Fusion產品設定檔](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 請勿變更[!UICONTROL 產品設定檔]本身。

1. 在清單上方選取&#x200B;**[!UICONTROL 使用者]**&#x200B;索引標籤後，按一下&#x200B;**[!UICONTROL 新增使用者]**。

1. 在&#x200B;**[!UICONTROL 將使用者新增至此產品設定檔]**&#x200B;方塊中，輸入您要新增使用者的電子郵件地址或名稱，然後在出現的清單中選取使用者。

1. 按一下「**[!UICONTROL 儲存]**」。

   已在[!DNL Workfront Fusion]中建立使用者。

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. （選擇性）繼續在 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)中[變更使用者的存取層級

## 在Workfront Fusion中變更使用者的存取層級

### 將使用者角色變更為管理員

必須在[!DNL Adobe Admin Console]中完成為使用者指定管理員角色。

1. 在您新增使用者的[!DNL Workfront Fusion] [!UICONTROL 產品設定檔]頁面上，選取「**[!UICONTROL 管理員]**」標籤。

1. 按一下&#x200B;**[!UICONTROL 新增管理員]**。

1. 在&#x200B;**[!UICONTROL 新增產品設定檔管理員]**&#x200B;方塊中，輸入您要新增的使用者的電子郵件地址或名稱，然後在出現的清單中選取使用者。

1. 按一下「**[!UICONTROL 儲存]**」。

   此使用者現在是[!DNL Workfront Fusion]的管理員。

### 將使用者的角色變更為[!UICONTROL 成員]、[!UICONTROL 會計]或[!UICONTROL 應用程式開發人員]。

[!UICONTROL 成員]、[!UICONTROL 會計]和[!UICONTROL 應用程式開發人員]角色在[!DNL Workfront Fusion]內處理。

如需指示，請參閱文章[管理 [!DNL Adobe Workfront Fusion] 組織中的使用者](../organizations/manage-fusion-users.md)中的[檢視或編輯使用者角色](../organizations/manage-fusion-users.md#view-or-edit-user-roles)

## 將[!DNL Adobe Admin Console]中的現有使用者指派給[!DNL Workfront Fusion]

1. 開始編輯使用者，如[!DNL Adobe Admin Console]檔案中文章[個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)的「編輯使用者詳細資訊」一節中所述。

1. 將&#x200B;**[!DNL Adobe Workfront Fusion]**&#x200B;新增至指派給使用者的產品。
