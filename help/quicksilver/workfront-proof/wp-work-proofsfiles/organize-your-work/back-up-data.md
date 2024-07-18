---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 備份您的 [!DNL Workfront Proof] 資料
description: 您可以使用備份函式，要求備份 [!DNL Workfront Proof] 中的所有資料。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 備份您的[!DNL Workfront Proof]資料

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

## 備份簡介

您可以使用備份函式，要求備份[!DNL Workfront Proof]中的所有資料。

備份會以.zip檔案形式傳送給您。 它包含您所有資料的XML匯出（包括所有校訂所有版本的註釋和回應）；但是，它不包含您上傳為校訂的原始檔案。

為您建立以供下載的每個備份.zip檔案都有唯一的檔案名稱，例如：

9789_05_05_2011_61703.zip

此範例中的檔案名稱提供下列資訊：

* 9789是您的[!DNL Workfront Proof]帳戶識別碼
* 05_05_2011是建立日期（2011年5月5日）
* 61703是隨機系統指派的數字

此命名慣例可讓您輕鬆將所有備份.zip檔案儲存在電腦上的單一位置，並讓您知道每個備份的確切建立時間。

[!UICONTROL Backup]函式可讓您決定如何使用資源：

* 可讓您釋放儲存空間，而不會失去作用中或封存的校樣。 您可以要求備份、刪除校樣，然後清空[還原並清空 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)中的垃圾桶。
* 可讓您存取您最初上傳至[!DNL Workfront]校訂的任何檔案。 刪除校樣之前，您可以使用[!UICONTROL 下載原始檔案]功能來下載它們。

>[!NOTE]
>
>使用備份時，請考量下列事項：
>
>* Enterprise和Unlimited計畫提供備份。 請連絡我們的[銷售團隊](mailto:sales@proofhq.com)以取得報價。
>* 資料編碼型別預設會設為UTF-8，我們建議使用此設定。 這是網際網路應用程式最常使用的編碼型別。
>* 您一次只能要求一個[!DNL backup]。 處理您的備份.zip檔案時，將不會顯示[備份]索引標籤上的[請求新備份]連結，而且顯示的訊息保持不變。 如需要求備份的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md)中要求新的資料備份。
>



## 備份您的資料

1. 按一下[!DNL Workfront Proof]介面右上角的&#x200B;**[!UICONTROL 帳戶設定]**。 (1)
1. 按一下「**[!UICONTROL 備份]**」標籤。 (2)
1. 按一下&#x200B;**[!UICONTROL 要求新備份]**&#x200B;連結(3)

當備份準備就緒時，會發生下列情況：

* 您收到來自[!DNL Workfront Proof]的電子郵件，通知您此問題（「您的[!DNL Workfront Proof]備份已就緒」）。 此電子郵件包含您備份資料的下載連結。
* [帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)備份索引標籤會顯示您備份資料的下載連結。
* Request new backup連結(3)會重新出現在Backups標籤上

您的資料將可以下載為zip檔案。 您可以從通知電子郵件或[!UICONTROL 帳戶設定]下載備份.zip檔案，如下列章節所述：

* [從電子郵件通知下載您的備份.zip檔案](#downloading-your-backup-zip-file-from-your-email-notification)
* [從帳戶設定下載您的備份.zip檔案](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## 從電子郵件通知下載您的備份.zip檔案 {#downloading-your-backup-zip-file-from-your-email-notification}

當您的備份.zip檔案準備下載時，您會收到來自[!DNL Workfront Proof]的電子郵件，主旨列為「您的[!DNL Workfront Proof]備份準備就緒」。

若要從電子郵件下載備份.zip檔案：

1. 按一下電子郵件中的下載連結。\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   如果您目前未登入[!DNL Workfront Proof]，則會開啟新的瀏覽器視窗並顯示登入頁面。

## 從帳戶設定下載您的備份.zip檔案 {#downloading-your-backup-zip-file-from-the-account-settings}

當您的備份.zip檔案準備下載時，[!UICONTROL 備份]索引標籤會顯示下載連結來指示此動作。 此外，[!UICONTROL 要求新備份]連結會再次出現。

1. 按一下[!DNL Workfront Proof]介面右上角的&#x200B;**[!UICONTROL 帳戶設定]**。 (1)
1. 按一下「**[!UICONTROL 備份]**」標籤。 (2)\
   如果您的帳戶中沒有使用者要求任何備份，則[!UICONTROL 備份]索引標籤會指出您沒有備份。 如果使用者已請求備份，索引標籤會顯示上次備份的建立日期和下載連結。

1. 按一下&#x200B;**[!UICONTROL 下載備份]**&#x200B;連結。 (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png)出現「檔案下載」畫面，詢問您是否要開啟或儲存下載檔案。

1. 按一下&#x200B;**[!UICONTROL 儲存]**，然後在您的電腦上選取要儲存備份.zip檔案的位置。\
   識別您最近備份日期的訊息會一直顯示在[!UICONTROL 備份]頁面的底部，直到您下次要求備份為止。 下載備份連結會套用至上次的備份。 每當顯示[!UICONTROL 要求新備份]連結時，您可以按一下該連結來要求另一個備份。

## 瞭解備份.zip檔案中的檔案

您的備份.zip檔案包含七個CSV （逗號分隔值或逗號分隔）檔案，其中包含您的活動和封存校樣直到資料備份時的資訊：

* comments.csv — 包含校訂的評論
* comment_replies.csv — 包含校樣organization.csv的回應 — 包含數值識別碼和您的組織名稱（您的帳戶）
* contacts.csv — 包含每個連絡人的數值識別碼、姓名和組織
* files.csv — 包含來自[校訂詳細資訊]頁面或上傳到[!DNL Workfront Proof]之校訂或檔案的[檔案詳細資訊]頁面的資訊
* recipients.csv — 包含在[!DNL Workfront Proof]上傳校樣以供檢閱時，指定為檢閱者、檢閱者和核准者等之每個人的數值識別碼、角色和決定
* users.csv — 包含數值識別碼和帳戶中所有使用者的名稱

您可以使用任何使用的zip公用程式，從備份.zip檔案中解壓縮這些檔案，然後將它們儲存在電腦上您所選擇的位置。 儲存zip檔案並解壓縮個別CSV檔案後，您可以視需要操作資訊以保留內部記錄。

您要求建立的每個備份.zip檔案都有專屬名稱，其中包含備份建立日期，但每個備份.zip檔案中包含的CSV檔案名稱一律相同。 您可能會想使用下列其中一個方法，來確保備份檔案彼此不同：

* 為每個備份.zip檔案以及您從中解壓縮的CSV檔案建立一個新資料夾。
* 重新命名每個個別CSV檔案，以便在您從zip檔案解壓縮時包含備份日期。

>[!NOTE]
>
>如果您的電腦上已安裝[!DNL Microsoft Excel]，則擷取公用程式可能會將個別CSV檔案的檔案型別列為[!DNL Microsoft Office Excel]個逗號分隔值檔案。 您可以使用[!DNL Excel]開啟擷取的CSV檔案，並將檔案儲存為[!DNL Excel]活頁簿(&#42;.xlsx)或其他檔案型別。
