---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: 將 [!DNL Workfront Proof] 與Basecamp Classic整合
description: 如果您使用 [!DNL Basecamp] 進行專案管理，可以使用 [!DNL Workfront Proof]提供專案團隊更豐富的檢閱和核准工具。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# 將[!DNL Workfront Proof]與[!DNL Basecamp Classic]整合

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您使用[!DNL Basecamp]進行專案管理，則可以使用[!DNL Workfront Proof]提供專案團隊更豐富的檢閱和核准工具。

## 瞭解[!DNL Basecamp]與[!DNL Workfront]的整合

與[!DNL Basecamp]整合可讓使用者在[!DNL Basecamp]內檢視、檢閱及核准校訂。 使用者可以將校訂提交至您的[!DNL Workfront Proof]帳戶，並將它們連結至您的[!DNL Basecamp]專案。 您的檢閱者可以使用Basecamp郵件中內嵌的迷你校訂，透過[!DNL Basecamp]在校訂檢視者](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)中決定校訂[。

與[!DNL Workfront Proof]整合時，[!DNL Basecamp]可讓使用者對校訂進行下列操作：

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

* 在[帳戶設定：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中設定[!DNL Basecamp]如此可讓您整個組織的Basecamp整合。
* 如需詳細資訊，請參閱[啟用 [!DNL Basecamp] 與 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof)的整合。
* 在[個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)中設定[!DNL Basecamp]：這可讓校訂建立者和擁有者連線到他們的個人[!DNL Basecamp]帳戶並授權[!DNL Workfront Proof]存取權。 如需詳細資訊，請參閱[設定個人設定](#configuring-personal-settings)。

您可以整合[!DNL Workfront]與[!DNL Basecamp]或[!DNL Basecamp Classic]。 每個版本的[!DNL Basecamp]使用不同的API，因此需要不同的設定程式。

如需有關設定[!DNL Basecamp Classic]的資訊，請參閱本文中的[啟用 [!DNL Basecamp] 與 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof)的整合。

如需設定[!DNL Basecamp]的詳細資訊，請參閱[整合 [!DNL Workfront Proof] 與 [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md)。

## 正在啟用[!DNL Basecamp]與[!DNL Workfront Proof]的整合

作為 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔或 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔，您可以在[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中為整個帳戶設定Basecamp整合。

1. 移至[帳戶設定。](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. 開啟&#x200B;**[!UICONTROL 整合]**&#x200B;標籤(1)。
1. 若要啟用Basecamp整合，請按一下&#x200B;**[!UICONTROL 啟用]** (2)。
1. 確認[!DNL Basecamp Classic]是您正在與(3)整合的版本。
1. （視條件而定）如果沒有顯示[!DNL Basecamp] URL (4)，請按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;並輸入您[!DNL Basecamp]帳戶的URL (不含http://)。
1. 按一下&#x200B;**[!UICONTROL 儲存]** (5)。\
   ![基本帳戶_設定_-_整合.png](assets/basecamp-account-settings---integration-350x192.png)

1. （選擇性）登入[!DNL Basecamp Classic]帳戶後，在瀏覽器中檢查您的[!DNL Basecamp] URL (6)。

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   一旦您將[!DNL Workfront Proof]與[!DNL Basecamp]整合，您的使用者就可以設定其個人設定。 如需設定個人設定的詳細資訊，請參閱[設定個人設定](#configuring-personal-settings)。

   如果您無法啟用[!DNL Basecamp]整合，您的[!DNL Workfront Proof]帳戶ID可能與您在[!DNL Basecamp]中使用的帳戶ID不同。

## 設定個人設定

在您為組織設定[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)後，建立/提交校訂的每位作者都應該設定其[個人設定。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>如果您在一個瀏覽器視窗中開啟您的[!DNL Basecamp]工作階段，而在另一個視窗中開啟您的[!DNL Workfront Proof]工作階段，完成這些步驟是最簡單的。

* [正在擷取您的 [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token)
* [正在將您的 [!DNL Basecamp] API Token新增至您的個人設定](#adding-your-basecamp-api-token-to-your-personal-settings)

### 正在擷取您的[!DNL Basecamp] API Token

若要在[!DNL Workfront Proof]中完成個別層級的整合，使用者需要[!DNL Basecamp] API的個別驗證權杖。

若要擷取您的[!DNL Basecamp] API Token：

1. 登入您的[!DNL Basecamp]帳戶。
1. 按一下熒幕右上角的&#x200B;**[!UICONTROL 我的資訊]** (1)。\
   顯示[!UICONTROL 我的資訊]頁面。\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. 在[!UICONTROL 驗證權杖]區段中，按一下&#x200B;**[!UICONTROL 顯示您的權杖]** (2)以顯示您的個人驗證權杖。
1. 選取摘要讀取程式的&#x200B;**[!UICONTROL Token]**&#x200B;或&#x200B;**[!UICONTROL Basecamp API]** (3)，然後將該Token複製到剪貼簿。

1. 將您的[!DNL Basecamp] API Token貼到摘要讀取程式的[!UICONTROL Token]或[!UICONTROL Basecamp API]方塊中。\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### 正在將您的[!DNL Basecamp] API Token新增至您的個人設定

若要將[!DNL Basecamp] API權杖貼入您的[!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)：

1. 移至[個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)中的[[!UICONTROL 整合] — 使用者設定](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md)。\
   系統管理員必須先啟用[!DNL Basecamp Classic]整合，您才能啟用個人設定。 如需設定整合的詳細資訊，請參閱本文中的[啟用 [!DNL Basecamp] 與 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof)的整合。

1. 在[!DNL Basecamp] API Token方塊(2)中，將您剛才從[!DNL Basecamp] [!UICONTROL 我的資訊]頁面複製的Token貼到欄位(3)。\
   如需有關複製[!DNL Basecamp] API Token的資訊，請參閱本文中的[擷取 [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token)。

1. 按一下&#x200B;**[!UICONTROL 儲存]** (4)。

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

您的[!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)現已與您的[!DNL Basecamp Classic]帳戶整合。
