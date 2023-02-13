---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: 如果您有企業計畫，則可以使用Dropzone，將新校樣和新版本的校樣提交至帳戶，而無須登入帳戶。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您有企業計畫，則可以使用Dropzone，將新校樣和新版本的校樣提交至帳戶，而無須登入帳戶。

透過Dropzone提交校樣時，校樣會顯示在您 [!DNL Workfront Proof] 帳戶。 從那裡，您可以將其路由至工作流程。

## 透過Dropzone URL提交新校樣

1. 在瀏覽器中，前往唯一的Dropzone URL，如 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 輸入您的電子郵件地址.
1. 按一下 **[!UICONTROL 選取檔案]** 或 **[!UICONTROL 擷取網頁]** 並選擇要上載的檔案或網頁。

1. 輸入安全代碼，然後按一下 **[!UICONTROL 下一個]**.\
   進度列會顯示上傳的進度。\
   在下一個畫面中，您將能新增校樣詳細資訊。\
   請注意，只有在「放置區」設定中已啟用此區段時，才會顯示此區段。

1. 填妥詳細資料後，按一下 **[!UICONTROL 下一個]**.
1. 任何新增至校樣的審核者，只有在啟動校樣後，才會收到其通知電子郵件（請參閱下方）。
1. 將校樣提交至Dropzone後，會經過下列狀態：

   * 第一次將檔案上傳至Dropzone時，校樣會以「草稿」顯示。
   * 提交完成後，校樣會在您的Dropzone中顯示為「已提交」。
   * 校樣啟動並解除鎖定後，在您的Dropzone中就會顯示為「作用中」。
   * 如果校樣已鎖定，在您的Dropzone中會顯示為「已鎖定」。

## 透過Dropzone URL提交新版本的現有校樣

1. 在瀏覽器中，前往唯一的Dropzone URL，如 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 輸入您的電子郵件地址.
1. 選取核取方塊，指出您正在上傳新版本的現有校樣。\
   如需建立新版校樣的資訊，請參閱。
1. 按一下 **[!UICONTROL 選取檔案]** 或 **[!UICONTROL 擷取網頁]** 並選擇要上載的檔案或網頁。

1. 輸入安全代碼，然後按一下 **[!UICONTROL 下一個]**.\
   進度列會顯示上傳的進度。\
   Workfront Proof會傳送驗證電子郵件給您。

1. 按一下電子郵件中的連結。\
   電子郵件會開啟瀏覽器中的「放置區」視窗。 電子郵件通知中的連結有效期為24小時。
1. 選取舊版校樣（只會顯示您建立/提交的校樣）。\
   在下一個畫面中，您將能新增校樣詳細資訊。\
   只有在「放置區」設定中已啟用此區段時，才會顯示此區段。

1. 輸入詳細資訊，按一下 **[!UICONTROL 下一個]**.

   >[!NOTE]
   >
   >任何新增至校樣的審核者，只有在啟動校樣後，才會收到其通知電子郵件（請參閱下方）。

   將校樣提交至Dropzone後，會經過下列狀態：

   * 第一次將檔案上傳至Dropzone時，校樣會以「草稿」顯示。
   * 提交完成後，校樣會在您的Dropzone中顯示為「已提交」。
   * 校樣啟動並解除鎖定後，在您的Dropzone中就會顯示為「作用中」。
   * 如果校樣已鎖定，在您的Dropzone中會顯示為「已鎖定」。

## 將校樣以電子郵件傳送至Dropzone

>[!NOTE]
>
>不再支援將校樣透過電子郵件傳送至dropzone。


## 完成提交

Workfront會傳送「完成提交」電子郵件給您，要求您確認檔案是新校樣還是新版本。 電子郵件通知中的連結有效期為24小時。

1. 視其為新校樣或現有校樣的新版本而定，按一下連結並遵循上述步驟。

## 啟用校樣

Dropzone擁有者會收到通知電子郵件，告知他們已將新校樣提交至Dropzone:

* 校樣會顯示在您帳戶的「Dropzone」頁面中（若要存取「Dropzone」頁面，請按一下左側導覽側欄中的連結）。
* 校樣可由Dropzone擁有者（或至少具有「主管」設定檔的使用者）存取。 擁有者可在Dropzone設定中變更（只有帳單管理員或管理員才能變更）。
* 校樣工作之前，必須由Dropzone所有者激活/解除鎖定（至少具有主管配置檔案的用戶也可以啟用/解除鎖定）。 校樣的狀態會顯示為已提交，直到它啟動/解除鎖定為止。

若要啟用校樣：

1. 前往校樣右側的下拉式功能表，然後按一下 **[!UICONTROL 啟動]**.
1. 校樣啟動/解除鎖定後：

   * 校樣狀態變更為「活動」。
   * 任何已新增至校樣的人都會收到通知電子郵件，告知他們有要檢閱的新校樣。 （在啟用/解除鎖定校樣之前，不會傳送任何電子郵件。）
   * 證據可以正常處理
   * 如果提交者也將自己顯式添加到校樣中，則他們將不會收到新校樣電子郵件。 如需詳細資訊，請參閱 [新校樣電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## 管理您的Dropzone

「放置區」頁面可讓您輕鬆管理提交至放置區的作業。 您的Dropzone頁面包含下列選項和功能：

* 頁面配置(1)
* 選擇在檢視中包含/排除已封存的校樣(2)
* 動作按鈕(3)
* 排序(4)
* 篩選器(5)
* 校樣動作功能表(6)
* 取消校樣(7)
* 展開/折疊校樣摘要(8)
* 選擇校樣(9)

頁面配置、排序和篩選選項與 [!DNL Views] 清單。 請參閱 [管理中檢視頁面上的項目 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 以取得更多資訊。

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
