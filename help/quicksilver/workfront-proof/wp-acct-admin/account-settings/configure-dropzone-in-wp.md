---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 在 [!DNL Workfront Proof]中設定下拉區域
description: 作為 [!DNL Workfront Proof] 管理員，您可以設定、檢視及編輯使用者的拖放區域設定。 如需拖放區域的詳細資訊，請參閱拖放區域。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中設定dropzone

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

作為[!DNL Workfront Proof]管理員，您可以設定、檢視及編輯使用者的拖放區域設定。 如需有關拖放區域的資訊，請參閱[拖放區域](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)。

1. 按一下「**[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**」，然後開啟「**[!UICONTROL 拖放區域]**」標籤。

1. 在&#x200B;**[!UICONTROL 拖放區域詳細資料]**&#x200B;區段中進行下列任何變更：

   * **[!UICONTROL 網頁拖放區域]**：啟用或停用拖放區域。
   * **[!UICONTROL 網頁拖放區域URL]**：您必須輸入瀏覽器的URL，才能透過Dropzone提交校樣。
   * **[!UICONTROL 電子郵件Dropzone]**：啟用或停用電子郵件Dropzone。

     >[!NOTE]
     >
     >不再支援以電子郵件傳送至dropzones。

   * **[!UICONTROL 拖放區域擁有者]**：設定或編輯拖放區域擁有者。 這是會收到新提交至Dropzone通知的人。 若要設定為拖放區域擁有者，使用者必須是監督員、管理員、帳單管理員或帳戶建立者。 如需詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的校訂許可權設定檔。

   * **[!UICONTROL 建立者的預設角色]**：所有提交者都已新增到校訂中，此角色為預設角色。
   * **[!UICONTROL 所有建立者的電子郵件通知]**：在此設定校訂建立者（提交者）的電子郵件通知偏好設定。 請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中設定電子郵件通知設定，以取得不同可用警示設定的相關資訊。

   * **[!UICONTROL 新版本函式]**：在Dropzone上啟用和停用New Version函式。 這會讓或移除使用者透過Dropzone提交新版校樣的能力。
   * **[!UICONTROL 在（天）之後刪除草稿校訂]**：指定將刪除草稿校訂的天數。 如果在將檔案上傳到Dropzone後Dropzone提交未完成，校訂仍維持在草稿狀態。
   * **[!UICONTROL 隱藏檢閱者角色]**：將人員新增至Dropzone時隱藏檢閱者角色欄位。
   * **[!UICONTROL 啟動時傳送校訂訊息]**：設定[!DNL Workfront Proof]，在啟動校訂時自動傳送校訂通知電子郵件給檢閱者。
   * **[!UICONTROL 在提交時啟用校訂]**：設定[!DNL Workfront Proof]在提交時自動啟用校訂（移除手動啟用校訂的需求）。

   * 如果校訂移出Dropzone （例如，到您帳戶中的另一個資料夾），Dropzone設定將不再套用於校訂。 這對於電子郵件警報設定尤其重要。

1. 在&#x200B;**[!UICONTROL 拖放區域欄位]**&#x200B;區段中進行任何變更，以指定透過Dropzone提交校樣時，哪些欄位會顯示在Dropzone提交頁面的[!UICONTROL 校樣詳細資料]區段中。
1. 在&#x200B;**[!UICONTROL 允許的網域]**&#x200B;區段中，指定您要允許使用Dropzone的網域。

   * 您可以按一下&#x200B;**[!UICONTROL 新增網域]**&#x200B;以新增網域。 完成新增網域詳細資料後，請按一下[儲存]。**&#x200B;**

   * 您可以&#x200B;**[!UICONTROL 編輯]**&#x200B;和&#x200B;**[!UICONTROL 刪除]**&#x200B;您先前新增的任何現有網域。

1. 在&#x200B;**[!UICONTROL 要通知的人員]**&#x200B;底下，指定當新校樣提交至拖放區域[拖放區域](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)時，要通知的人員以及拖放區域擁有者

   * 按一下&#x200B;**[!UICONTROL 新增人員]**，輸入收件者的詳細資料，然後按一下&#x200B;**[!UICONTROL 儲存]**。

   * **[!UICONTROL 刪除您先前新增的]**&#x200B;人員。
