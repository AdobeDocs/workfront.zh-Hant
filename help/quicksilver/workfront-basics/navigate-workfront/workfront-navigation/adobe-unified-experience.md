---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: ' [!DNL Workfront]的Adobe Unified Experience'
description: 透過Adobe CX Enterprise存取 [!DNL Workfront] 可讓您以順暢、統一的體驗管理所有Adobe應用程式。
author: Courtney
feature: Get Started with Workfront
exl-id: 458631a2-d77d-46d6-8d6b-7008237e5154
TQID: https://experienceleague.adobe.com/4fgMPIn0x6PWLmdi-iP9lt7skFKPiGMLOGGYYfCrhC8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 697
ht-degree: 3%

---

# [!DNL Workfront]的[!DNL Adobe Unified Experience]

<!--Audited: 10/2024-->

透過[!DNL Adobe CX Enterprise]存取[!DNL Workfront]可讓您以順暢、統一的體驗管理所有[!DNL Adobe]應用程式。 單一身分管理可為您提供一個登入位置，不需要多個URL或登入ID。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 封裝</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權</strong></td> 
   <td> <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您組織的[!DNL Workfront]執行個體必須上線到[!DNL Adobe Business Platform]或[!DNL Adobe Admin Console]。

如果您對加入[!DNL Adobe Admin Console]有任何疑問，請參閱[[!DNL Adobe Unified Experience] 常見問答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md/)。

## Adobe Identity Management系統(IMS)

在改用Adobe Unified Experience的過程中，您的組織現在會使用Adobe的Identity Management系統來驗證使用者。 這表示您會透過Adobe登入Workfront，而非直接登入Workfront。 Adobe IMS也要求Workfront管理員在Adobe Admin Console中處理使用者管理，而不是在Workfront中。

如需有關在Adobe Unified Experience中登入Workfront的資訊，請參閱本文中的[登入Adobe CX Enterprise](#log-in-to-adobe-cx-enterprise)。

如需Adobe Admin Console中的使用者管理資訊，請參閱文章[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

## 登入 [!DNL Adobe CX Enterprise]

1. 開啟瀏覽器視窗並移至<https://experience.adobe.com>。
1. 在&#x200B;[!UICONTROL **登入**]&#x200B;畫面上，輸入您的電子郵件地址並按一下&#x200B;**[!UICONTROL 繼續]**。

   ![登入[!DNL Adobe CX Enterprise]](assets/aec-login-page.png)

>[!NOTE]
>
>如果您已開啟Workfront的頁面中的瀏覽器分頁工作階段到期，且另一個瀏覽器分頁中有作用中的Workfront工作階段，您可以重新載入過期的分頁以重新開啟Workfront頁面。

## 存取[!DNL Workfront]

登入[!DNL Adobe CX Enterprise]後，按一下頂端導覽區中的組織切換器，即可檢視您有權存取的所有[!DNL Workfront]組織和環境。 選取您要使用的[!DNL Workfront]組織或環境。 如果您的組織使用[!UICONTROL 預覽]和[!UICONTROL 沙箱]等環境。

![檢視[!DNL Workfront]組織和環境](assets/wf-org-instance-switcher-2026.png)

>[!NOTE]
>
>第一次登入[!DNL Adobe CX Enterprise]時，組織會預設為字母清單中的第一個組織。 下次登入時，組織會預設為您上次造訪的組織。

[!DNL Workfront]會出現在您有權存取的[!DNL Adobe CX Enterprise]產品清單中。 您可以在[!DNL CX Enterprise]首頁上的快速存取功能表中選擇[!DNL Workfront]，或使用產品切換器![產品切換器](assets/main-menu-icon.png)隨時變更應用程式。

![選取[!DNL Workfront]以存取應用程式](assets/cx-enterprise-home-2026.png)

## 導覽[!DNL Workfront]

使用[!DNL Workfront]導覽列左側的[!UICONTROL 主功能表]圖示![主功能表圖示](assets/main-menu-icon-left-nav.png)，導覽至您有權存取的任何頁面。 [!UICONTROL 主要功能表]中可用的選項相依於：

* **配置範本設定**：若要瞭解[!DNL Workfront]系統管理員如何從配置範本修改[!UICONTROL 主功能表]，請參閱[使用配置範本自訂[!UICONTROL 主功能表]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)。
* **授權型別**：若要瞭解不同授權型別的預設設定，請參閱[瞭解[!UICONTROL 輕量級]授權使用者的導覽](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/reviewer-global-navigation-bar.md)或[瞭解[!UICONTROL 工作]授權使用者的導覽](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/worker-global-navigation-bar.md)。

![主功能表](assets/main-menu-options-left-nav.png)

## 存取您的設定檔和偏好設定

您可以按一下頂端導覽區域中的Adobe帳戶選單（您的設定檔圖片），存取您的設定檔和偏好設定選項。

![設定檔功能表](assets/unified-shell-profile-menu-2026.png)

此功能表可讓您：

* 選擇[!DNL Adobe CX Enterprise]的&#x200B;**[!UICONTROL 深色佈景主題]**&#x200B;格式。
* 設定[!DNL Adobe CX Enterprise]的&#x200B;**[!UICONTROL 偏好設定]**，包括主要和次要語言偏好設定。

  >[!NOTE]
  >
  >您的日期設定是以您的主要語言設定為基礎。 例如，選取&#x200B;**英文（美國）**&#x200B;會以MM/DD/YYYY格式顯示日期，而選取&#x200B;**英文（英國）**&#x200B;則會以DD/MM/YYYY格式顯示日期。

* 存取您的&#x200B;**[!UICONTROL [!DNL Workfront]設定檔]**。 進入設定檔後，按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-icon.png)，然後選取&#x200B;**[!UICONTROL 編輯]**。 如需設定檔的詳細資訊，請參閱[設定我的設定](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。
* **[!UICONTROL 登出]** / [!DNL Adobe CX Enterprise]。

## 管理您的密碼

>[!NOTE]
>
>變更您的密碼會變更您所有[!DNL Adobe CX Enterprise]應用程式的密碼。

您的密碼未在[!DNL Workfront]中管理。

如果您的組織使用單獨的應用程式來管理密碼，您將透過該提供者變更您的密碼。

如果您的密碼是由[!DNL Adobe]管理，您可以在Adobe帳戶中變更密碼。

[請參閱本文以瞭解如何變更您的Adobe密碼。](https://helpx.adobe.com/account/individual/sign-in-and-security/security-and-recovery/reset-adobe-password.html){target="_blank"}

如需變更密碼的詳細資訊，請連絡管理員。


