---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 新校樣電子郵件
description: 讓本文更適合PiW。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 新校樣電子郵件

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

當您建立新校樣或新版本的校樣、新增人員至校樣或將工作流程新增至校樣時，可以決定是否要依照以下文章所述傳送電子郵件給審核者：

* [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

您的收件者收到的電子郵件稱為 [!UICONTROL 新校樣] 電子郵件。 只有校樣建立者和獲授權將審閱者新增至校樣的使用者才能控制此電子郵件。 收件者無法加以停用。

新校樣電子郵件包含：

* 您的個人訊息（如果您選擇加入）
* 如果您一律會傳送相同的自訂訊息給審核者，最好將其儲存在 [!UICONTROL 個人設定] 在 [!UICONTROL 校對預設值] 標籤。 如需詳細資訊，請參閱。
* 證明的個人連結
* **[!UICONTROL 查看詳細資訊]** 將您導向至 [!DNL Workfront] 對象（如項目、任務或問題）
* 校樣影像的縮圖
* 下列校樣詳細資料：

   * 校訂名稱
   * 版本號

      如需詳細資訊，請參閱。

   * 審查者清單及其證明進展
   * 與他人共用校樣的連結

      這可讓您共用原始檔案的校樣URL和/或下載連結。 這不允許您明確將審核者新增至校樣，您只會共用公用校樣URL，而收件者將收到校樣的唯讀存取權。

      請參閱 [在中共用校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) 以取得更多資訊。

      如果您不希望此連結出現在收件者的電子郵件中，您可以停用 [!UICONTROL 公共共用] 校樣的設定

      （下載原始檔案和公用URL）。 請參閱 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以取得更多資訊。

## 活動記錄

傳送 [!UICONTROL 新校樣] 已登入給審核者的電子郵件 [!UICONTROL 活動] 區段 [!UICONTROL 校樣詳細資料] 頁面。 請參閱  [管理[!UICONTROL  校樣詳細資料] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以取得更多資訊。 您可以檢查 [!UICONTROL 新校樣] 建立校樣時已啟用電子郵件。

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 如果校樣的建立者或擁有者 [!UICONTROL 製作校樣] 依預設會停用的電子郵件（在其個人設定中），不會收到任何 [!UICONTROL 證明] 或 [!UICONTROL 新校樣] 即使 [!UICONTROL 通過電子郵件通知人] 框中，選擇「新建校樣」。 如需詳細資訊，請參閱。
>* 如果 [!UICONTROL 帳戶設定] 校樣的建立者/擁有者不會收到任何 [!UICONTROL 證明] 或 [!UICONTROL 新校樣] 即使在其個人設定和 [!UICONTROL 通知] 「新增校樣」頁面上會勾選「以電子郵件方式查看人員」方塊。 如需詳細資訊， [此 [!UICONTROL 製作校樣] 電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 和請參閱。
>




## 啟用 [!UICONTROL 新校樣] 電子郵件和包含自訂訊息

您可以指定在建立校樣時，還是在您新增某人時，要將電子郵件警報傳送給校樣的審核者。

* [建立校樣時](#when-you-create-a-proof)
* [將審核者添加到校樣時](#when-you-add-a-reviewer-to-a-proof)

### 建立校樣時 {#when-you-create-a-proof}

當您在 [!UICONTROL 新校樣] 頁面下方 **[!UICONTROL 共用]** 區段中，您可以選取是否要傳送電子郵件警報：

* 您可以在此決定是否要 [!UICONTROL 通過電子郵件通知人] (1)。 如果您取消選取此選項，審核者將不會收到電子郵件，通知他們校樣已可供審核。
* 您也可以在電子郵件通知(2)中包含自訂訊息。
* 如果您決定新增自訂訊息，則可放入自訂主旨行(3)，以及電子郵件(4)內文的訊息。
* 若要捨棄自訂訊息，只需按一下連結(5)即可。

   >[!NOTE]
   >
   >如果您一律會傳送相同的自訂訊息給審核者，最好將訊息儲存在「個人設定」下的 [!UICONTROL 校對預設值] 標籤。 如需詳細資訊，請參閱。

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 將審核者添加到校樣時 {#when-you-add-a-reviewer-to-a-proof}

您可以選取新增至現有校樣的新審核者是否會收到校樣的通知（類似上方）。

* 首先，按一下 **[!UICONTROL 共用此版本]** 按鈕 **[!UICONTROL 校樣詳細資料]** 頁面(1)。

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 此時將出現一個框，您可以在其中添加新審閱者。 然後，您可以決定是否希望電子郵件(2)通知他們，並選擇將自訂訊息新增至電子郵件(3)。

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* 如果您選擇新增自訂訊息，方塊會展開，您就能放入自訂主旨行(4)，以及電子郵件內文(5)中的自訂文字。 您也可以按一下連結(6)來捨棄自訂訊息。

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
