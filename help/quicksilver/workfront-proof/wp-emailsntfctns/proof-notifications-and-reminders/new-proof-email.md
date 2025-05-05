---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 新校訂電子郵件
description: 讓本文更適合PiW。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 新校訂電子郵件

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

當您建立新校訂或新版本的校訂、將新人員新增到校訂，或將工作流程新增到校訂時，您可以決定是否要向檢閱者傳送電子郵件，如以下文章所述：

* [使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [在 [!DNL Workfront Proof]中產生校樣](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

收件者收到的電子郵件稱為[!UICONTROL 新校訂]電子郵件。 只有校訂建立者和有權將檢閱者新增到校訂的使用者可以控制此電子郵件。 收件者無法將其停用。

新校樣電子郵件包含：

* 您的個人訊息（如果您選擇包含一則訊息）
* 如果您一律傳送相同的自訂訊息給檢閱者，最好將其儲存在[!UICONTROL 校訂預設值]標籤下的[!UICONTROL 個人設定]中。 如需詳細資訊，請參閱。
* 證明的個人連結
* **[!UICONTROL 檢視詳細資料]**&#x200B;連結，將您導向相關聯的[!DNL Workfront]物件（例如專案、任務或問題）
* 校樣影像的縮圖
* 以下校訂詳細資訊：

   * 校樣名稱
   * 版本號碼
   * 稽核者清單及其在校訂上的進度
   * 與其他人共用校訂的連結

     這可讓您共用原始檔案的校訂URL和/或下載連結。 這不允許您將檢閱者明確新增到校訂，您將只會共用公開的校訂URL，收件者將獲得對校訂的唯讀存取權。

     如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)中共用校訂。

     如果您不想讓此連結出現在收件者的電子郵件中，您可以停用校訂上的[!UICONTROL 公開共用]設定

     （下載原始檔案和公用URL）。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校訂詳細資訊。

## 活動記錄

傳送[!UICONTROL 新校訂]電子郵件給檢閱者記錄在[!UICONTROL 校訂詳細資料]頁面的[!UICONTROL 活動]區段。 如需詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中的管理[!UICONTROL 校訂詳細資料]。 您可以檢查在建立校訂時是否已啟用[!UICONTROL 新校訂]電子郵件。

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 如果校訂的建立者或擁有者依預設（在其個人設定中）已停用[!UICONTROL 校訂已製作]電子郵件，則他們將不會收到任何[!UICONTROL 校訂已製作]或[!UICONTROL 新校訂]電子郵件，即使在新校訂頁面上勾選[!UICONTROL 透過電子郵件通知人員]方塊亦然。 如需詳細資訊，請參閱。
>* 如果電子郵件通知在[!UICONTROL 帳戶設定]中停用為預設值，則校訂的建立者/擁有者將不會收到任何[!UICONTROL 校訂已製作]或[!UICONTROL 新校訂]電子郵件，即使這在其個人設定中已啟用且已在「新校訂」頁面上勾選[!UICONTROL 透過電子郵件通知]人員方塊。 如需詳細資訊，[校訂已進行[!UICONTROL 校訂]電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)並參閱。
>



## 啟用[!UICONTROL 新校訂]電子郵件並包含自訂訊息

您可以指定在建立校訂或新增某人時，是否要向校訂上的稽核者傳送電子郵件警報。

* [當您建立校訂時](#when-you-create-a-proof)
* [當您將檢閱者新增到校訂時](#when-you-add-a-reviewer-to-a-proof)

### 當您建立校訂時 {#when-you-create-a-proof}

當您在[!UICONTROL 新校訂]頁面的&#x200B;**[!UICONTROL 共用]**&#x200B;區段下建立新校訂時，您可以選取是否要傳送電子郵件警示：

* 您可以在此決定是否要[!UICONTROL 透過電子郵件通知別人] (1)。 如果您取消選取此選項，則沒有任何稽核者會收到電子郵件，告知他們校訂已準備好進行稽核。
* 您也可以在電子郵件通知(2)中加入「自訂」訊息。
* 如果您決定新增自己的自訂訊息，則可以在電子郵件內文中加入自訂主旨列(3)和訊息(4)。
* 若要捨棄自訂訊息，只要按一下連結(5)即可。

  >[!NOTE]
  >
  >如果您一律傳送相同的自訂訊息給檢閱者，最好將訊息儲存在[!UICONTROL 校訂預設值]標籤下的個人設定中。 如需詳細資訊，請參閱。

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 當您將檢閱者新增到校訂時 {#when-you-add-a-reviewer-to-a-proof}

如果新增到現有校訂的新檢閱者將收到校訂的通知（與上述類似），您可以進行選擇。

* 首先，在&#x200B;**[!UICONTROL 校訂詳細資料]**&#x200B;頁面(1)上按一下&#x200B;**[!UICONTROL 共用此版本]**&#x200B;按鈕，以新增檢閱者。

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 會出現一個方塊，您可在其中新增稽核者。 然後，您可以決定是否要以電子郵件通知他們(2)，並選擇將自訂訊息新增至電子郵件(3)。

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* 如果您選擇新增自訂訊息，方塊會展開，您可在電子郵件內文放入自訂主旨列(4)和自訂文字(5)。 您也可以按一下連結(6)以捨棄自訂訊息。

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
