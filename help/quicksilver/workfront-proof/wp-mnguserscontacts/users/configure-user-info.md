---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 設定使用者資訊，使用 [!DNL Workfront Proof]
description: 設定使用者資訊，使用 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 設定使用者資訊，使用 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文提及獨立版產品中的功能 [!DNL Workfront Proof]. 有關內部校訂的資訊 [!DNL Adobe Workfront]，請參閱 [校訂](../../../review-and-approve-work/proofing/proofing.md).

1. 依照中的說明開始建立或編輯使用者 [建立使用者，使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 指定下列資訊：

   * 在 **[!UICONTROL 個人詳細資料]** 區段：

      * **電子郵件地址：** 使用者的電子郵件地址。
      * **名字：** 使用者的名字。
      * **姓氏：** 使用者的姓氏。
      * **位置：** 使用者在公司中的職位。
      * **許可權設定檔：** 使用者對校訂帳戶的許可權。
      * **語言：** 使用者的主要語言。
      * **時區：** 選取使用者的時區。
      * **日期格式：** 選取使用者偏好的日期格式。
      * **選擇加入 — 產品和行銷電子郵件：** 選擇是否讓使用者加入產品和行銷電子郵件。
      * **僅限API：** 僅允許使用者透過API登入。

   * 在 **[!UICONTROL 使用者詳細資訊]** 區段，輸入使用者的聯絡資訊，例如街道地址和電話號碼。
   * 在 **[!UICONTROL 預設校訂設定]** 區段，設定會影響使用者建立或處理校樣之方式的設定。

      * **預設校訂角色：** 選取使用者的預設校訂角色。 角色選項為 **[!UICONTROL 唯讀]**， **[!UICONTROL 檢閱者]**， **[!UICONTROL 核准者]**， **[!UICONTROL 檢閱者和核准者]**， **[!UICONTROL 作者]**，或 **[!UICONTROL 版主]**.

        如需校訂角色的詳細資訊，請參閱 [管理校訂角色於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **完成所有決定時鎖定校訂：** 在校樣的所有決定都完成後，自動鎖定校樣以防止進一步的變更。
      * **需要登入。 校訂只能與其他使用者共用：** 讓校訂僅供擁有以下身分的使用者使用： [!DNL Workfront Proof] 登入認證。
      * **只需要一個決定：** 只需要一個校訂決定。
      * **下載原始檔案：** 讓使用者下載原始檔案以進行校訂。 此選項預設為啟用。

        如需有關下載原始檔案的詳細資訊，請參閱 [下載儲存在中的檔案 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **訂閱。 人們可以透過公開URL或內嵌程式碼註冊校訂：** 允許組織外部的檢閱者透過公開URL或內嵌程式碼註冊校訂。

        選取此選項時， **訂閱者必須按一下電子郵件中的連結才能存取校訂** 也可供使用。 選取此選項可要求外部檢閱者按一下電子郵件內的連結以存取校訂。
如果符合以下條件，則此選項預設為啟用： **公開共用** 已選取選項。

      * **新來賓稽核者的預設角色：** 選取訪客檢閱者的預設校訂角色。 選項與中的相同 **預設校訂角色**，版主和作者除外。

   * 在 **[!UICONTROL 預設電子郵件警報設定]** 區段：

      * **預設電子郵件警示：** 選取使用者接收電子郵件更新的頻率。 選取 **所有活動、回覆我的意見、決定、最終決定、每小時摘要、每日摘要、** 或 **已停用**.

        如需預設電子郵件警示選項的詳細資訊，請參閱 [在中設定電子郵件通知設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **新訪客稽核者的預設電子郵件警報：** 選取訪客檢閱者接收電子郵件更新的頻率。 選項與相同 **預設電子郵件警示。**

      * **校樣準備就緒時傳送電子郵件確認：** 選取以在校樣準備就緒時自動向使用者傳送確認電子郵件。
      * **傳送給此使用者的電子郵件格式：** 選取 **[!UICONTROL HTML]** 或 **[!UICONTROL 純文字]** 作為傳送給使用者的電子郵件的預設格式。

   * 在 **[!UICONTROL 自訂訊息設定]** 區段：建立校訂範本的設定。

     如需範本的詳細資訊，請參閱：

      * **校訂主旨範本：** 為校訂主旨建立範本。
      * **校樣訊息範本：** 為校樣訊息及其格式建立範本。
