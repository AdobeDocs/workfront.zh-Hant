---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: 了解 [!DNL Workfront Proof]
description: 電子簽名可讓您增強校樣的安全性，並符合ISO等行業標準。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 了解 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

電子簽名可讓您增強校樣的安全性，並符合ISO等行業標準。

在帳戶層級，此設定可設為強制或非強制。 如果預設為強制，則會在您帳戶中建立的所有校樣上啟用，且無法在校樣層級停用。 如果此設定預設為非強制性，您將能在校樣層級啟用/停用。

如需詳細資訊，請參閱。

當在校樣上啟用電子簽名設定時，電子簽名框將提示對校樣做出決定的任何審核者提供其電子郵件和密碼。

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## 電子簽名 [!UICONTROL 校樣詳細資料] 頁面

若審核者透過選取 [!UICONTROL 校樣詳細資料] 第(1)頁 [!UICONTROL 電子簽名] 彈出式方塊會出現，要求他們輸入其詳細資訊(2)並確認其決定(3)。

快顯視窗會顯示預設訊息集（如果有），且審核者必須輸入其電子郵件和密碼。

此 [!UICONTROL 電子簽名] 彈出式視窗會顯示在校對檢視器中，也會顯示在 [!UICONTROL 校樣詳細資料] 頁面，以便審核者決定從該層級進行決策。

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

若 [!UICONTROL 單一登入] 選項，則電子郵件和密碼詳細資訊不會顯示在 [!UICONTROL 電子簽名] 做決定時彈出。

而是在按一下 [!UICONTROL 確認] (4)此彈出式視窗上的按鈕會將審核者重新導向至 [!UICONTROL 單一登入] 頁面。

輸入SSO憑證後，審核者會自動重新導向回 [!UICONTROL 校樣詳細資料] 頁面(或返回 [!UICONTROL 校樣檢視器] 如果從那裡做出決定)。

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 如果以電子方式簽署決定， **[!UICONTROL 簽名表徵圖]** (5)會顯示在 [!UICONTROL 工作流程] 區段 [!UICONTROL 校樣詳細資料] 頁面。 如果不由審核者更改決定，而是由對校樣具有編輯權的另一人更改，則不會要求該人以電子方式簽署決定，且該決定(6)旁將沒有簽名表徵圖。

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)如需單一登入的詳細資訊，請參閱 [Workfront校樣中的單一登入](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

如需「校樣」詳細資訊頁面的相關資訊，請參閱 [在中管理校樣詳細資料 [!DNL Workfront] 校樣](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
