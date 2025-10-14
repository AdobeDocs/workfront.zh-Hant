---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 整合 [!DNL Workfront Proof] 與 [!DNL Basecamp]
description: 如果您使用 [!DNL Basecamp] 進行專案管理，可以使用 [!DNL Workfront Proof]提供專案團隊更豐富的檢閱和核准工具。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# 將[!DNL Workfront Proof]與[!DNL Basecamp]整合

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您使用[!DNL Basecamp]進行專案管理，則可以使用[!DNL Workfront Proof]提供專案團隊更豐富的檢閱和核准工具。

## 瞭解[!DNL Basecamp]與[!DNL Workfront]的整合

與[!DNL Basecamp]整合可讓使用者在[!DNL Basecamp]內檢視、檢閱及核准校訂。 使用者可以將校訂提交至您的[!DNL Workfront Proof]帳戶，並將它們連結至您的[!DNL Basecamp]專案。 您的檢閱者可以使用內嵌在Basecamp訊息中的迷你校訂，透過[!DNL Basecamp]進行評論和決策。

與[!DNL Workfront Proof]整合時，[!DNL Basecamp]有下列校訂功能：

* 使用者可以在[!DNL Basecamp Classic]內檢閱和核准校樣。
* 使用者隨時可以使用檢閱工具。
* 專案稽核團隊在[!DNL Basecamp]中收到一封包含迷你校訂的郵件，以供稽核和核准。
* 使用者可以切換到整頁校訂以供檢閱和核准。
* 使用者可以在迷你和完整大小的校樣中新增評論和標籤。

  >[!NOTE]
  >
  >評論回覆後即無法編輯或刪除。

* 稽核者可回應其他稽核者所做的和標示。
* 當有新版本的校訂可用時，會提醒使用者。
* 不是[!DNL Workfront Proof]使用者的使用者可以在[!DNL Basecamp]中處理校訂。

[!DNL Workfront Proof]與[!DNL Basecamp]的整合必須在兩個層級上設定：

* 在[帳戶設定：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中設定[!DNL Basecamp]如此可讓您整個組織的Basecamp整合。 如需詳細資訊，請參閱[啟用Basecamp與 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof)的整合。

* 在[個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)中設定[!DNL Basecamp]：這可讓校訂建立者和擁有者連線到他們的個人Basecamp帳戶並授權[!DNL Workfront Proof]存取權。 如需詳細資訊，請參閱[設定個人設定](#configuring-personal-settings)。

您可以整合[!DNL Workfront]與[!DNL Basecamp]或[!DNL Basecamp Classic]。 每個版本的[!DNL Basecamp]使用不同的API，因此需要不同的設定程式。

如需設定[!DNL Basecamp Classic]的相關資訊，請參閱[整合 [!DNL Workfront Proof] 與 [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## 正在啟用[!DNL Basecamp]與[!DNL Workfront Proof]的整合

作為 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔或 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的校訂許可權設定檔，您可以在[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中設定整個帳戶的[!DNL Basecamp]整合。

1. 在[!UICONTROL Basecamp]中，收集下列資訊：

   * [!DNL Basecamp]帳戶的URL
   * 在[!UICONTROL 我的資訊]區段中找到URL

1. 登出[!DNL Basecamp]。
1. 按一下右上角附近的&#x200B;**[!UICONTROL 帳戶設定]**。
1. 按一下「**[!UICONTROL 整合]**」標籤。
1. 在&#x200B;**[!UICONTROL [!DNL Basecamp]]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL [!DNL Basecamp]整合]**&#x200B;右側的&#x200B;**[!UICONTROL 啟用]**。

1. 在&#x200B;**[!UICONTROL [!DNL Basecamp]版本]**&#x200B;旁邊，確認&#x200B;**[!UICONTROL Classic版本]**&#x200B;是您正在整合的版本。

1. （視條件而定）如果沒有顯示[!DNL Basecamp] URL，請按一下&#x200B;**[!UICONTROL 編輯]**，輸入您[!DNL Basecamp]帳戶的URL (不包括「http://」)，然後按一下&#x200B;**[!UICONTROL 儲存]**。

1. 在視窗的右上角，按一下&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。

1. 按一下「**[!UICONTROL 整合]**」標籤。
1. 在&#x200B;**[!DNL Basecamp]**&#x200B;下方&#x200B;**[!UICONTROL Basecamp整合]**&#x200B;的右側，按一下&#x200B;**[!UICONTROL 啟用]**。

1. 在出現的選項中，**[!UICONTROL [!DNL Basecamp]API Token]**&#x200B;的右側，按一下&#x200B;**[!UICONTROL 編輯]**。

1. 在出現的方塊中，輸入[!DNL Basecamp]中「[!UICONTROL 我的資訊]」區段中找到的URL，然後按一下&#x200B;**[!UICONTROL 儲存]**。\
   一旦您將[!DNL Workfront Proof]與[!DNL Basecamp]整合，您的使用者就可以設定其個人設定。 如需設定個人設定的詳細資訊，請參閱[設定個人設定](#configuring-personal-settings)

1. 如果您無法啟用[!DNL Basecamp]整合，您的[!DNL Workfront Proof]帳戶ID可能與您在[!DNL Basecamp]中使用的帳戶ID不同。
1. 一旦您將[!DNL Workfront Proof]與[!DNL Basecamp]整合，您的使用者就可以設定其個人設定。 如需設定個人設定的詳細資訊，請參閱[設定個人設定](#configuring-personal-settings)。

## 設定個人設定

在您為組織設定[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)後，建立/提交校訂的每位作者都應該設定其[個人設定。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. 移至&#x200B;**[!UICONTROL 個人**&#x200B;**設定]**。

1. 開啟&#x200B;**[!UICONTROL 整合]**&#x200B;標籤(1)。
1. 若要啟用[!DNL Basecamp]整合，請按一下&#x200B;**[!UICONTROL 啟用]** (2)。
1. 按一下&#x200B;**[!UICONTROL 連線到您的[!DNL Basecamp]帳戶]** (3)。\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. 登入您的[!DNL Basecamp]帳戶(1)。\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. 按一下&#x200B;**[!UICONTROL 是，我將允許存取]**&#x200B;以授權[!DNL Workfront Proof]存取您的帳戶(2)。\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. （選擇性）當您的個人整合作用中(3)時，您可以輕鬆地在[!DNL Basecamp]帳戶之間切換。

   1. 按一下&#x200B;**[!UICONTROL 切換[!DNL Basecamp]帳戶]** (4)。\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      [!UICONTROL Switch Basecamp帳戶]會帶您前往[!UICONTROL 個人設定]頁面，您可以在其中選擇要與[!DNL Workfront Proof]帳戶整合的[!DNL Basecamp]帳戶。

   1. 在選擇[!DNL Basecamp]帳戶之前，請按一下&#x200B;**[!UICONTROL 與[!DNL Basecamp]]** (5)重新整合\

      這會重新整理[!UICONTROL 個人設定]頁面，並顯示您[!DNL Basecamp]帳戶的最新清單。

   1. 按一下&#x200B;**[!UICONTROL 與此帳戶整合]**，以將其與[!DNL Workfront Proof]連線。\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      您現在可以將校樣新增到[!DNL Basecamp]個專案。
