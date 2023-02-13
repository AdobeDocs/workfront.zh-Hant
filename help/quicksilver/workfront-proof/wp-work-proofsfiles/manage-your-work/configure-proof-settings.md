---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中配置校樣設定 [!DNL Workfront Proof]
description: 您可以透過下列任何方式設定要建立或編輯的校樣 — 編輯我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 1%

---

# 在中配置校樣設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

您可以透過下列任何方式來設定要建立或編輯的校樣：

>[!NOTE]
>
>您可以為您建立的所有新校樣配置這些設定。 如需詳細資訊，請參閱。

## 在做出最後決定時鎖定證明

您可以設定在最終核准者做出決策時鎖定的校樣狀態。 如果您想要確定審核者無法返回校樣並新增其他意見或變更其決定，這個功能會很實用。

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 校樣設定]**，選取 **[!UICONTROL 做出所有必要決策時鎖定校樣]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 做出所有決定時鎖定證明]**.

如需決策的相關資訊，請參閱 [在校對檢視器中決定校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## 需要所有檢閱校樣的使用者登入

關於 [!DNL Workfront Proof] 任何人都可以查證，你不需要擁有自己的證據 [!DNL Workfront Proof] 來做。 收件者會收到包含個人URL的電子郵件，該URL會將他們直接帶至校樣頁面，而無須登入 [!DNL Workfront Proof].

不過，如果您的審核和批准流程需要更高級別的安全性，則可以使用要求登錄校樣。 這隻表示 [!DNL Workfront Proof] 可將使用者新增至校樣。 他們必須輸入電子郵件和密碼才能訪問。

>[!NOTE]
>
>* *為了讓某人登入校樣（當需要登入時），必須已將其新增至校樣。*
>* *如果啟用「需要登入」，則無法啟用「訂閱」。*


若要要求所有檢閱校樣的使用者登入：

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 校樣設定]**，選取 **[!UICONTROL 需要登入]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 需要登入]**.

## 只需要一個證明決定

當您只需要群組、部門或公司中的一個人員來決定校樣時，此設定就十分實用。

即使您將核准者或審核者和核准者的角色指派給多個人員，一旦一個人對校樣做出決策，校樣的狀態就會更新（根據所做決定）。 如需校樣狀態的詳細資訊，請參閱 [在中檢視校樣的進度和狀態 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 工作流程]**，選取 **[!UICONTROL 此階段只需要一個決策]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 只需一個決定]**.

如需決策的相關資訊，請參閱 [在校對檢視器中決定校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## 要求以電子方式簽署決定

任何審核者決定提供其電子郵件和密碼的校樣，您都可以要求其電子簽名。 當審核者做出決策提示時，似乎會要求他們輸入電子郵件和密碼並確認其決策。 如需詳細資訊，請參閱 [了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 校樣設定]**，選取 **[!UICONTROL 要求以電子方式簽署決定]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 要求以電子方式簽署決定]**.

如需決策的相關資訊，請參閱 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## 不允許用戶下載原始檔案

您可以讓校樣的審核者不下載建立校樣的原始檔案。

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 校樣設定]**，取消選取 **[!UICONTROL 下載原始檔案]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 下載原始檔案]**.

## 允許其他使用者訂閱校樣

訂閱是可與校樣URL和Mini校樣搭配使用的進階設定。

依預設，尚未明確新增至校樣，且使用校樣URL或Mini校樣來存取校樣的人，只能以「唯讀」模式檢視校樣。 已經是校樣審核者的人員可以使用其電子郵件地址登入。 如需詳細資訊，請參閱 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

啟用校樣的訂閱，可讓尚未明確新增至校樣的使用者訂閱校樣（即將自己新增至校樣）。 然後，系統會為使用者指派您在訂閱設定中為其選取的角色和電子郵件警報。

如果已對校樣啟用訂閱，則下列欄位將會生效：

* **[!UICONTROL 需要訂閱者驗證]**  — 訂閱者必須按一下電子郵件中的連結才能存取校樣\
   選取此選項表示訂閱者無法立即存取校樣，但會在電子郵件中取得校樣的連結。 訂閱者驗證的目的，是確保使用者輸入了其有權存取的正確電子郵件地址。

* **[!UICONTROL 新訂閱者的預設角色]**  — 這是將分配給所有訂閱校樣的審核者的預設校樣角色。
* **[!UICONTROL 新訂閱者的預設電子郵件警報]**  — 這是預設電子郵件警報，將分配給所有訂閱校樣的審核者。

另請參閱 [在中訂閱校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

若要允許其他使用者訂閱校樣：

1. 建立新校樣，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校樣的「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 若是新的證明，請在 **[!UICONTROL 校樣設定]**，取消選取 **[!UICONTROL 透過公開URL或內嵌程式碼訂閱校樣]**.\
   或\
   若為現有證明，請在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 訂閱]**.
