---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 校樣已製作電子郵件
description: 校樣建立者建立校樣後，才會向校樣建立者傳送電子郵件。 如果某人已建立校訂並將另一個人設為擁有者，則只有新擁有者會收到已建立校訂的電子郵件。 建立者和/或擁有者不會收到校訂；他們只會收到「校訂已製作」電子郵件。 如需新校訂電子郵件的詳細資訊，請參閱新校訂電子郵件。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# [!UICONTROL 校訂已進行]電子郵件

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

僅當校訂建立者已建立校訂時，才會將[!UICONTROL 校訂製作]電子郵件傳送給校訂建立者。 如果某人已建立校訂並將另一個人設為擁有者，則只有新擁有者會收到已建立的[!UICONTROL 校訂]電子郵件。 建立者和/或擁有者不會收到校訂；他們只會收到[!UICONTROL 校訂製作]電子郵件。 如需[!UICONTROL 新校訂]電子郵件的詳細資訊，請參閱[[!UICONTROL 新校訂]電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

使用者可以在他們的設定檔設定中停用[!UICONTROL 校訂已製作]電子郵件，如下所述。

>[!NOTE]
>
> 如果校訂的建立者或擁有者在其個人設定中依預設已停用[!UICONTROL 校訂已製作]電子郵件，則他們不會收到任何[!UICONTROL 校訂已製作]或[!UICONTROL 新校訂]電子郵件，即使[!UICONTROL 新校訂]頁面上的[!UICONTROL 透過電子郵件通知人員]方塊已核取。

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

[!UICONTROL 校訂已進行]電子郵件包含您的個人訊息（如果您包含其中一封）和下列校訂詳細資訊：

* 校樣名稱
* 證明的個人連結
* 版本號碼
* 校訂的縮圖
* 校訂進度
* 與他人共用校訂的連結
* 這可讓您共用原始檔案的校訂URL和/或下載連結。

>[!NOTE]
>
> 共用校訂連結不允許您明確將檢閱者新增至校訂、您只會共用公開校訂URL，且收件者將取得校訂的唯讀存取權。

如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)中共用校訂。

如果您不想讓此連結出現在收件者的電子郵件中，您應該停用校訂上的[!UICONTROL 公開共用]設定（[!UICONTROL 下載原始檔案]和[!UICONTROL 公開URL]）。

## 正在停用[!UICONTROL 校訂已製作]電子郵件

1. 按一下&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，開啟&#x200B;**[!UICONTROL 校訂預設值]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL 校訂就緒時電子郵件確認旁的**[!UICONTROL &#x200B;停用&#x200B;]**]**。

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. 請參閱[在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)以取得更詳細的指示。
1. 如果[!UICONTROL 帳戶設定]中的電子郵件通知預設為停用，則校訂的建立者或擁有者將不會收到任何[!UICONTROL 校訂已製作]或[!UICONTROL 新校訂]電子郵件，即使這已在他們的個人設定中啟用且已在[!UICONTROL 新校訂]頁面上勾選[!UICONTROL 透過電子郵件通知人員]方塊。
