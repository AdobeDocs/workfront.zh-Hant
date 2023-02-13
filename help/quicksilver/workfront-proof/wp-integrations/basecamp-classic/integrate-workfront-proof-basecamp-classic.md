---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: 整合 [!DNL Workfront Proof] 與Basecamp Classic
description: 如果您使用 [!DNL Basecamp] 對於項目管理，您可以使用 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 整合 [!DNL Workfront Proof] with [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您使用 [!DNL Basecamp] 對於項目管理，您可以使用 [!DNL Workfront Proof].

## 了解 [!DNL Basecamp] 與整合 [!DNL Workfront]

與整合 [!DNL Basecamp] 可讓使用者在 [!DNL Basecamp]. 使用者可以將校樣提交至您的 [!DNL Workfront Proof] 將其與您的 [!DNL Basecamp] 專案。 您的審核者可以 [在校對檢視器中決定校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp]，使用內嵌於Basecamp訊息中的mini校樣。

與整合時 [!DNL Workfront Proof], [!DNL Basecamp] 可讓使用者對校樣執行下列動作：

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

* 設定 [!DNL Basecamp] in [帳戶設定：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 這可讓您整個組織的Basecamp整合。
* 如需詳細資訊，請參閱 [啟用 [!DNL Basecamp] 與整合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* 設定 [!DNL Basecamp] in [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):這可讓證明建立者和擁有者與其個人連結 [!DNL Basecamp] 帳戶和授權 [!DNL Workfront Proof] 存取權。 如需詳細資訊，請參閱 [配置個人設定](#configuring-personal-settings).

您可以整合 [!DNL Workfront] 為 [!DNL Basecamp] 或 [!DNL Basecamp Classic]. 每個版本 [!DNL Basecamp] 使用不同的API，因此需要不同的設定程式。

有關配置的資訊 [!DNL Basecamp Classic]，請參閱 [啟用 [!DNL Basecamp] 與整合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 這篇文章。

有關配置的資訊 [!DNL Basecamp]，請參閱 [整合 [!DNL Workfront Proof] with [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## 啟用 [!DNL Basecamp] 與整合 [!DNL Workfront Proof]

As a [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 或 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)，您可以在您的 [帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. 前往 [帳戶設定。](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. 開啟 **[!UICONTROL 整合]** 標籤(1)。
1. 若要啟用Basecamp整合，請按一下 **[!UICONTROL 啟用]** (2)。
1. 確認 [!DNL Basecamp Classic] 是您要與(3)整合的版本。
1. （條件性）若否 [!DNL Basecamp] URL顯示(4)，按一下 **[!UICONTROL 編輯]** 並輸入 [!DNL Basecamp] 帳戶(不含http://)。
1. 按一下 **[!UICONTROL 儲存]** (5)。\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. （選用）檢查 [!DNL Basecamp] 登入您的 [!DNL Basecamp Classic] 賬號(6)。

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   整合後 [!DNL Workfront Proof] with [!DNL Basecamp]，您的使用者可以設定其個人設定。 有關設定個人設定的資訊，請參閱 [配置個人設定](#configuring-personal-settings).

   如果您無法啟用 [!DNL Basecamp] 整合，您的 [!DNL Workfront Proof] 帳戶ID可能與您在 [!DNL Basecamp].

## 配置個人設定

在您設定 [帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 針對您的組織，建立/提交證明的每個作者都應設定  [個人設定。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>如果您有 [!DNL Basecamp] 工作階段在單一瀏覽器視窗中開啟，而您的 [!DNL Workfront Proof] 工作階段會在另一個視窗中開啟。

* [擷取 [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token)
* [新增您的 [!DNL Basecamp] API代號至您的個人設定](#adding-your-basecamp-api-token-to-your-personal-settings)

### 擷取 [!DNL Basecamp] API Token

若要在 [!DNL Workfront Proof]，使用者需要其個別驗證Token才能 [!DNL Basecamp] API。

若要擷取 [!DNL Basecamp] API Token:

1. 登入 [!DNL Basecamp] 帳戶。
1. 按一下 **[!UICONTROL 我的資訊]** （一）螢幕右上角。\
   此 [!UICONTROL 我的資訊] 頁面。\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. 在 [!UICONTROL 驗證Token] ，按一下 **[!UICONTROL 顯示代號]** (2)顯示個人驗證代號。
1. 選取 **[!UICONTROL 摘要讀取器的代號]** 或 **[!UICONTROL Basecamp API]** (3)，然後將代號複製到剪貼簿。

1. 貼上您的 [!DNL Basecamp] API代號放入 [!UICONTROL 摘要讀取器的代號] 或 [!UICONTROL Basecamp API] 框。\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### 新增您的 [!DNL Basecamp] API代號至您的個人設定

若要貼上 [!DNL Basecamp] API代號放入您的 [!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. 前往 [[!UICONTROL 整合]  — 使用者設定](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) 在 [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)。\
   管理員必須先啟用 [!DNL Basecamp Classic] 整合，以便啟用個人設定。 如需設定整合的詳細資訊，請參閱 [啟用 [!DNL Basecamp] 與整合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 這篇文章。

1. 在 [!DNL Basecamp] API代號方塊(2)，貼上您剛從 [!DNL Basecamp] [!UICONTROL 我的資訊] 頁面到欄位(3)。\
   有關複製 [!DNL Basecamp] API代號，請參閱 [擷取 [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token) 這篇文章。

1. 按一下 **[!UICONTROL 儲存]** (4)。

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

您的 [!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) 現在已與 [!DNL Basecamp Classic] 帳戶。
