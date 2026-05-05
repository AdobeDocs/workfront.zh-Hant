---
product-area: documents
navigation-topic: approvals
title: 統一檢閱和核准總覽
description: 深入瞭解由Workfront和Frame.io支援的統一檢閱和核准。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: abca776dd79dcb1b5ef7c59745719a0faee5c845
workflow-type: tm+mt
source-wordcount: '3977'
ht-degree: 0%

---


# 統一檢閱和核准總覽

統一的稽核和核准將Adobe Workfront和Adobe Frame.io整合為單一、深度連結的體驗，消除行銷管理、創意稽核和內容傳送之間的差距。
專案專員在Workfront中管理工作，而創意人員、行銷人員和利害關係人則在專業級Frame.io檢視器中稽核及核准資產，所有這一切都無需在中斷連線的工具之間移動檔案。

![圖表顯示整合式稽核與核准工作流程，專案專員在Workfront中管理工作，而稽核者與核准者在Frame.io檢視器中提供意見與決策。](assets/Unified-Review-Approvals-Image.png)

<!--
## Integration requirements

* The Workfront instance must be enabled on the Adobe Unified Experience.

-->

## 內建於Adobe企業儲存空間

統一的檢閱和核准是以Adobe企業儲存空間為基礎所打造，這是一種雲端式儲存空間解決方案，可作為Adobe企業產品（包括Workfront和Frame.io）資產的中央存放庫。<!--, and Creative Cloud.-->

Adobe企業儲存的主要優點包括：

* 適用於創意與工作管理資產的統一儲存層
* 使用Adobe Identity Management系統(IMS)集中管理許可權，以進行安全存取控制
* Workfront和Frame.io <!--, and Creative Cloud apps -->的端對端資產可見性
* 可擴充的儲存與配額管理，因應企業需求

如需詳細資訊，請參閱[Adobe企業儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 統一的稽核和核准

透過統一的稽核和核准，您可以：

* 直接從Workfront建立和管理稽核與核准
* 即時追蹤稽核和核准的狀態
* 將意見反應與核准集中於一處
* 確保所有利害關係人都能存取最新版本的資產
* 利用AI稽核者來自動進行品牌法規審查
* 及更多內容

如需詳細資訊，請參閱[整合檔案核准：文章索引](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)。


### 使用Frame.io檢視器

使用Frame.io檢視器檢閱及核准資產。 Frame.io檢視器提供

* 標籤和註解工具
* 版本記錄與比較
* 視訊評論的時間戳記評論
* 行動存取以進行行動稽核和核准

如需詳細資訊，請參閱[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

#### 影片檢閱限制

視訊校訂要求的年度上限設定為組織總付費Workfront使用者授權的10% — 標準和輕度。 此上限適用於組織層級。

當使用量達到上限的80%和100%時，Workfront管理員會收到通知。

此限制不適用於Frame.io Enterprise客戶。

#### Frame.io檢視器中支援的檔案型別

Frame.io檢視器支援所有常見的視訊、影像、音訊、PDF和MS® Office型別。 如需支援檔案的詳細清單，請參閱Frame.io[&#128279;](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)上的支援的檔案型別。

#### Frame.io檢視器的存取與授權

Frame.io檢視器是所有Workfront檢閱和核准工作流程的預設檢視器。 所有擁有付費授權的Workfront使用者都會自動包含此功能。 使用Frame.io檢視器進行檢閱和核准不需要額外的Frame.io授權。

如果您的組織想要利用此整合提供的其他Frame.io功能（例如直接將資產上傳到Frame.io中的專案），您可以購買Frame.io Enterprise授權。 請聯絡您的Adobe客戶代表以排程示範，並探索完整Frame.io解決方案的優點。

此整合無法使用Workfront校訂功能。

## Workfront強大的專案管理

專案專員可善用Workfront強大的專案管理功能來規劃、追蹤及管理工作。

如需有關在Workfront中管理專案的詳細資訊，請參閱[專案：文章索引](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。

### 強制的結構與命名慣例

由於統一檢閱和核准是使用Adobe企業儲存空間建立的，因此在管理專案和檔案時，應注意一些強制執行的結構和命名慣例。

* 如果程式和專案屬於相同的投資組合，則不能有相同的名稱。
* 如果檔案屬於相同專案，則不能使用相同名稱。
* 物件名稱不能包含下列任何特殊字元： \ / ： * ？ &quot; | &lt; >
* 計畫、投資組合、專案、範本、任務、問題和檔案資料夾不能有以句點或空格結尾的名稱。
* 物件名稱的上限為255個字元。

考慮到這些限制，Workfront會視需要自動重新命名物件或檔案，以避免衝突。

### 共用與許可權

在整合過程中，使用者許可權需在Workfront中加以控制並向下流至Frame.io。 這表示您無法邀請使用者加入Frame.io中的專案，也無法修改Frame.io中的使用者許可權。 這些動作需要透過Workfront中的專案共用模式完成。

下表顯示Workfront許可權對應至Frame.io許可權的方式：

<table>
<tr>
<th>Workfront使用者許可權</th>
<th>Frame.io使用者許可權</th>
</tr>
<tr>
<td>管理</td>
<td>編輯與共用</td>
</tr>
<tr>
<td>參與</td>
<td>編輯與共用</td>
</tr>
<tr>
<td>檢視</td>
<td>僅註解</td>
</tr>
</table>



### Workfront的檔案管理

上傳至Workfront的檔案會儲存在Adobe企業儲存空間中，並可在Workfront和Frame.io中存取。 當您將檔案上傳到Workfront中的任務或問題時，系統會在Adobe企業儲存空間中建立一個系統產生的檔案夾，該檔案夾會繼承任務或問題的許可權。 上傳至該任務或問題的所有檔案都會儲存在該資料夾中，並繼承其許可權。 如需Workfront中檔案的詳細資訊，請參閱[新的檔案區域總覽](/help/quicksilver/documents/managing-documents/documents-area.md)和[Adobe企業儲存模型的物件許可權和存取層級總覽](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)。

### 檔案體驗限制

不包含下列檔案功能：

<!--* External document providers-->
* 在Workfront中存取校訂
* Workfront中的檔案檢視器
* 我的最愛檔案
* 要求檔案

## 開始使用統一檢閱和核准

若要開始進行統一檢閱和核准，請參閱[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

## 常見問題

### 統一檢閱和核准快速入門

+++ 展開以檢視開始使用統一檢閱和核准的常見問題。

**什麼是整合式檢閱和核准？**

整合式稽核和核准是Adobe Workfront與Adobe Frame.io之間的原生整合，可在單一連線系統中將工作管理和創意稽核整合在一起。 專案專員在Workfront中規劃和追蹤工作，而稽核者和核准者則使用專業級的Frame.io檢視器來提供意見回饋、標籤資產並做出核准決定，而不需在個別工具或手動移動檔案之間切換。

稽核和核准是每個內容操作的中心。 這是創意工作、利害關係人的意見和業務決策融合的地方。 當這個過程分散在中斷連線的工具（電子郵件對話、聊天訊息、熒幕擷圖示示）中時，結果會複雜化：上市時間變慢、失去意見反應、版本混淆，以及耗費在管理檔案而非建立內容上的時間。

統一檢閱和核准可透過以一個現代系統取代分散式檢閱工具的拼湊方式來解決這個問題，這個現代系統是一個真實資料來源，存在於已發生工作的地方。

**使用此整合需要哪些條件？**

若要使用統一的稽核和核准，以下條件必須符合：

* Workfront和Frame.io必須部署至相同的Adobe Identity Management System (IMS)組織。

* 使用者只能屬於IMS組織內的一個Workfront執行個體。

* 必須在Adobe Unified Experience和Adobe企業儲存空間上啟用Workfront執行個體。

* Workfront客戶必須使用V2 Workfront SKU。 如果您的組織尚未使用V2 Workfront SKU，則需要與Adobe進行合約活動，才能將V2 Workfront SKU新增至您的合約。 請聯絡您的Adobe客戶代表。

**我是否需要Frame.io授權才能使用此整合？**

否。 所有擁有付費授權的Workfront使用者都能自動隨附Frame.io檢視器，不需額外付費。 您不需要個別的Frame.io授權，就能透過Workfront檢閱及核准資產。

如果您的組織想要存取其他Frame.io功能 — 例如直接將資產上傳到Frame.io中的專案 — 您可以購買Frame.io Enterprise授權。 請聯絡您的Adobe客戶代表以瞭解更多資訊。

**這是否會取代Workfront Proof？**

是。 啟用統一檢閱和核准後，Frame.io檢視器會成為Workfront中的主要檢閱表面，取代Workfront Proof。

現有客戶可繼續存取Workfront校訂功能，此功能適用於整合啟用前建立的任何專案。

**如何取得整合式檢閱和核准的存取權？**

**我需要做什麼才能取得存取權？**

若要存取統一的檢閱和核准，您的組織必須使用V2 Workfront SKU。 尚未使用V2 Workfront SKU的任何組織都必須與Adobe進行合約活動，才能新增V2 Workfront SKU。 若要開始執行:

* 請聯絡您的Adobe客戶代表，確認您目前的Workfront合約是否採用V2 Workfront SKU。

* 如果您的組織不是V2 Workfront SKU，您的客戶代表將引導您完成新增所需的合約事件。

* 一旦您的合約包含V2 Workfront SKU，Adobe Professional Services就會為您的組織設定整合。

   * 如果您不確定您的Adobe客戶代表是誰，可以透過Adobe支援入口網站聯絡或造訪Experience League以取得聯絡選項。

+++

### 統一檢閱和核准的運作方式

+++ 展開以檢視統一檢閱和核准如何運作的常見問題。

**檢閱和核准工作流程如何運作？**

工作流程會遵循下列一般步驟：

1. 專案協調員會在Workfront中建立專案，並上傳或連結資產。

1. 當資產準備好進行檢閱時，協調員會建立核准工作流程 — 單一使用核准或套用可重複使用的核准範本。

1. 指派的檢閱者和核准者會透過電子郵件收到通知，並可直接在Frame.io檢視器中開啟資產。

1. 檢閱者可以新增註釋和標示。 核准者必須做出正式決定。

1. 協調員會即時追蹤Workfront的狀態。

**檢閱者和核准者之間有何差異？**

檢閱者可以在Frame.io檢視器中新增註解及標示資產。 完成後，他們將評論標籤為完成。 但是，核准工作流程無需其動作即可推進。

核准者必須執行下列其中一項決定，才能推進核准工作流程：

* **核准**：資產已準備就緒，可依原樣使用。

* **需要工作**：資產需要變更，必須重新提交為新版本才能重新核准。

**我可以建立哪些型別的核准工作流程？**

* **單次使用核准**：您可以直接在專案、任務或問題中的檔案上建立單次使用核准。 您可以視需要指派稽核者和核准者、設定截止日期以及設定多個階段。 自動化電子郵件提醒會在截止日期前72小時、前24小時傳送。

* **核准範本**：您可以在Workfront設定中建立可重複使用的範本。 範本定義稽核者、核准者和相對完成時間範圍。 您可以視需要建立多個階段。 將範本套用至資產後，系統會自動計算截止日期。

**外部使用者如何參與稽核？**

外部Workfront使用者指派給稽核或核準時，會透過電子郵件收到通知。 系統會提示他們建立Frame.io登入以存取檢視器並參與稽核程式。

**如何追蹤稽核和核准進度？**

專案專員可以透過多種方式監視所有執行中的核准：

* Workfront首頁區域中的我的核准Widget可提供擱置和逾期核准的即時摘要。

* 檔案核准量度Widget會顯示平均核准時間和決定劃分。

* 可以在畫布儀表板中建置自訂報告儀表板，以便更深入地瞭解審查和核准活動。

+++


### 檢閱和核准資產和影片

+++ 展開以檢視檢閱和核准資產和影片的常見問題。

**視訊評論是否有任何限制？**

是。 視訊校訂要求的年度上限設定為貴組織總付費Workfront使用者授權（標準和輕度）的10%。 此上限適用於組織層級。

當使用量達到上限的80%和100%時，Workfront管理員會收到應用程式內通知。

此限制不適用於Frame.io Enterprise客戶。 如果貴組織定期檢視大量視訊內容，請聯絡您的Adobe客戶代表，瞭解有關Frame.io Enterprise授權的相關資訊。

**同一位使用者可以出現在核准工作流程的多個階段嗎？**

是。 使用者可指派至相同核准工作流程中的多個階段。

**我可以新增階段來建立多階段核准工作流程嗎？**

是。 支援多階段核准工作流程，可讓您在每個階段透過不同參與者的循序稽核和核准輪次來路由資產。

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**核准範本是否可以包含群組或團隊，或僅包含個別使用者？**

目前，核准範本支援個別使用者和團隊。

**當核准者有需要檢閱的內容時，他們是否會收到電子郵件通知？**

是。 核准者和稽核者會在被指派給稽核或核準時收到電子郵件通知。 自動提醒電子郵件也會在截止日期前72小時、前24小時及截止日期本身傳送。

自訂電子郵件通知訊息的功能目前無法使用，但已列入產品藍圖中。

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**我可以保留其他參與者的私人稽核階段嗎？**

目前沒有私人階段功能。 為了不讓其他參與者檢視該稽核，建議的方法是為該稽核群組建立單獨的資產副本。 評論目前不會依單一資產中的參與者群組分段。

請注意，有權檢視該資產的任何人一律可以看到版本記錄，包括過去和目前的版本。

**評論可以標示為已解決嗎？**

是。 註解可在Frame.io檢視器中標示為已解決。

**Frame.io檢視器中有哪些標籤和註釋工具可用？**

Frame.io檢視器包含完整的視覺標籤工具，包括手繪繪圖和標準形狀，例如圓形、箭頭和正方形。 對於視訊資產，註解會以精確到影格的精確度加上時間戳記，因此回饋一律會與剪輯中的精確時間連結，而不只是一般時間戳記。

**在Frame.io檢視器中所做的評論是否會出現在Workfront專案中？**

註解與註解會保留在Frame.io檢視器中，以便保留完整的上下文，包括時間戳記與視覺標籤。 這在未來版本中可能會演變。

**是否可以將註解新增至資產的下載版本（例如PDF）？**

目前不支援此功能，但這是常見要求的功能，正在考慮在未來版本中。

**我可以一起檢閱多個資產嗎？**

即將推出增強型大量檢閱選項。 同時，不同檔案型別的資產（例如影片和Word檔案）可一起包含在分組資產評論中。

**是僅限視訊的統一檢閱和核准，還是支援其他檔案型別？**

整合式檢閱和核准是專為所有資產型別所設計，不只是視訊。 Frame.io檢視器已大幅更新，除了視訊外，還支援影像、檔案、PDF和其他常見的檔案格式。

如需支援的檔案型別完整清單，請參閱Experience League上的Frame.io支援的檔案型別檔案。

**我是否可以在外部與無法存取Workfront的利害關係人共用資產？**

是。 Assets可在外部共用。 系統會透過電子郵件通知外部使用者，並提示您建立Frame.io登入以存取檢視器並參與檢閱。

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### 儲存與檔案管理

+++ 展開以檢視儲存和檔案管理的常見問題。

**什麼是Adobe企業儲存空間？它與此整合有何關係？**

Adobe企業儲存是連線Workfront、Frame.io和Adobe Creative Cloud的常用儲存層。 Assets在一個位置上線，且可供所有工具存取，無需手動傳輸檔案。 創意內容可以在適當位置運作，且稽核者一律會看到最新版本。

Adobe企業儲存的主要優點包括：

* 適用於Workfront和Frame.io的所有進行中資產的單一儲存層

* 透過Adobe Identity Management System (IMS)管理的集中式存取控制

* 端對端資產可視性 — 不會發生版本漂移，不會遺失中繼資料

* 可擴充的企業級儲存管理

**檔案和專案是否有命名或結構需求？**

是。 由於整合使用Adobe企業儲存空間，因此適用下列慣例：

* 如果程式和專案屬於相同的投資組合，則不能有相同的名稱。

* 檔名稱在資料夾階層的相同父項中必須是唯一的。

* 相同專案中的檔案無法共用名稱。

* 程式、投資組合、專案、範本、任務、問題、檔案、檔案資料夾名稱不能包含下列特殊字元： `\ / : * ? " | < >`且限製為255個字元。

* 方案、投資組合、專案、範本、任務、問題和檔案資料夾不能有以句點或空格結尾的名稱。

Workfront會視需要自動重新命名物件或檔案，以避免衝突。

**Frame.io檢視器支援哪些檔案型別？**

Frame.io檢視器支援超過40種檔案格式，包括所有常見的視訊、影像、音訊、PDF和Microsoft Office型別。 視訊支援包括專業格式（例如ProRes、H.265和DNxHD）的原生播放，支援高達500 GB的檔案。

Frame.io是專為創意評論而建置，這表示它可處理行銷和創意團隊使用的各種資產型別。

+++

### 許可權和存取權

+++ 展開以檢視許可權和存取的常見問題。

**如何管理使用者許可權？**

您可以在Workfront中設定和控制使用者許可權，並自動傳遞至Frame.io。 您無法直接在Frame.io中邀請使用者或修改此整合的許可權。 所有存取權管理都必須使用Workfront中的專案共用模式完成。

下表顯示Workfront許可權對應至Frame.io許可權的方式：

<table>
  <thead>
    <tr>
      <th>Workfront許可權</th>
      <th>Frame.io許可權</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>管理</td>
      <td>編輯與共用</td>
    </tr>
    <tr>
      <td>參與</td>
      <td>編輯與共用</td>
    </tr>
    <tr>
      <td>檢視</td>
      <td>僅註解</td>
    </tr>
  </tbody>
</table>

+++


### 整合與進階功能

+++ 展開以檢視整合和進階功能的常見問題。

**這對現有的Creative Cloud外掛程式與Adobe Express和GenStudio的整合有何影響？**

支援Frame.io檢視器體驗的整合功能目前正在開發中，以便用於Adobe Express和GenStudio效能行銷。 新的整合將會建置在相同的統一檢閱和核准系統上，因此他們會利用Frame.io檢視器，針對所有三種產品提供一致的檢閱體驗。

**Frame.io是否已整合至Workfront，或是使用者是否導覽至個別介面？**

使用者可以直接從Workfront啟動Frame.io檢視器。 所有檢閱和核准活動都會在Frame.io檢視器中進行，並自動同步回Workfront。

**我可以傳送已核准的資產至Adobe Experience Manager (AEM)嗎？**

是。 資產完成複查和核准週期後，您就可以將其轉移至Adobe Experience Manager Assets進行最終儲存和分發。 這會將Workfront用於工作管理、Frame.io用於審查，以及AEM用於數位資產管理，連線到統一的內容supply chain。

如需詳細資訊，請參閱&lt;如需詳細資訊>，請參閱[使用Adobe Experience Manager與Frame.io整合](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

**統一檢閱和核准如何融入Adobe GenStudio？**

統一檢閱和核准是Adobe GenStudio的基本元件，Adobe對連線內容supply chain有更廣闊的視野。 GenStudio將Workfront、Frame.io、Creative Cloud、Adobe Express、Adobe Experience Manager Assets和GenStudio for Performance Marketing連線至行銷活動簡介到內容傳送的統一工作流程。

在該生態系統中，檢閱和核准是建立和傳遞之間的關鍵交接點。 它是創意工作與利害關係人意見相符的地方，品質經過驗證，內容經許可後可發佈。 當切換快速、可見且可靠時，它會解鎖整個supply chain內容的速度 — AI可以加速建立，自動化可以處理分發，但稽核的瓶頸限制了雙方的成果。 連線Workfront和Frame.io可移除該瓶頸。

**什麼是AI檢閱者功能？**

整合式稽核和核准包括AI稽核者功能，可在稽核程式中自動進行品牌合規性檢查。 AI稽核者可以根據品牌指南評估資產，並在人力稽核者參與之前指出潛在問題，幫助團隊更早發現問題並更快行動。

如需設定和使用AI檢閱者的詳細資訊，請參閱Experience League上的Workfront檔案。

+++

### 合約、SKU和儲存

+++ 展開以檢視合約、SKU和儲存的常見問題。

**我何時可以取得整合稽核和核准？**

整合式檢閱和核准現在可供使用。 存取許可權需要V2 Workfront SKU。 如果您的合約是在V2 Workfront SKU推出之前簽訂，則新增V2 Workfront SKU需要與Adobe進行合約活動。 路徑有兩種：

* 續約時：V2 Workfront SKU會於下次合約續約日期新增。

* 提早重新合約：您的Adobe客戶團隊可以提早重新合約，在保留現有合約結束日期的同時，新增V2 Workfront SKU權益。 移至同等套件時不會漲價。

請聯絡您的Adobe客戶代表，為您的組織決定最佳路徑。

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 Workfront SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 Workfront SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**升級至V2 Workfront SKU能給我更多儲存空間嗎？**

是。 透過V2 Workfront SKU，每個獲授權的使用者可接收60 GB的儲存空間，而舊版為30 GB。

**如何在Adobe企業儲存裝置與舊版Workfront儲存裝置之間進行選擇？**

企業儲存可啟用Frame.io檢視器體驗，且為統一檢閱和核准所必需。 舊版儲存繼續使用Workfront Proof檢視器(ProofHQ)作為預設值。

如果您的組織混合了簡單的工作流程和更複雜的校訂工作流程，您可以優先處理要先移轉的工作流程。

企業儲存提供您以遞增方式推出新體驗的彈性，從最有利的工作流程開始。

**如何管理Frame.io授權？**

簽署V2 Workfront SKU後，所有Workfront使用者都可存取Frame.io檢視器以進行檢閱和核准工作流程，不需個別的Frame.io Enterprise授權。

如果您的組織需要額外的Frame.io Enterprise功能，例如

* 進階浮水印（動態和取證）
* 具有自動資產刪除功能的數位版權管理
* AI產生內容的內容認證
* 自訂創意中繼資料
* Camera至雲端的整合
* 您自己的創意工作進行中工作區

您可以與Adobe客戶團隊合作，決定適當的Frame.io Enterprise授權數量。 所有授權均透過Adobe Admin Console管理。

+++

### 沙箱和轉出

+++ 展開以檢視沙箱和轉出的常見問題。

**我可以在沙箱環境中測試整合式稽核和核准嗎？**

部分。 核准工作流程可在Workfront沙箱環境中測試。 不過，沙箱中不提供Frame.io檢視器體驗。 測試檢閱表面本身需要生產環境。

若要限制轉出時的曝光度，您可以在Workfront生產環境中為特定群組啟用統一檢閱和核准。 這可讓您在更廣泛推出之前，先以較小的使用者集執行目標式試驗。

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### 互動式校訂和HTML

+++ 展開以檢視互動式校樣和HTML的常見問答集。

**整合式檢閱和核准是否支援互動式校訂或HTML URL？**

目前支援Zip HTML檔案進行互動式稽核。 HTML URL支援（即時Web URL審查）正在藍圖中，預計於第三季提供。

如需更新，請參閱Experience League上的Workfront發行說明。

+++

### Fusion與自動化

+++ 展開以檢視Fusion和自動化的常見問題。

**我是否需要Workfront Fusion才能使用統一的檢閱和核准？**

否。 整合式檢閱和核准是原生產品整合，不需要Fusion。 工作流程直接內建在Workfront中。

**Fusion Connectors是否可用於統一的檢閱和核准？**

是。 統一檢閱和核准的融合動作目前正在開發中，預計將於第3季推出。 檢視Experience League上的Workfront發行說明，瞭解更新何時可用。

**Fusion是否可以在檔案上傳時自動觸發稽核？**

是。 搭配Fusion使用Workfront Webhook即可進行這類自動化。

**在Workfront Proof上建立的現有Fusion工作流程將會受到什麼影響？**

其影響會因每個工作流程的建置方式而異。 一般而言：

* **編輯或更新**：可以更新現有校訂相關動作在統一核准中具有直接對等動作的工作流程，以使用新動作。

* **重新建置**：基礎步驟已大幅變更或存在新功能的工作流程，可能需要從頭重新建置。

統一核准的Fusion API一經可用，畫面就會更清晰。 建議稽核您現有的Fusion工作流程，並根據當時新的統一核准功能加以評估。

+++






