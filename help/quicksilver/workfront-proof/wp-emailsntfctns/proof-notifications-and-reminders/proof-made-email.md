---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 校樣製作的電子郵件
description: 只有在校樣建立者已建立校樣時，才會傳送「校樣製作」電子郵件給校樣建立者。 如果某人已建立校樣並將另一人設為「擁有者」，則只有新擁有者也會收到「校樣」製作的電子郵件。 建立者和/或擁有者不會得到；他們只會收到「證明製作」電子郵件。 如需New Proof電子郵件的詳細資訊，請參閱New proof電子郵件。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# 此 [!UICONTROL 製作校樣] 電子郵件

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

A [!UICONTROL 製作校樣] 只有當證明建立者已建立證明時，才會傳送電子郵件給證明建立者。 如果某人已建立校樣並將另一人設為「擁有者」，則只有新擁有者也會收到 [!UICONTROL 證明] 電子郵件。 建立者和/或擁有者不會得到；他們只得到 [!UICONTROL 製作校樣] 電子郵件。 如需 [!UICONTROL 新校樣] 電子郵件，請參閱 [[!UICONTROL 新校樣] 電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

用戶可禁用 [!UICONTROL 製作校樣] 電子郵件，如下所述。

>[!NOTE]
>
> 如果校樣的建立者或擁有者 [!UICONTROL 製作校樣] 依預設在個人設定中停用的電子郵件，不會收到任何 [!UICONTROL 製作校樣] 或 [!UICONTROL 新校樣] 電子郵件，即使 [!UICONTROL 通過電子郵件通知人] 框 [!UICONTROL 新校樣] 頁面。

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

A [!UICONTROL 製作校樣] 電子郵件包含您的個人訊息（如果您包含其中一則），以及下列證明詳細資料：

* 校訂名稱
* 證明的個人連結
* 版本號
* 校樣縮圖
* 校訂進度
* 與他人共用校樣的連結
* 這可讓您共用原始檔案的校樣URL和/或下載連結。

>[!NOTE]
>
> 共用校樣連結不允許您明確將審核者新增至校樣，您只會共用公用校樣URL，而收件者將會收到校樣的唯讀存取權。

請參閱 [在中共用校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) 以取得更多資訊。

如果您不希望此連結出現在收件者的電子郵件中，則應停用 [!UICONTROL 公共共用] 校樣的設定([!UICONTROL 下載原始檔案] 和 [!UICONTROL 公用URL])。

## 停用 [!UICONTROL 製作校樣] 電子郵件

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，開啟 **[!UICONTROL 校對預設值]** ，然後按一下 **[!UICONTROL 停用]** 下一頁 **[!UICONTROL 校樣準備就緒時的電子郵件確認]**.

1. ![Proof_Made_-_pooking_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. 請參閱 [在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) 以取得更詳細的指示。
1. 如果 [!UICONTROL 帳戶設定]，校樣的建立者或擁有者將不會收到任何 [!UICONTROL 製作校樣] 或 [!UICONTROL 新校樣] 電子郵件，即使在其個人設定和 [!UICONTROL 通過電子郵件通知人] 框 [!UICONTROL 新校樣] 頁面。
