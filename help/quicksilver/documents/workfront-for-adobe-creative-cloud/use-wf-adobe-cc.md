---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: 使用適用於Illustrator和InDesign的Workfront擴充功能
description: 您可以使用Workfront擴充功能，將您在Adobe Illustrator和Adobe InDesign中儲存和建立的數位內容匯出至Workfront。 這能加快檔案稽核和核准流程。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '3076'
ht-degree: 0%

---

# 使用適用於Illustrator和InDesign的Workfront擴充功能

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>我們正在將適用於Illustrator的Workfront擴充功能取代為，並將InDesign替換為 [已更新Creative Cloud外掛程式](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). 自2022年底開始，將不再支援此擴充功能，並依現狀提供。

您可以使用Workfront擴充功能，將您在Adobe Illustrator和Adobe InDesign中儲存和建立的數位內容匯出至Workfront。 這能加快檔案稽核和核准流程。

下列應用程式支援Workfront擴充功能Adobe Creative Cloud 2017和更新版本：

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >我們建議使用新的 [適用於Photoshop的Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) 外掛程式。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前：Pro或更高</p>
   或
   <p>新增：任何計畫</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前：工作或以上</p>
   或
   <p>新增：標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>除了Adobe Creative Cloud授權，您還必須擁有Workfront授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯您想要與其互動之物件的存取權。</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 從Illustrator或InDesign登入Workfront擴充功能 {#log-in-to-workfront-extension-from-illustrator-or-indesign}

當您從其中一個支援的Adobe應用程式登入Workfront時，您會登入所有支援的Adobe應用程式。

1. 前往您要使用Workfront擴充功能的Adobe應用程式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的匯出檔案格式](#supported-exported-file-formats) 本文章內容。

1. 按一下 **視窗** > **擴充功能** >Workfront。

1. （可選）將Workfront面板拖曳至您要其在Adobe應用程式中顯示的位置。
1. 依照提示登入Workfront。

   >[!NOTE]
   >
   >* Workfront使用OAuth 2.0連線至Adobe Creative Cloud，這是大部分網頁型整合所使用的安全標準，用於驗證及授權使用者。
   >* 當系統提示您輸入 [網域或主機] 的，請以此格式輸入Workfront帳戶：`yourCompany'sDomain.my.workfront.com`. 您公司的網域通常是您公司的名稱。

   如果專案為目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

## 將檔案上傳至Workfront專案、任務或問題 {#upload-a-file-to-a-workfront-project-task-or-issue}

您可以從您的電腦檔案系統上傳檔案，或將目前在Adobe Creative Cloud應用程式中開啟的檔案匯出至Workfront專案、任務或問題。 

從Adobe Creative Cloud上傳或匯出檔案時，請考量下列事項：

* 您的存取層級必須允許將檔案上傳至Workfront。 如需詳細資訊，請參閱 [授與檔案的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* 您必須有許可權將檔案上傳至您想要的專案。 如需詳細資訊，請參閱 [物件許可權共用概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* 檔案會針對您選取的Workfront物件上傳至檔案區域。
* 您無法將檔案匯出至主功能表中的[檔案]區域 ![](assets/main-menu-icon.png) 來自Adobe Creative Cloud應用程式。

以下章節說明下列內容：

* [上傳檔案](#upload-a-file)
* [匯出目前在Illustrator或InDesign中開啟的檔案](#export-a-file-currently-open-in-illustrator-or-indesign)
* [從Illustrator或InDesign上傳檔案的新版本](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### 上傳檔案 {#upload-a-file}

您可以上傳檔案至專案、任務或問題，而不需要離開Adobe Creative Cloud應用程式。

1. 如果您在開啟Workfront應用程式時沒有看到Adobe Creative Cloud擴充功能，請按一下 **視窗** > **擴充功能** > **Workfront**.

   如果專案處於目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 按一下您要上傳檔案的專案、任務或問題的名稱。

   您可以輸入「 」中的名稱來搜尋此專案 **搜尋** 方塊並選取 **專案**， **任務**，或 **問題** 從下拉式功能表右側 **搜尋** 方塊。 如果工作專案的名稱未出現在清單中，請按 **輸入** 以搜尋您有權檢視的所有Workfront專案。

1. 按一下 **選取** 在Workfront擴充功能的右下角。
1. 在 **按一下以選取格式** 下拉式功能表，按一下您要在Workfront中儲存檔案的格式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的匯出檔案格式](#supported-exported-file-formats) 本文章內容。

1. （視條件而定）如果要上傳檔案的工作專案具有檔案資料夾，請在 **按一下以選取檔案資料夾** 欄位，然後按一下 **選取**.

1. 按一下 **上傳本機檔案**.
1. 在 **開啟檔案** 方塊中，在您的檔案系統中尋找檔案，然後按一下 **開啟**.

1. （選擇性）為檔案輸入新名稱。

   ![](assets/rename-file-uploading.png)

1. 按一下 **上傳**.

   在Workfront中，該檔案現在會列在您所選專案、任務或問題的檔案區域中。

1. （選用）按一下檔名稱，在Workfront中開啟其「檔案詳細資訊」頁面。

   Workfront會在新的瀏覽器標籤中開啟。

### 匯出目前在Illustrator或InDesign中開啟的檔案 {#export-a-file-currently-open-in-illustrator-or-indesign}

1. 在支援的Adobe Creative Cloud應用程式中，開啟您要匯出至Workfront的檔案。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > **Workfront**.

   如果專案處於目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 按一下您要匯出檔案的專案、任務或問題的名稱。

   您可以輸入「 」中的名稱來搜尋此專案 **搜尋** 方塊並選取 **專案**， **任務**，或 **問題** 從下拉式功能表右側 **搜尋** 方塊。 如果工作專案的名稱未出現在清單中，請按 **輸入** 以搜尋您有權檢視的所有Workfront專案。

1. 在 **按一下以選取格式** 下拉式功能表，按一下您要在Workfront中儲存檔案的格式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的匯出檔案格式](#supported-exported-file-formats) 本文章內容。

1. （視條件而定）如果要上傳檔案的工作專案具有檔案資料夾，請在&#x200B;**按一下以選取檔案資料夾** 欄位，然後按一下 **選取**.
1. （選擇性）若要重新命名檔案，請按一下檔名稱並鍵入新名稱。

   ![](assets/rename-doc-exporting.png)

1. 按一下 **匯出**.

   系統會顯示訊息，確認檔案已成功匯出至Workfront。

   在Workfront中，檔案會列在您於Workfront中指定的物件的「檔案」區域中。

1. （選用）按一下檔名稱，即可在Workfront中存取。

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront會在新的瀏覽器標籤中開啟。

### 從Illustrator或InDesign上傳檔案的新版本 {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. 如果您想要將在受支援的Adobe應用程式中處理的檔案匯出為Workfront中檔案的新版本，請在Adobe應用程式中開啟該檔案。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > **Workfront**.

   如果專案為目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 按一下列出現有檔案的專案、任務或問題的名稱。

   您可以輸入「 」中的名稱來搜尋此專案 **搜尋** 方塊並選取 **專案**， **任務**，或 **問題** 從下拉式功能表右側 **搜尋** 方塊。 如果工作專案的名稱未出現在清單中，請按 **輸入** 以搜尋您有權檢視的所有Workfront專案。

   上傳到專案、任務或問題的所有檔案都會顯示在清單中，無論這些檔案是否從Adobe應用程式上傳。

1. 在 **按一下以選取格式** 下拉式功能表，按一下您要在Workfront中儲存檔案的格式。

   如果要匯出已在Adobe應用程式中開啟的檔案，則需要此專案。 如需每個支援應用程式的支援格式清單，請參閱 [支援的匯出檔案格式](#supported-exported-file-formats) 本文章內容。

1. 如果要將已在Adobe應用程式中開啟的檔案匯出為您所選Workfront檔案的新版本，請按一下 **匯出**.

   或

   如果您想從電腦檔案系統上傳檔案，作為所選Workfront檔案的新版本，請按一下 **上傳本機檔案**，在出現的方塊中尋找檔案，按一下 **開啟**，然後按一下 **上傳**.

1. （選用）按一下檔名稱，在Workfront中檢視其新版本。

   >[!NOTE]
   >
   >Workfront中的檔名稱預設會填入，且無法編輯。 它也不會變更您上傳或匯出為新版本的檔案的名稱。
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## 在Illustrator或InDesign的Workfront檔案上加上註解 {#comment-on-a-workfront-document-from-illustrator-or-indesign}

您可以在Adobe應用程式內直接將註解新增至Workfront檔案。 在Workfront中，您的註解會顯示在檔案的「更新」區域中，以及儲存檔案的Workfront專案的「更新」區域中。

1. 開啟其中一個支援的Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > **Workfront**.

   如果專案為目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 按一下列出現有檔案的專案、任務或問題。

   您可以輸入「 」中的名稱來搜尋此專案 **搜尋** 方塊並選取 **專案**， **任務**，或 **問題** 從下拉式功能表右側 **搜尋** 方塊。 如果工作專案的名稱未出現在清單中，請按 **輸入** 以搜尋您有權檢視的所有Workfront專案。

1. 按一下現有檔案的名稱，然後按一下 **選取** 在Workfront擴充功能的右下角。
1. 按一下 **註解** 標籤，然後在方塊中輸入您的更新。

1. （可選）若要在評論中加入其他Workfront使用者或團隊，請在 **通知人員或團隊** 方塊，然後按一下該名稱（當它出現在下拉式清單中時）。
1. （選擇性）若要請求核准檔案，請選取 **提出核准請求**.
1. 按一下 **更新**.

   更新已發佈在檔案的更新索引標籤中。 您加入評論中的Workfront使用者會收到應用程式內通知，且根據Workfront的設定方式，也可能會收到電子郵件通知。

   如需Workfront中通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

   如需接收電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 向Illustrator或InDesign請求檔案核准

您可以直接從Adobe應用程式要求Workfront檔案核准。

您可以向下列實體請求檔案核准：

* Workfront使用者
* 沒有Workfront帳戶的外部使用者

您可以透過下列方式，從Adobe應用程式請求檔案核准：

* 將核准者附加至檔案。
* 在檔案上加上註解，在註解時通知使用者，並以核准者身分將其附加至檔案。

  如需在檔案註解時請求核准的相關資訊，請參閱區段 [在Illustrator或InDesign的Workfront檔案上加上註解](#comment-on-a-workfront-document-from-illustrator-or-indesign) 本文章內容。

若要從Adobe應用模組請求檔案的核准，請執行下列步驟：

1. 開啟其中一個支援的Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > **Workfront**.

   如果專案為目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 按一下列出現有檔案的專案、任務或問題，然後按一下現有檔案的名稱。

   您可以輸入「 」中的名稱來搜尋此專案 **搜尋** 方塊並選取 **專案**， **任務**，或 **問題** 從下拉式功能表右側 **搜尋** 方塊。 如果工作專案的名稱未出現在清單中，請按 **輸入** 以搜尋您有權檢視的所有Workfront專案。

1. 按一下現有檔案的名稱，然後按一下 **選取**&#x200B;在Workfront擴充功能的右下角。
1. 按一下 **核准** 標籤。
1. 若要新增核准者，請在 **開始輸入名稱方塊** 執行下列任一項作業：

   * 輸入核准者的名稱，然後在清單中顯示時選取該名稱。

     ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * 輸入外部使用者的電子郵件地址。

1. 按一下 **要求核准**.

   您加入評論或新增為核准者的Workfront使用者會收到應用程式內通知，且根據Workfront的設定方式，也可能會收到電子郵件通知。\
   外部使用者會收到電子郵件通知，以便決定核准。

   如需Workfront中通知的相關資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 如需有關接收電子郵件通知的資訊，請參閱 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 從Illustrator或InDesign產生校訂 {#generate-a-proof-from-illustrator-or-indesign}

如果您的組織使用自動化工作流程範本，您無需離開應用程式，即可為您在Adobe應用程式中建立的檔案產生校訂。 如需關於建立校訂的資訊，請參閱 [建立校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md). 如需有關自動化工作流程範本的資訊，請參閱 [自動化工作流程範本](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) 在 [自動化工作流程總覽](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. 開啟其中一個支援的Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** >Workfront。

   如果專案為目前狀態，則會顯示指派給您的工作專案清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無專案**.

1. 如果檔案已上傳至Workfront，請在Workfront擴充功能中選取列出該檔案的專案、任務或問題，然後按一下檔案的名稱。

   或

   將Adobe檔案上傳至Workfront物件，如一節所述 [將檔案上傳至Workfront專案、任務或問題](#upload-a-file-to-a-workfront-project-task-or-issue) 然後，在本文章中按一下檔案的名稱。

1. 在 **按一下以選取格式** 下拉式功能表，按一下您要在Workfront中儲存檔案的格式。

   在此格式之後的步驟中啟用校訂功能後，部分格式就無法使用。 如需詳細資訊，請參閱 [支援的匯出檔案格式](#supported-exported-file-formats) 本文章內容。

1. 按一下 **上傳為新校訂** 以啟用它。
1. 選取 **工作流程範本** 您希望人們在檢閱檔案時使用。

   您的Workfront管理員會設定自動化工作流程範本，如所述 [建立及管理自動化工作流程範本](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). 如有疑問，請洽詢管理員。

   1. 至少新增一個 **新收件者** 至工作流程範本中的每個階段。

      您可以開始輸入名稱，然後在出現的下拉式清單中看到該名稱時將其選取。

   1. 指定 **校訂角色** 和頻率 **電子郵件警示** 您新增的每個收件者。

   1. （選用）在 **電子郵件通知** 區段，選取是否將包含有關校訂的可選自訂訊息的電子郵件通知傳送給您新增的所有校訂收件者。

1. 按一下 **建立校訂**.

   您可以檢視校樣建立流程的進度。 警報產生完成後便會顯示。 您可以開啟您建立校樣的工作，它便列於此處。

## 在不離開Illustrator或InDesign的情況下上傳新版本的校訂

1. 按一下有校訂的現有檔案，然後按一下 **選取** 在右下角。
1. 按一下 **上傳為新校訂版本** 以啟用它。
1. （可選）選取 **工作流程範本** 您希望使用者在檢閱新版本時使用。

   如果您未選取其他範本，則為舊版選取的範本將維持有效。 此外，如果您已修改舊版的範本，則新版本的變更會生效。

   您的Workfront管理員會設定自動化工作流程範本，如所述 [建立及管理自動化工作流程範本](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). 如有疑問，請洽詢管理員。

   1. 至少新增一個 **新收件者** 至工作流程範本中的每個階段。

      您可以開始輸入名稱，然後在出現的下拉式清單中看到該名稱時將其選取。

   1. 指定 **校訂角色** 和頻率 **電子郵件警示** 您新增的每個收件者。
   1. （選用）在 **電子郵件通知** 區段，選取是否將包含有關校訂的可選自訂訊息的電子郵件通知傳送給您新增的所有校訂收件者。

1. 按一下 **建立新校訂版本**.

   您可以檢視校樣建立流程的進度。 警報產生完成後便會顯示。 您可以開啟您建立校樣的工作，它便列於此處。

## 登出Workfront擴充功能

1. 在Adobe應用程式中，按一下 **視窗** > **擴充功能** > **Workfront**.

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在面板的右上角。

1. （選用）按一下 **意見反應** 開啟簡短問卷調查，並將您對於Adobe Creative CloudWorkfront的意見反應傳送給Workfront。
1. 按一下 **登出**.\
   「登入」畫面隨即顯示。 如需有關登入的資訊，請參閱 [從Illustrator或InDesign登入Workfront擴充功能](#log-in-to-workfront-extension-from-illustrator-or-indesign) 本文章內容。

## 支援的匯出檔案格式 {#supported-exported-file-formats}

* [Adobe InDesign支援的匯出檔案格式](#supported-exported-file-formats-for-adobe-indesign)
* [Adobe Illustrator支援的匯出檔案格式](#supported-exported-file-formats-for-adobe-illustrator)

### Adobe InDesign支援的匯出檔案格式  {#supported-exported-file-formats-for-adobe-indesign}

Workfront支援以下檔案格式，可將檔案從InDesign匯出至Workfront：

* EPS — 封裝式PostScript
* ePub — 固定版面電子出版物
* ePub — 可重新整理的電子出版物 &#42;
* HTML- HyperText標籤語言
* IDML -InDesign標籤語言 &#42;
* JPG、JPEG — 聯合攝影專家小組
* PDF-Adobe可攜式檔案檔案
* PNG — 可攜式網路圖形
* SWF-Flash Player &#42;
* XML — 可延伸標籤語言 &#42;

&#42; 此檔案格式在下列情況下無法使用 **上傳新校訂** 已啟用(如需此選項的相關資訊，請參閱 [從Illustrator或InDesign產生校訂](#generate-a-proof-from-illustrator-or-indesign) 本文章中)。 如果您在啟用之前已選取此檔案格式 **上傳新校訂**，系統會將檔案格式變更為PDF。 您可以從清單中選取不同的格式。

### Adobe Illustrator支援的匯出檔案格式  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront支援下列檔案格式，可將檔案從Illustrator匯出至Workfront：

* DWG - AutoCAD工程圖、AutoCAD交換檔案 &#42;
* JPG、JPEG — 聯合攝影專家小組
* PNG — 可攜式網路圖形
* PSD- Photoshop檔案
* SWF-Flash Player &#42;
* TIFF — 標籤影像檔案格式

&#42; 此檔案格式在下列情況下無法使用 **上傳新校訂** 已啟用(如需此選項的相關資訊，請參閱 [從Illustrator或InDesign產生校訂](#generate-a-proof-from-illustrator-or-indesign) 本文章中)。 如果您在啟用之前已選取此檔案格式 **上傳新校訂**，系統會將檔案格式變更為PNG。 您可以從清單中選取不同的格式。
