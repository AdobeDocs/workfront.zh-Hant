---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 使用 [!DNL Workfront Proof]設定使用者資訊
description: 使用 [!DNL Workfront Proof]設定使用者資訊
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 使用[!DNL Workfront Proof]設定使用者資訊

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

1. 開始建立或編輯使用者，如[使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md)建立使用者。
1. 指定下列資訊：

   * 在&#x200B;**[!UICONTROL 個人詳細資料]**&#x200B;區段中：

      * **電子郵件地址：**&#x200B;使用者的電子郵件地址。
      * **名字：**&#x200B;使用者的名字。
      * **姓氏：**&#x200B;使用者的姓氏。
      * **位置：**&#x200B;使用者在公司中的位置。
      * **許可權設定檔：**&#x200B;使用者對校訂帳戶的許可權。
      * **語言：**&#x200B;使用者的主要語言。
      * **時區：**&#x200B;選取使用者的時區。
      * **日期格式：**&#x200B;選取使用者偏好的日期格式。
      * **選擇加入 — 產品和行銷電子郵件：**&#x200B;選擇是否讓使用者加入產品和行銷電子郵件。
      * **僅限API：**&#x200B;僅允許使用者透過API登入。

   * 在&#x200B;**[!UICONTROL 使用者詳細資訊]**&#x200B;區段中，輸入使用者的聯絡資訊，例如街道地址和電話號碼。
   * 在&#x200B;**[!UICONTROL 預設校訂設定]**&#x200B;區段中，設定會影響使用者建立或處理校訂方式的設定。

      * **預設校訂角色：**&#x200B;為使用者選取預設校訂角色。 角色選項為&#x200B;**[!UICONTROL 唯讀]**、**[!UICONTROL 檢閱者]**、**[!UICONTROL 核准者]**、**[!UICONTROL 檢閱者和核准者]**、**[!UICONTROL 作者]**&#x200B;或&#x200B;**[!UICONTROL 仲裁者]**。

        如需校訂角色的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

      * **完成所有決定時鎖定校訂：**&#x200B;對校訂做出所有決定後，自動鎖定校訂以防止進一步變更。
      * **需要登入。 校訂只能與其他使用者共用：**&#x200B;讓校訂僅供具有[!DNL Workfront Proof]登入認證的使用者使用。
      * **只需要一個決定：**&#x200B;只需要一個關於校訂的決定。
      * **下載原始檔案：**&#x200B;讓使用者下載原始檔案以進行校訂。 此選項預設為啟用。

        如需有關下載原始檔案的詳細資訊，請參閱[下載儲存在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)中的檔案。

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **訂閱。 人員可以透過公用URL或內嵌程式碼註冊校訂：**&#x200B;允許組織外部的檢閱者透過公用URL或內嵌程式碼註冊校訂。

        選取此選項時，**訂閱者必須按一下電子郵件中的連結，才能存取校訂**。 選取此選項可要求外部檢閱者按一下電子郵件內的連結以存取校訂。
如果已選取**公用共用**&#x200B;選項，則預設會啟用此選項。

      * **新來賓檢閱者的預設角色：**&#x200B;請為來賓檢閱者選取預設校訂角色。 選項與&#x200B;**預設校訂角色**&#x200B;中的選項相同，但版主和作者除外。

   * 在&#x200B;**[!UICONTROL 預設電子郵件警示設定]**&#x200B;區段中：

      * **預設電子郵件警示：**&#x200B;選取使用者接收電子郵件更新的頻率。 選取&#x200B;**所有活動、回覆我的意見、決定、最終決定、每小時摘要、每日摘要、**&#x200B;或&#x200B;**已停用**。

        如需預設電子郵件警示選項的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中設定電子郵件通知設定

      * **新訪客檢閱者的預設電子郵件警示：**&#x200B;選取訪客檢閱者接收電子郵件更新的頻率。 選項與&#x200B;**預設電子郵件警示的選項相同。**

      * **在校訂就緒時傳送電子郵件確認：**&#x200B;選取以在校訂就緒時自動傳送確認電子郵件給使用者。
      * **傳送給此使用者的電子郵件格式：**&#x200B;選取&#x200B;**[!UICONTROL HTML]**&#x200B;或&#x200B;**[!UICONTROL 純文字]**&#x200B;作為傳送給使用者的電子郵件的預設格式。

   * 在&#x200B;**[!UICONTROL 自訂訊息設定]**&#x200B;區段中：建立校訂範本的設定。

     如需範本的詳細資訊，請參閱：

      * **校訂主旨範本：**&#x200B;建立校訂主旨的範本。
      * **校訂訊息範本：**&#x200B;建立校訂訊息及其格式的範本。
