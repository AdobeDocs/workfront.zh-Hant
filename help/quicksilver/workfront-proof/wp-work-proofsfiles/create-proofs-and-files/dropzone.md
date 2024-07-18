---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: 下拉區域
description: 如果您有企業計畫，則可使用Dropzone向您的帳戶提交新校訂和新版本的校訂，而無需登入您的帳戶。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# 下拉區域

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您有企業計畫，則可使用Dropzone向您的帳戶提交新校訂和新版本的校訂，而無需登入您的帳戶。

當您透過Dropzone提交校訂時，它會顯示在[!DNL Workfront Proof]帳戶的Dropzone頁面中。 從那裡，您可以將其路由到您的工作流程中。

## 透過Dropzone URL提交新校訂

1. 在您的瀏覽器中，移至唯一的拖放區域URL，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定拖放區域中所述
1. 輸入您的電子郵件地址。
1. 按一下&#x200B;**[!UICONTROL 選取檔案]**&#x200B;或&#x200B;**[!UICONTROL 擷取網頁]**，然後選擇您要上傳的檔案或網頁。

1. 輸入安全碼，然後按[下一步] ****。\
   進度列會顯示上傳的進度。\
   在下一個畫面中，您將能夠新增校訂詳細資訊。\
   請注意，此區段只有在已於拖放區域設定中啟用時才會顯示。

1. 填妥詳細資料後，請按[下一步]。****
1. 新增到校訂的任何檢閱者將只會在校訂啟動時收到通知電子郵件（請參閱下文）。
1. 將校樣提交到Dropzone後，您的校樣會經歷以下狀態：

   * 第一次將檔案上傳到拖放區域時，校樣會在那裡顯示為草稿。
   * 提交完成後，證明會在您的放置區顯示為已提交。
   * 在啟動和解鎖校訂後，它在您的拖放區域中顯示為使用中。
   * 如果校訂已鎖定，在您的Dropzone中會顯示為「已鎖定」。

## 透過Dropzone URL提交現有校訂的新版本

1. 在您的瀏覽器中，移至唯一的拖放區域URL，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定拖放區域中所述
1. 輸入您的電子郵件地址。
1. 選取核取方塊以表示您正在上傳現有校訂的新版本。\
   如需建立新版校訂的相關資訊，請參閱。
1. 按一下&#x200B;**[!UICONTROL 選取檔案]**&#x200B;或&#x200B;**[!UICONTROL 擷取網頁]**，然後選擇您要上傳的檔案或網頁。

1. 輸入安全碼，然後按[下一步] ****。\
   進度列會顯示上傳的進度。\
   Workfront Proof傳送驗證電子郵件給您。

1. 按一下電子郵件中的連結。\
   電子郵件會在您的瀏覽器中開啟Dropzone視窗。 電子郵件通知中的連結有效期為24小時。
1. 選取校訂的先前版本（只會顯示您建立/提交的校訂）。\
   在下一個畫面中，您將能夠新增校訂詳細資訊。\
   此區段只有在已在Dropzone設定中啟用時才會顯示。

1. 輸入詳細資料，按一下&#x200B;**[!UICONTROL 下一步]**。

   >[!NOTE]
   >
   >新增到校訂的任何檢閱者將只會在校訂啟動時收到通知電子郵件（請參閱下文）。

   將校樣提交到Dropzone後，您的校樣會經歷以下狀態：

   * 第一次將檔案上傳到拖放區域時，校樣會在那裡顯示為草稿。
   * 提交完成後，證明會在您的放置區顯示為已提交。
   * 在啟動和解鎖校訂後，它在您的拖放區域中顯示為使用中。
   * 如果校訂已鎖定，在您的Dropzone中會顯示為「已鎖定」。

## 以電子郵件傳送證明給Dropzone

>[!NOTE]
>
>不再支援透過電子郵件將校樣傳送到dropzone。


## 正在完成您的提交

Workfront會傳送一封完整的提交電子郵件給您（提交者），要求您確認檔案是新校訂還是新版本。 電子郵件通知中的連結有效期為24小時。

1. 視是新校訂還是現有校訂的新版本而定，按一下連結並按照上述步驟操作。

## 啟動校訂

Dropzone所有者會收到通知電子郵件，通知您已向Dropzone提交新校訂：

* 校訂會顯示在您帳戶的Dropzone頁面中（若要存取Dropzone頁面，請按一下左側導覽側邊欄中的連結）。
* 拖放區域所有者（或至少擁有監督員設定檔的使用者）可以存取校訂。 擁有者可在Dropzone設定中變更（只有帳單管理員或管理員可以執行此操作）。
* 必須先由Dropzone所有者啟用/解除鎖定，校訂才能運作（至少具有主管設定檔的使用者也可這麼做）。 在啟用/解除鎖定之前，校訂的狀態會顯示為「已提交」。

啟動校訂：

1. 移至校訂右側的下拉式功能表，然後按一下&#x200B;**[!UICONTROL 啟動]**。
1. 啟動/解除鎖定校訂後：

   * 校訂狀態會變更為作用中。
   * 新增到校訂的任何人都會收到通知電子郵件，通知他們要檢閱新的校訂。 （在啟動/解除鎖定校訂之前，不會傳送電子郵件。）
   * 證明可以正常運作
   * 如果提交者也明確將自己新增到校樣中，他們將不會收到新校樣電子郵件。 如需詳細資訊，請參閱[新校訂電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

## 管理您的Dropzone

Dropzone頁面可讓您輕鬆管理對Dropzone的提交。 您的Dropzone頁面包含下列選項和功能：

* 頁面配置(1)
* 選擇在檢視中包含/排除封存的校樣(2)
* 動作按鈕(3)
* 排序(4)
* 篩選器(5)
* 校訂動作選單(6)
* 取消封存證明(7)
* 展開/摺疊校樣摘要(8)
* 選取校訂(9)

頁面配置、排序和篩選選項與[!DNL Views]清單中的選項相同。 如需詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中檢視頁面上的[管理專案。

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
