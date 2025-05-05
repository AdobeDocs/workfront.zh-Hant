---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 常見問題集 — 建立和共用校樣和檔案
description: 校訂是靜態、音訊或視訊檔案，可在校訂檢視器中檢視。 新增到校訂的檢閱者擁有一組可用於對校訂進行評論和決策的工具。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 1%

---

# 常見問題集 — 建立和共用校樣和檔案

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

## 什麼是證明？

### 解答

校訂是靜態、音訊或視訊檔案，可在校訂檢視器中檢視。 新增到校訂的檢閱者擁有一組可用於對校訂進行評論和決策的工具。

## 支援哪些檔案型別？

### 解答

校樣可從靜態、音訊和視訊檔案建立。 您無法上傳大於4GB的檔案。 [!DNL Workfront]支援超過150個檔案型別（如需完整清單，請參閱[支援的校訂檔案型別和大小限制總覽](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)）。

## 校樣和檔案有何不同？

### 解答

當您上傳檔案至[!DNL Workfront Proof]時，系統會將檔案儲存在您的[!DNL Workfront Proof]帳戶中。 當您共用時，[!DNL Workfront Proof]會以電子郵件傳送一個連結，讓收件者可以按一下該連結來下載檔案。 您可以共用任何需要的檔案型別。

當您從已上傳至[!DNL Workfront Proof]的檔案建立校訂時，可讓檔案在校訂檢視器中供檢視。 稽核者會收到一封電子郵件，其中包含校訂的連結。 當他們開啟校訂時，他們會看到校訂影像，並可以在其中新增評論和做出決定。 您可以從支援的檔案型別清單中使用檔案來建立校樣。 您也可以使用網站和其他網頁內容的URL來建立校樣。

如需支援的檔案型別完整清單，請參閱[支援的校訂檔案型別和大小限制概觀](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)。

## 如何建立校訂？

### 解答

您可以從靜態檔案、音訊檔案、視訊檔案和URL建立校樣（請參閱）。

若要在帳戶中建立校訂，您必須是具有正確許可權設定檔的使用者（請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[!UICONTROL 校訂許可權設定檔]）。

如果同時上傳多個檔案，您會建立多個校樣，並使用一封電子郵件將其傳送給相同的稽核者群組。 如果您的組織有[!UICONTROL Enterprise]或[!UICONTROL Unlimited]帳戶，您可以將檔案合併為單一校訂（請參閱[建立多頁校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)）。

## 什麼是校訂角色和電子郵件警示？

### 解答

校訂角色定義檢閱者在校訂上需要採取的動作。 建立校訂時，您可以使用不同的角色選項供檢閱者使用，取決於您是否希望他們能夠發表評論、做出決定等。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

電子郵件警報會更新校訂進度的稽核者（它們與新校訂和延遲校訂通知不同）。 您可以根據稽核者在校樣上的角色，為不同的稽核者選取不同的選項。 如需詳細資訊，請參閱[使用[!UICONTROL 自動化工作流程]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)建立進階校訂。

## 我可以從多個檔案建立校訂嗎？

### 解答

將多個檔案合併為單一校訂是[!UICONTROL Enterprise]和[!UICONTROL Unlimited]版本計畫上可用的功能。 此選項僅適用於靜態檔案，不適用於視訊檔案。 如需詳細資訊，請參閱[建立多頁校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

## 我可以從URL建立校訂嗎？

### 解答

可以，您可以從網站和其他網路內容建立校樣。 當您新增URL以建立校訂時，您可以指定想要靜態校訂還是互動式校訂：

* 在互動式校訂中，檢閱者可以像平常一樣導覽及互動網站或其他網路內容，例如具有串流視訊或音訊的廣告、廣告中的[!DNL Flash]元素、HTML動畫及互動橫幅。 如需詳細資訊，請參閱[在ZIP檔案中建立互動式內容的校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md)。
* 針對靜態校樣，[!DNL Workfront]會取得您指定之頁面和子頁面的一組熒幕擷取畫面。 超連結在校訂中是即時的，因此您可以測試它們是否導向到正確的目的地。 如需詳細資訊，請參閱[為網站或其他網頁內容建立靜態校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md)。

如果您以空格分隔多個URL，可以一次新增多個URL。 請注意，組合僅適用於[!UICONTROL Enterprise]與[!UICONTROL Unlimited]版本計畫。

## 沒有登入許可權的使用者可以在我的帳戶中建立校訂嗎？

### 解答

您需要登入認證，才能直接在[!DNL Workfront Proof]帳戶中建立證明。

## 共用校訂是什麼意思？

### 解答

共用校訂可讓檢閱者存取校訂，以便他們可以新增評論和標示，並做出相關決策。 訪客檢閱者從收到的電子郵件通知存取校樣。 擁有自己[!DNL Workfront Proof]帳戶的檢閱者可以存取[!UICONTROL 儀表板]上的校樣。

## 如何共用校訂？

### 解答

建立校訂時，您可以在[!UICONTROL 新校訂]頁面的[!UICONTROL 工作流程]區段中新增檢閱者。 當校訂準備就緒時，[!DNL Workfront Proof]會傳送電子郵件給檢閱者，其中包含校訂的連結。

如果您有足夠的校訂許可權，可以使用校訂檢視器、您的[!UICONTROL 儀表板]或任何清單檢視將檢閱者新增到現有的校訂中(請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] 中共用校訂 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的頁面。

新增檢閱者是共用校樣的最常見方式。 如果您想探索其他可用選項，請參閱：

* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)中共用校訂連結
* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)中共用公用URL
* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)中訂閱校訂
* [在 [!DNL Workfront Proof]中建立Mini校訂](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## 您必須是使用者才能檢閱校訂嗎？

### 解答

否。訪客檢閱者（沒有[!DNL Workfront Proof]登入認證的人員）可以從他們收到的校訂電子郵件通知存取校訂。 您可以視需要與更多來賓共用校樣。

可以將共用校樣限製為具有[!DNL Workfront Proof]登入認證的人員。 這會在您的校樣中新增另一個安全性層。 為了增強安全性，擁有[!UICONTROL Enterprise]和[!UICONTROL Unlimited]計畫的組織的系統管理員可以針對組織中建立的所有校訂設定此需求。

如需需要登入的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md)中的證明安全性。

如果您的組織要求檢閱者以電子方式簽署校訂（需要登入[!DNL Workfront Proof]），則使用者只能與註冊使用者共用校訂。 這適用於[!UICONTROL Enterprise]和[!UICONTROL Unlimited]版本計畫。 如需詳細資訊，請參閱[瞭解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)中的電子簽章。

## 我可以設定檢閱者的截止日期嗎？

### 解答

當您建立校訂時，可以設定新校訂或新校訂版本的截止日期。 您在[!UICONTROL 新校訂]頁面的[!UICONTROL 工作流程]區段中執行此動作。 如果您使用[!UICONTROL 自動化工作流程]，您可以為檢閱的每個階段設定不同的截止日期。

您也可以使用[!UICONTROL 校訂詳細資料]頁面，設定或更新現有校訂的截止日期。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校訂詳細資訊。

## 如何建立新版本的校訂？

### 解答

檢閱者經常要求變更其對校訂的評論，並且想要檢視新版本的校訂。 您可以建立新版本的校訂。 [!DNL Workfront Proof]會記住先前版本的校訂設定。 如果您需要為校樣新增或移除稽核者等動作，您仍可編輯這些設定。

您必須將每個版本與需要檢視該版本的特定稽核者共用。 例如，如果您只與檢閱者共用版本3，則該人員無法看到版本1和2。 您帳戶中的主管和管理員會監督帳戶中的所有專案，以便他們可以檢視和編輯校訂的所有版本。

如需詳細資訊，請參閱。

## 我可以使用[!DNL Workfront Proof]共用檔案嗎？

### 解答

是。如果您想要與其他人共用某專案，但您不需要他們以校訂方式檢視它（或如果它是[!DNL Workfront Proof]不支援的檔案型別），您可以將它作為檔案上傳到您的[!DNL Workfront Proof]帳戶。 和校樣一樣，您可以在共用檔案時，將檔案整理到資料夾、標籤檔案及新增自訂訊息至通知電子郵件。 如需詳細資訊，請參閱[將檔案與網頁內容上傳至 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)。

當您的收件者收到與您共用檔案的電子郵件通知時，他們可以按一下通知中的連結以下載檔案。

[!DNL Workfront Proof]使用者可將檔案儲存在帳戶中後，轉換為校樣。

<!--Is there a limit-->
