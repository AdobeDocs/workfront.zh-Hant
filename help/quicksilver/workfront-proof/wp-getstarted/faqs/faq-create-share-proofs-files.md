---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 常見問題集 — 建立和共用校樣和檔案
description: 校樣是靜態、音訊或視訊檔案，可在校樣檢視器中檢閱。 加入校樣的審核者有一套工具可供他們對校樣進行評論和決策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# 常見問題集 — 建立和共用校樣和檔案

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

## 什麼是證據？

### 回答

校樣是靜態、音訊或視訊檔案，可在校樣檢視器中檢閱。 加入校樣的審核者有一套工具可供他們對校樣進行評論和決策。

## 支援哪些檔案類型？

### 回答

校樣可從靜態、音訊和視訊檔案建立。 您無法上傳超過4GB的檔案。 [!DNL Workfront] 支援超過150種檔案類型(請參閱 [支援的校對檔案類型和大小限制概觀](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) 以取得完整清單)。

## 校樣和檔案有何不同？

### 回答

將檔案上傳至 [!DNL Workfront Proof]，系統會將檔案儲存在 [!DNL Workfront Proof] 帳戶。 當你共用它時， [!DNL Workfront Proof] 您的收件者會透過電子郵件傳送連結，供他們點按以下載檔案。 您可以共用任何想要的檔案類型。

從已上傳的檔案建立校樣時 [!DNL Workfront Proof]，則可讓檔案在校對檢視器中供檢閱。 審核者會收到包含校樣連結的電子郵件。 當他們開啟校樣時，會看到校樣影像，並可以新增註解並據此做出決策。 您可以使用支援的檔案類型清單中的檔案來建立校樣。 您也可以使用網站URL和其他網頁內容來建立校樣。

如需支援檔案類型的完整清單，請參閱 [支援的校對檔案類型和大小限制概觀](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## 如何建立校樣？

### 回答

您可以從靜態檔案、音訊檔案、視訊檔案和URL建立校樣（請參閱）。

若要在帳戶中建立校樣，您必須是具有正確權限設定檔的使用者(請參閱 [[!UICONTROL 校樣權限設定檔] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))。

如果您同時上傳多個檔案，您會建立多個校樣，可透過一封電子郵件傳送給相同的審核者群組。 如果貴組織有 [!UICONTROL 企業] 或 [!UICONTROL 無限制] 帳戶，您可以將檔案合併成單一校樣(請參閱 [建立多頁校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md))。

## 什麼是校樣角色和電子郵件警報？

### 回答

校樣角色定義審核者對校樣所需採取的動作。 在建立校樣時，您可以針對審核者使用不同的角色選項，具體取決於您希望審核者是否能夠進行評論、做出決策等。 如需詳細資訊，請參閱 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

電子郵件警報會更新審核者校樣的進度（它們與新校樣和延遲校樣通知不同）。 您可以根據每個審閱者對校樣的角色，為不同的審閱者選擇不同的選項。 如需詳細資訊，請參閱 [使用建立進階校樣 [!UICONTROL 自動化工作流程]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 我可以從多個檔案建立校樣嗎？

### 回答

將多個檔案合併為單一校樣是 [!UICONTROL 企業] 和 [!UICONTROL 無限制] 版本計畫。 此選項僅適用於靜態檔案，而不適用於視訊檔案。 如需詳細資訊，請參閱  [建立多頁校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## 我可以從URL建立校樣嗎？

### 回答

可以，您可以從網站和其他網頁內容建立校樣。 新增URL以建立校樣時，您可以指定您要靜態校樣或互動式校樣：

* 在互動式校樣中，審核者可像平常一樣導覽及互動網站或其他網路內容，例如含有串流視訊或音訊的廣告， [!DNL Flash] 廣告中的元素、HTML動畫和互動式橫幅。 如需詳細資訊，請參閱 [建立ZIP檔案中互動式內容的校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* 對於靜態校樣， [!DNL Workfront] 會擷取您指定之頁面和子頁面的設定螢幕擷取畫面。 超連結在校樣中是即時的，因此您可以測試它們是否會導向正確的目的地。 如需詳細資訊，請參閱 [為網站或其他網路內容建立靜態校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

如果您以空格分隔多個URL，則可一次新增這些URL。 請注意，僅可在 [!UICONTROL 企業] 和 [!UICONTROL 無限制] 版本計畫。

## 沒有登入資訊的人可以在我的帳戶中建立證明嗎？

### 回答

您需要登入憑證，才能直接在 [!DNL Workfront Proof] 帳戶。

## 分享證明是什麼意思？

### 回答

分享校樣可讓審核者存取校樣，以便新增註解和標籤，並據此做出決策。 訪客審核者從收到的電子郵件通知中存取校樣。 具有自己的審核者 [!DNL Workfront Proof] 帳戶可以存取 [!UICONTROL 控制面板].

## 如何分享證明？

### 回答

建立校樣時，您可以在 [!UICONTROL 工作流程] 區段 [!UICONTROL 新校樣] 頁面。 證據準備好後， [!DNL Workfront Proof] 傳送電子郵件給包含校樣連結的審核者。

如果您對校樣有足夠的權限，則可以使用校樣檢視器，您的 [!UICONTROL 控制面板]，或任何清單檢視以將審核者新增至現有校樣(請參閱 [在中共用校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] 頁面 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

新增審核者是共用校樣的最常見方式。 如果您想要探索其他可用選項，請參閱：

* [在中共用校樣連結 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [共用公用URL於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [在中訂閱校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [在中建立Mini校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## 您必須是使用者才能檢閱證明嗎？

### 回答

否. 訪客審核者(沒有 [!DNL Workfront Proof] 登入認證)可從收到的校樣電子郵件通知中存取校樣。 您可以與任意數量的來賓共用證明。

您可以限制將分享證明給具有 [!DNL Workfront Proof] 登入憑證。 這會為校樣增加另一層安全性。 為了增強安全性，使用 [!UICONTROL 企業] 和 [!UICONTROL 無限制] 計畫可以為組織中建立的所有校樣配置此需求。

如需需要登入的詳細資訊，請參閱 [證明安全性 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

如果您的組織要求審核者以電子方式簽署校樣，則需要登入 [!DNL Workfront Proof]，則使用者只能與已註冊的使用者共用校樣。 可在 [!UICONTROL 企業] 和 [!UICONTROL 無限制] 版本計畫。 如需詳細資訊，請參閱 [了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## 我可以為審閱者設定最後期限嗎？

### 回答

建立校樣時，您可以設定新校樣或新校樣版本的截止日期。 您在 [!UICONTROL 工作流程] 區段 [!UICONTROL 新校樣] 頁面。 如果您使用 [!UICONTROL 自動化工作流程]，您可以為每個審核階段設定不同的截止時間。

您也可以使用 [!UICONTROL 校樣詳細資料] 頁面。 如需詳細資訊，請參閱 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## 如何建立新版本的校樣？

### 回答

審核者通常會要求對校樣的意見進行變更，並想查看新版校樣。 您可以建立校樣的新版本。 [!DNL Workfront Proof] 會記住上一個版本的校樣設定。 如果需要執行添加或刪除校樣審核者之類的操作，您仍可以編輯這些設定。

您必須與需要檢視的每個版本的特定審核者共用每個版本。 例如，如果您只與審核者共用第3版，該人員將看不到第1版和第2版。 您帳戶中的主管和管理員會監督帳戶中的所有專案，讓他們可以查看及編輯所有版本的校樣。

如需詳細資訊，請參閱。

## 我可以使用 [!DNL Workfront Proof]?

### 回答

是. 如果您想要與他人共用某個項目，但您不需要他們將其視為校樣（或是不支援的檔案類型） [!DNL Workfront Proof])，您可以將其以檔案形式上傳至 [!DNL Workfront Proof] 帳戶。 和校樣一樣，您可以將檔案組織成資料夾、標籤檔案，並在共用檔案時將自訂訊息新增至通知電子郵件。 如需詳細資訊，請參閱 [將檔案和網頁內容上傳至 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

收件者收到您所共用檔案的電子郵件通知時，可按一下通知中的連結下載檔案。

[!DNL Workfront Proof] 將檔案儲存在帳戶中後，使用者可將檔案轉換為校樣。

<!--Is there a limit-->
