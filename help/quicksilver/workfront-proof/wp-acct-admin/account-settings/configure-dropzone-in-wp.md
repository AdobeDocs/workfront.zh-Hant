---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 在 [!DNL Workfront Proof]
description: As a [!DNL Workfront Proof] 管理員，您可以設定、檢視及編輯使用者的Dropzone設定。 如需Dropzone的相關資訊，請參閱Dropzone。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 在 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] 管理員，您可以設定、檢視及編輯使用者的Dropzone設定。 如需Dropzone的相關資訊，請參閱 [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**，然後開啟 **[!UICONTROL Dropzone]** 標籤。

1. 在 **[!UICONTROL Dropzone詳細資訊]** 小節：

   * **[!UICONTROL Web放置區]**:啟用或停用「放置區」。
   * **[!UICONTROL Web放置區URL]**:您必須在瀏覽器中輸入的URL，才能透過Dropzone提交校樣。
   * **[!UICONTROL 電子郵件放置區]**:啟用或停用「電子郵件放置」。

      >[!NOTE]
      >
      >不再支援以電子郵件傳送至dropzones。

   * **[!UICONTROL Dropzone所有者]**:設定或編輯Dropzone所有者。 這個人會收到Dropzone新提交內容的通知。 要設定為Dropzone所有者，用戶必須是主管、管理員、計費管理員或帳戶建立者。 如需詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL 建立者的預設角色]**:所有提交者都會以此角色為預設新增至校樣。
   * **[!UICONTROL 所有建立者的電子郵件通知]**:在此處設定校樣建立者（提交者）的電子郵件警報偏好設定。 請參閱 [在中配置電子郵件通知設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) 有關可用的不同警報設定的資訊。

   * **[!UICONTROL 新版本函式]**:在Dropzone上啟用並停用「新版本」功能。 如此一來，使用者就能透過Dropzone提交新版本校樣。
   * **[!UICONTROL 在（天）之後刪除草稿校樣]**:指定刪除草稿校樣的天數。 如果將檔案上傳至Dropzone後，Dropzone提交作業未完成，校樣會維持草稿狀態。
   * **[!UICONTROL 隱藏審閱者角色]**:將人員新增至Dropzone時隱藏審核者角色欄位。
   * **[!UICONTROL 啟動時傳送校樣訊息]**:設定 [!DNL Workfront Proof] 啟用校樣時，自動傳送校樣通知電子郵件給審核者。
   * **[!UICONTROL 啟用提交校樣]**:設定 [!DNL Workfront Proof] 在提交時自動啟用校樣（不需要手動啟用）。

   * 如果校樣已移出Dropzone（例如，移至您帳戶中的其他資料夾），則Dropzone設定將不再套用至校樣。 這在電子郵件警報設定方面尤其重要。

1. 在 **[!UICONTROL Dropzone欄位]** 區段來指定 [!UICONTROL 校樣詳細資料] 填入透過Dropzone提交校樣時的區段。
1. 在 **[!UICONTROL 允許的網域]** 區段中，指定您希望允許使用「放置區」的網域。

   * 您可以按一下 **[!UICONTROL 新增網域]** 添加域。 添加完域詳細資訊後，按一下 **[!UICONTROL 儲存]**.

   * 您可以 **[!UICONTROL 編輯]** 和 **[!UICONTROL 刪除]** 您先前新增的任何現有網域。

1. 在 **[!UICONTROL 要通知的人]**，請在將新校樣提交至Dropzone時，指定要通知的對象，以及「放置區」擁有者 [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * 按一下 **[!UICONTROL 新增人員]**，輸入收件者的詳細資訊，然後按一下 **[!UICONTROL 儲存]**.

   * **[!UICONTROL 刪除]** 您先前新增的人員。
