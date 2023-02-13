---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 整合 [!DNL Workfront Proof] with [!DNL Basecamp]
description: 如果您使用 [!DNL Basecamp] 對於項目管理，您可以使用 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# 整合 [!DNL Workfront Proof] with [!DNL Basecamp]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您使用 [!DNL Basecamp] 對於項目管理，您可以使用 [!DNL Workfront Proof].

## 了解 [!DNL Basecamp] 與整合 [!DNL Workfront]

與整合 [!DNL Basecamp] 可讓使用者在 [!DNL Basecamp]. 使用者可以將校樣提交至您的 [!DNL Workfront Proof] 將其與您的 [!DNL Basecamp] 專案。 審核者可以透過 [!DNL Basecamp]，使用內嵌於Basecamp訊息中的mini校樣。

與整合時 [!DNL Workfront Proof], [!DNL Basecamp] 具有下列校對功能：

* 使用者可以在 [!DNL Basecamp Classic].
* 使用者可隨時使用審核工具。
* 專案審核團隊會在 [!DNL Basecamp] 提供微型的審核和批准證明。
* 使用者可切換至完整頁面的校樣，以進行審核和核准。
* 使用者可為小型和完整校樣新增註解和標籤。

   >[!NOTE]
   >
   >評論一經回覆，便無法編輯或刪除。

* 審核者可回應其他審核者所做的和標籤。
* 有新版本的校樣可用時，系統會提醒使用者。
* 非 [!DNL Workfront Proof] 使用者可以在 [!DNL Basecamp].

整合 [!DNL Workfront Proof] with [!DNL Basecamp] 必須設定在兩個層級：

* 設定 [!DNL Basecamp] in [帳戶設定：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 這可讓您整個組織的Basecamp整合。 如需詳細資訊，請參閱 [啟用Basecamp整合，與 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* 設定 [!DNL Basecamp] in [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):這可讓證明建立者和擁有者連線至其個人Basecamp帳戶並授權 [!DNL Workfront Proof] 存取權。 如需詳細資訊，請參閱 [配置個人設定](#configuring-personal-settings).

您可以整合 [!DNL Workfront] 為 [!DNL Basecamp] 或 [!DNL Basecamp Classic]. 每個版本 [!DNL Basecamp] 使用不同的API，因此需要不同的設定程式。

有關配置的資訊 [!DNL Basecamp Classic]，請參閱 [整合 [!DNL Workfront Proof] with [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## 啟用 [!DNL Basecamp] 與整合 [!DNL Workfront Proof]

As a [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 或 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)，您可以設定 [!DNL Basecamp] 整合 [帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. 在 [!UICONTROL 巴塞坎普]，收集下列資訊：

   * 您 [!DNL Basecamp] 帳戶
   * 在「[!UICONTROL 我的資訊]&quot;部分

1. 登出 [!DNL Basecamp].
1. 按一下 **[!UICONTROL 帳戶設定]** 在右上角。
1. 按一下 **[!UICONTROL 整合]** 標籤。
1. 在 **[!UICONTROL [!DNL Basecamp]]** 部分，在 **[!UICONTROL [!DNL Basecamp]整合]**，按一下 **[!UICONTROL 啟用]**.

1. 旁邊 **[!UICONTROL [!DNL Basecamp]版本]**，驗證 **[!UICONTROL 傳統版本]** 是您要整合的版本。

1. （條件性）若否 [!DNL Basecamp] URL顯示，按一下 **[!UICONTROL 編輯]**，輸入 [!DNL Basecamp] 帳戶(不含「http://」)，然後按一下 **[!UICONTROL 儲存]**.

1. 在視窗的右上角，按一下 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

1. 按一下 **[!UICONTROL 整合]** 標籤。
1. 在 **[!DNL Basecamp]**，位於 **[!UICONTROL Basecamp整合]**，按一下 **[!UICONTROL 啟用]**.

1. 在顯示的選項中，位於 **[!UICONTROL [!DNL Basecamp]API Token]**，按一下 **[!UICONTROL 編輯]**.

1. 在顯示的方塊中，輸入在「[!UICONTROL 我的資訊]「 」部分 [!DNL Basecamp]，然後按一下 **[!UICONTROL 儲存]**.\
   整合後 [!DNL Workfront Proof] with [!DNL Basecamp]，您的使用者可以設定其個人設定。 有關設定個人設定的資訊，請參閱 [配置個人設定](#configuring-personal-settings)

1. 如果您無法啟用 [!DNL Basecamp] 整合，您的 [!DNL Workfront Proof] 帳戶ID可能與您在 [!DNL Basecamp].
1. 整合後 [!DNL Workfront Proof] with [!DNL Basecamp]，您的使用者可以設定其個人設定。 有關設定個人設定的資訊，請參閱 [配置個人設定](#configuring-personal-settings).

## 配置個人設定

在您設定 [帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 針對您的組織，建立/提交證明的每個作者都應設定  [個人設定。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. 前往 **[!UICONTROL 個人** &#x200B; **設定]**.

1. 開啟 **[!UICONTROL 整合]** 標籤(1)。
1. 若要啟用 [!DNL Basecamp] 整合，按一下 **[!UICONTROL 啟用]** (2)。
1. 按一下 **[!UICONTROL 連線至您的 [!DNL Basecamp] 帳戶]** (3)。\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. 登入 [!DNL Basecamp] 帳戶(1)。\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. 按一下 **[!UICONTROL 是的，我會允許]** 授權 [!DNL Workfront Proof] 對您的帳戶的訪問(2)。\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. （選用）當您的個人整合處於作用中狀態時(3)，您可輕鬆在 [!DNL Basecamp] 帳戶。

   1. 按一下 **[!UICONTROL 交換機 [!DNL Basecamp] 帳戶]** (4)。\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      此 [!UICONTROL 交換機Basecamp帳戶] 帶你去 [!UICONTROL 個人設定] 頁面，您可在其中選取 [!DNL Basecamp] 您想要與 [!DNL Workfront Proof] 帳戶。

   1. 按一下 **[!UICONTROL 重新整合，與[!DNL Basecamp]]** (5)在選擇 [!DNL Basecamp] 帳戶\

      這會重新整理 [!UICONTROL 個人設定] 頁面，並顯示最新清單 [!DNL Basecamp] 帳戶。

   1. 按一下 **[!UICONTROL 與此帳戶整合]** 連接 [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      您現在可以將校樣新增至 [!DNL Basecamp] 專案。
