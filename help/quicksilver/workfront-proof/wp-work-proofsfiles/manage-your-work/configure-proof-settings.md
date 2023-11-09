---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中設定校訂設定 [!DNL Workfront Proof]
description: 您可以設定在校樣中建立或編輯的校樣。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# 在中設定校訂設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文提及獨立版產品中的功能 [!DNL Workfront Proof]. 有關內部校訂的資訊 [!DNL Adobe Workfront]，請參閱 [校訂](../../../review-and-approve-work/proofing/proofing.md).

您可以透過下列任何方式設定您正在建立或編輯的校樣：

>[!NOTE]
>
>您可以為您建立的所有新校樣設定這些設定。 如需詳細資訊，請參閱。

## 進行最後決定時鎖定校訂

您可以設定校訂狀態，以在最終核准者做出決定時鎖定。 如果您想要確保檢閱者無法返回校樣並新增其他評論或變更其決定，這將很有用。

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 校訂設定]**，選取 **[!UICONTROL 完成所有必要的決定時鎖定校訂]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 完成所有決定時鎖定校訂]**.

如需決策的詳細資訊，請參閱 [在校訂檢視器中對校訂做出決定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## 所有檢閱校訂的使用者需要登入

最棒的一點是 [!DNL Workfront Proof] 任何人都可以檢閱證明，您不需要擁有自己的證明 [!DNL Workfront Proof] 以達成此目的。 收件者會收到一封電子郵件，其中包含個人URL，可直接帶他們前往校訂頁面，無需登入 [!DNL Workfront Proof].

不過，如果您的稽核和核准流程需要更高的安全性級別，您可以使用需要登入到校訂中。 這表示 [!DNL Workfront Proof] 可以將使用者新增到校訂中。 而且使用者必須先輸入電子郵件和密碼，才能存取。

>[!NOTE]
>
>* *為了讓某人登入校訂（已啟用需要登入功能），必須將他們新增至校訂中。*
>* *如果已啟用需要登入，則無法啟用訂閱。*

若要要求所有檢閱校訂的使用者登入：

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 校訂設定]**，選取 **[!UICONTROL 需要登入]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 需要登入]**.

## 只需一個決定即可證明

如果您只需要群組、部門或公司中的一個人來決定校訂，此設定很有用。

即使您將核准者或檢閱者和核准者的角色指派給多個人，一旦有一個人對校訂做出決定，校訂的狀態將更新（根據所做決定）。 如需有關校訂狀態的詳細資訊，請參閱 [在中檢視校訂的進度和狀態 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 工作流程]**，選取 **[!UICONTROL 此階段只需要一個決定]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 只需要一個決定]**.

如需決策的詳細資訊，請參閱 [在校訂檢視器中對校訂做出決定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## 需要以電子方式簽署決策

您可以要求任何對校樣做出決定的檢閱者的電子簽章，以提供其電子郵件和密碼。 當稽核者做出決定提示出現時，會要求他們輸入電子郵件和密碼並確認其決定。 如需詳細資訊，請參閱 [瞭解中的電子簽章 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 校訂設定]**，選取 **[!UICONTROL 需要以電子方式簽署決策]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 需要以電子方式簽署決策]**.

如需決策的詳細資訊，請參閱 [在中設定核准決定選項 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## 不允許使用者下載原始檔案

您可以讓校訂上的檢閱者下載建立校訂的原始檔案。

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 校訂設定]**，取消選取 **[!UICONTROL 下載原始檔案]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 下載原始檔案]**.

## 允許其他使用者訂閱證明

訂閱是進階設定，可與校訂URL和迷你校訂搭配使用。

根據預設，未特別新增到校訂並使用Proof URL或Mini Proof來存取的人只能以唯讀模式檢視校訂。 已經是校訂稽核者的使用者可以使用他們的電子郵件地址登入。 如需詳細資訊，請參閱 [管理校訂角色於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

對校訂啟用訂閱可讓未明確新增到校訂的人員訂閱校訂（也就是將自己新增到校訂中）。 接著，系統會為您指派在訂閱設定中為其選取的角色和電子郵件警示。

如果已在校訂上啟用訂閱，則下列欄位將變為使用中：

* **[!UICONTROL 需要訂閱者驗證]**  — 訂閱者必須按一下電子郵件中的連結才能存取校訂\
   選取此選項表示訂閱者不會立即存取校訂，但會透過電子郵件取得校訂連結。 訂閱者驗證的目的是確保該人員輸入了他們有權存取的正確電子郵件地址。

* **[!UICONTROL 新訂閱者的預設角色]**  — 這是將指派給訂閱校訂的所有檢閱者的預設校訂角色。
* **[!UICONTROL 新訂閱者的預設電子郵件警示]**  — 這是將指派給訂閱校訂的所有檢閱者的預設電子郵件警報。

另請參閱 [訂閱中的校訂 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

若要允許其他使用者訂閱校訂：

1. 建立新校訂，如所述 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   開啟現有校訂的校訂詳細資訊頁面，如所述 [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 如需新校樣，請前往 **[!UICONTROL 校訂設定]**，取消選取 **[!UICONTROL 透過公開URL或內嵌程式碼訂閱校訂]**.\
   或\
   針對現有校樣，在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 訂閱]**.
