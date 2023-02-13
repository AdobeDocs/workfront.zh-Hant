---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 使用 [!DNL Workfront Proof]
description: 使用 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 使用 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

1. 如 [使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 指定下列資訊：

   * 在 **[!UICONTROL 個人詳細資訊]** 小節：

      * **電子郵件地址：** 使用者的電子郵件地址。
      * **名字：** 使用者的名字。
      * **姓氏：** 使用者的姓氏。
      * **位置：** 使用者在公司中的位置。
      * **權限配置檔案：** 使用者對校樣帳戶的權限。
      * **語言：** 使用者的主要語言。
      * **時區：** 選取使用者的時區。
      * **日期格式：** 選取使用者偏好的日期格式。
      * **選擇加入 — 產品與行銷電子郵件：** 選取是否選擇使用者加入產品和行銷電子郵件。
      * **僅限API:** 僅允許使用者透過API登入。
   * 在 **[!UICONTROL 使用者詳細資料]** 區段，鍵入用戶的聯繫資訊，如街道地址和電話號碼。
   * 在 **[!UICONTROL 預設校樣設定]** 區段中，配置影響使用者建立或處理校樣的方式的設定。

      * **預設校樣角色：** 為用戶選擇預設校樣角色。 角色選項包括 **[!UICONTROL 唯讀]**, **[!UICONTROL 審核者]**, **[!UICONTROL 核准者]**, **[!UICONTROL 審核者與核准者]**, **[!UICONTROL 作者]**，或 **[!UICONTROL 版主]**.

         如需校樣角色的詳細資訊，請參閱 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **做出所有決定時鎖定證明：** 在對校樣做出所有決策後，自動鎖定校樣，使其不再進行更改。
      * **需要登入。 校樣只能與其他使用者共用：** 使校樣僅供具有 [!DNL Workfront Proof] 登入憑證。
      * **只需要一個決定：** 只需要一個證明決定。
      * **下載原始檔案：** 可讓使用者下載原始檔案以進行校樣。 預設會啟用此選項。

         如需下載原始檔案的詳細資訊，請參閱 [下載儲存在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **訂閱。 人們可以透過公開URL或內嵌程式碼註冊校樣：** 可讓組織外部的審核者透過公開URL或內嵌程式碼註冊校樣。

         選取此選項時， **訂閱者必須按一下電子郵件中的連結才能存取校樣** 也可用。 選取此選項，要求外部審核者按一下電子郵件中的連結以存取校樣。
如果 **公共共用** 選項。

      * **新來賓審核者的預設角色：** 為來賓審核者選擇預設校樣角色。 選項與 **預設校樣角色。**
   * 在 **[!UICONTROL 預設電子郵件警報設定]** 小節：

      * **預設電子郵件警報：** 選取使用者收到電子郵件更新的頻率。 選擇 **所有活動、對我的評論的回覆、決策、最終決策、每小時摘要、每日摘要** 或 **已停用**.

         如需預設電子郵件警報選項的詳細資訊，請參閱 [在中配置電子郵件通知設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **新來賓審核者的預設電子郵件警報：** 選擇來賓審核者接收電子郵件更新的頻率。 選項與 **預設電子郵件警報。**

      * **校樣就緒時，傳送電子郵件確認：** 選取，在校樣就緒時自動傳送確認電子郵件給使用者。
      * **傳送給此使用者的電子郵件格式：** 選擇 **[!UICONTROL HTML]** 或 **[!UICONTROL 純文字]** 作為傳送給使用者之電子郵件的預設格式。
   * 在 **[!UICONTROL 自訂訊息設定]** 小節：建立校樣範本的設定。

      如需範本的詳細資訊，請參閱：

      * **校樣主題模板：** 建立校樣主題的範本。
      * **校樣訊息範本：** 建立校樣訊息及其格式的範本。
