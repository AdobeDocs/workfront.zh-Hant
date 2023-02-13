---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: 使用適用於Illustrator的Workfront擴充功能和InDesign
description: 您可以使用Workfront擴充功能，將您在Adobe Illustrator和Adobe InDesign中儲存及建立的數位內容匯出至Workfront。 這可加快檔案審核和核准程式。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# 使用適用於Illustrator的Workfront擴充功能和InDesign

>[!IMPORTANT]
>
>我們將以取代Workfront的Illustrator和InDesign擴充功能 [更新Creative Cloud外掛程式](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). 自2022年底起，我們將不再支援此擴充功能，並依現狀提供。


您可以使用Workfront擴充功能，將您在Adobe Illustrator和Adobe InDesign中儲存及建立的數位內容匯出至Workfront。 這可加快檔案審核和核准程式。

Adobe Creative Cloud 2017及更新版本支援Workfront擴充功能，適用於下列應用程式：

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >建議使用 [Adobe Workfront for Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) 外掛程式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>除了Adobe Creative Cloud授權，您還必須擁有Workfront授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>編輯您要與之互動之物件的存取權。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從Illustrator登入Workfront擴充功能或InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

當您從其中一個支援的Adobe應用程式登入Workfront時，就會登入所有支援的Adobe應用程式。

1. 前往您要使用Workfront擴充功能的Adobe應用程式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的導出檔案格式](#supported-exported-file-formats) 這篇文章。

1. 按一下 **視窗** > **擴充功能** > Workfront。

1. （可選）將Workfront面板拖曳至您要其顯示在Adobe應用程式中的位置。
1. 依照提示登入Workfront。

   >[!NOTE]
   >
   >* Workfront使用OAuth 2.0連線至Adobe Creative Cloud，此為大多數網頁型整合用於驗證和授權使用者的安全標準。
   >* 系統提示您輸入 [域或主機] Workfront帳戶的，請使用此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。


   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

## 上傳檔案至Workfront專案、工作或問題 {#upload-a-file-to-a-workfront-project-task-or-issue}

您可以從電腦檔案系統上傳檔案，或將目前在Adobe Creative Cloud應用程式中開啟的檔案匯出至Workfront專案、工作或問題。 

從Adobe Creative Cloud上傳或匯出檔案時，請考量下列事項：

* 您的存取層級必須允許將檔案上傳至Workfront。 如需詳細資訊，請參閱 [授予對文檔的訪問權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* 您必須擁有將文檔上載到所需項目的權限。 如需詳細資訊，請參閱 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* 檔案會上傳至您選取之Workfront物件的「檔案」區域。
* 無法將文檔導出到主菜單中的「文檔」區域 ![](assets/main-menu-icon.png) 來自Adobe Creative Cloud應用程式。

本節將說明以下內容：

* [上傳檔案](#upload-a-file)
* [匯出目前在Illustrator或InDesign中開啟的檔案](#export-a-file-currently-open-in-illustrator-or-indesign)
* [從Illustrator或InDesign上傳新版本的檔案](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### 上傳檔案 {#upload-a-file}

您不必離開Adobe Creative Cloud應用程式，即可將檔案上傳至專案、工作或問題。

1. 如果您在開啟Workfront應用程式時未看到Adobe Creative Cloud擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 按一下您要上傳檔案的專案、任務或問題名稱。

   您可以在 **搜尋** 框和選擇 **專案**, **任務**，或 **問題** 從 **搜尋** 框。 如果工作項目名稱未出現在清單中，請按 **輸入** 搜尋您有權檢視的所有Workfront項目。

1. 按一下 **選擇**&#x200B;在Workfront延伸功能的右下角。
1. 在 **按一下以選取格式** 下拉式選單中，按一下您要將檔案儲存在Workfront中的格式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的導出檔案格式](#supported-exported-file-formats) 這篇文章。

1. （條件性）如果要上載檔案的工作項包含文檔資料夾，請在&#x200B;**按一下以選擇文檔資料夾** 欄位，然後按一下 **選擇**.

1. 按一下 **上傳本機檔案**.
1. 在 **開啟檔案** 框中，在檔案系統中查找檔案，然後按一下 **開啟**.

1. （選用）為檔案輸入新名稱。 

   ![](assets/rename-file-uploading.png)

1. 按一下 **上傳**.

   在Workfront中，該文檔現在會列在您指定的項目、任務或問題的「文檔」區域中。  

1. （可選）按一下檔案的名稱，以開啟Workfront中的「檔案詳細資料」頁面。

   Workfront會在新瀏覽器標籤中開啟。

### 匯出目前在Illustrator或InDesign中開啟的檔案 {#export-a-file-currently-open-in-illustrator-or-indesign}

1. 在支援的Adobe Creative Cloud應用程式中，開啟您要匯出至Workfront的檔案。 
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 按一下要導出檔案的項目、任務或問題的名稱。

   您可以在 **搜尋** 框和選擇 **專案**, **任務**，或 **問題** 從 **搜尋** 框。 如果工作項目名稱未出現在清單中，請按 **輸入** 搜尋您有權檢視的所有Workfront項目。

1. 在 **按一下以選取格式** 下拉式選單中，按一下您要將檔案儲存在Workfront中的格式。

   如需每個支援應用程式的支援格式清單，請參閱 [支援的導出檔案格式](#supported-exported-file-formats) 這篇文章。

1. （條件性）如果要上載檔案的工作項包含文檔資料夾，請在&#x200B;**按一下以選擇文檔資料夾** 欄位，然後按一下 **選擇**.
1. （可選）要更名文檔，請按一下文檔名稱並鍵入新名稱。

   ![](assets/rename-doc-exporting.png)

1. 按一下 **匯出**. 

   系統會顯示訊息，確認檔案已成功匯出至Workfront。

   在Workfront中，文檔會列在您在Workfront中指定對象的「文檔」區域中。

1. （選用）按一下檔案名稱，即可在Workfront中存取。

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront會在新瀏覽器標籤中開啟。

### 從Illustrator或InDesign上傳新版本的檔案 {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. 如果要將在支援的Adobe應用程式中處理的檔案導出為Workfront中的新版本檔案，請在Adobe應用程式中開啟該檔案。 
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 按一下列出現有文檔的項目、任務或問題的名稱。

   您可以在 **搜尋** 框和選擇 **專案**, **任務**，或 **問題** 從 **搜尋** 框。 如果工作項目名稱未出現在清單中，請按 **輸入** 搜尋您有權檢視的所有Workfront項目。

   上傳至專案、工作或問題的所有檔案都會顯示在清單中，無論這些檔案是否從Adobe應用程式上傳。

1.  
1. 在 **按一下以選取格式** 下拉式選單中，按一下您要將檔案儲存在Workfront中的格式。

   如果要匯出已在Adobe應用程式中開啟的檔案，則此為必要項目。 如需每個支援應用程式的支援格式清單，請參閱 [支援的導出檔案格式](#supported-exported-file-formats) 這篇文章。

1. 如果要導出在Adobe應用程式中開啟的檔案作為所選Workfront文檔的新版本，請按一下 **匯出**.

   或

   如果要從電腦檔案系統上傳檔案，作為您選取的新版Workfront檔案，請按一下 **上傳本機檔案**，在出現的方塊中尋找檔案，按一下 **開啟**，然後按一下 **上傳**.

1. （選用）按一下檔案的名稱，即可在Workfront中查看其新版本。 

   >[!NOTE]
   >
   >預設會填入Workfront中的檔案名稱，且無法編輯。 也不會變更您上傳或匯出為新版本的檔案名稱。
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## 對來自Illustrator或InDesign的Workfront檔案的註解 {#comment-on-a-workfront-document-from-illustrator-or-indesign}

您可以直接在Adobe應用程式中將注釋新增至Workfront檔案。 在Workfront中，您的備注會顯示在文檔的「更新」區域和保存文檔的Workfront項的「更新」區域。 

1. 開啟支援的其中一個Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 按一下列出現有文檔的項目、任務或問題。

   您可以在 **搜尋** 框和選擇 **專案**, **任務**，或 **問題** 從 **搜尋** 框。 如果工作項目名稱未出現在清單中，請按 **輸入** 搜尋您有權檢視的所有Workfront項目。

1. 按一下現有文檔的名稱，然後按一下 **選擇**&#x200B;在Workfront延伸功能的右下角。
1. 按一下 **註解** ，然後在顯示的框中鍵入更新。

1. （可選）若要將其他Workfront使用者或團隊納入註解，請開始在 **通知人員或團隊** 框中，然後在名稱出現在下拉清單中時按一下該名稱。
1. （可選）要請求文檔批准，請選擇 **提出核准請求**.
1. 按一下 **更新**.

   更新會發佈在文檔的「更新」頁簽中。 您加入備注的Workfront使用者會收到應用程式內通知，而且，視Workfront的設定方式而定，也可能會收到電子郵件通知。

   如需Workfront中通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   如需接收電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 向Illustrator或InDesign申請檔案核准

您可以直接向Workfront應用程式請求Adobe檔案核准。

您可以向以下實體請求文檔批准：

* Workfront使用者
* 沒有Workfront帳戶的外部使用者

您可以通過以下方式向Adobe應用程式請求文檔的批准：

* 將批准者附加至檔案。
* 在文檔上加上注釋，在您發表評論時通知該人。 並將他們作為批准者附加到文檔。

   有關在對文檔進行注釋時請求批准的資訊，請參閱 [對來自Illustrator或InDesign的Workfront檔案的註解](#comment-on-a-workfront-document-from-illustrator-or-indesign) 這篇文章。

要向Adobe應用程式請求文檔批准，請執行以下操作：

1. 開啟支援的其中一個Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 按一下列出現有文檔的項目、任務或問題，然後按一下現有文檔的名稱。

   您可以在 **搜尋** 框和選擇 **專案**, **任務**，或 **問題** 從 **搜尋** 框。 如果工作項目名稱未出現在清單中，請按 **輸入** 搜尋您有權檢視的所有Workfront項目。

1. 按一下現有文檔的名稱，然後按一下 **選擇**&#x200B;在Workfront延伸功能的右下角。
1. 按一下 **核准** 標籤。
1. 若要新增核准者，請在 **開始鍵入名稱框** 執行下列其中一項操作：

   * 輸入核准者的名稱，然後在核准者顯示在清單中時加以選取。

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * 輸入外部使用者的電子郵件地址。

1. 按一下 **請求核准**.

   您加入註解或新增為核准者的Workfront使用者會收到應用程式內通知，而且，視Workfront的設定方式而定，也可能會收到電子郵件通知。\
   外部使用者會收到電子郵件通知，通知可在此決定核准。

   如需Workfront中通知的相關資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 如需接收電子郵件通知的相關資訊，請參閱 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 從Illustrator或InDesign產生校樣 {#generate-a-proof-from-illustrator-or-indesign}

如果您的組織使用「自動化工作流」模板，則可以為您在Adobe應用程式中建立的文檔生成校樣，而不需要離開應用程式。 如需建立校樣的詳細資訊，請參閱 [建立校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). 如需自動化工作流程範本的相關資訊，請參閱 [自動化工作流程範本](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) in [自動化工作流程概觀](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. 開啟支援的其中一個Adobe應用程式。
1. 如果未顯示Workfront擴充功能，請按一下 **視窗** > **擴充功能** > Workfront。

   如果項目為當前狀態，則會顯示分配給您的工作項清單。 如果清單未顯示，請登入Workfront。

   個人任務列於 **無項目**.

1. 如果檔案已上傳至Workfront，請在列出檔案的Workfront擴充功能中選取專案、任務或問題，然後按一下檔案的名稱。

   或

   將Adobe檔案上傳至Workfront物件，如 [上傳檔案至Workfront專案、工作或問題](#upload-a-file-to-a-workfront-project-task-or-issue) 在本文中，然後按一下檔案的名稱。

1. 在 **按一下以選取格式** 下拉式選單中，按一下您要將檔案儲存在Workfront中的格式。

   在執行此測試後的步驟中啟用校對功能後，某些格式將無法使用。 如需詳細資訊，請參閱 [支援的導出檔案格式](#supported-exported-file-formats) 這篇文章。

1. 按一下 **以新校樣上傳** 來啟用。
1. 選取 **工作流程範本** 您希望人們在審閱文檔時使用。

   您的Workfront管理員會設定自動化工作流程範本，如所述。 如有疑問，請洽詢管理員。

   1. 至少添加一個 **新收件者** 到「工作流模板」中的每個階段。

      您可以開始輸入名稱，然後在出現的下拉式清單中看到名稱時加以選取。

   1. 指定 **證明角色** 和頻率 **電子郵件警報** 為您新增的每個收件者。

   1. （選用）在 **電子郵件通知** 區段中，選取是否要傳送包含關於校樣的選用自訂訊息的電子郵件通知給您新增的所有校樣收件者。

1. 按一下 **建立校樣**.

   您可以檢視校樣建立程式的進度。 警報完成生成後，將顯示該警報。 您可以開啟建立校樣並列在其中的任務。

## 上傳新版本的校樣，而不需離開Illustrator或InDesign

1. 按一下具有校樣的現有文檔，然後按一下 **選擇** 在右下角。
1. 按一下 **以新校樣版本上傳** 來啟用。
1. （選用）選取 **工作流程範本** 您希望使用者在檢閱新版本時使用。

   如果您未選取其他範本，則為舊版選取的範本仍會生效。 此外，如果您修改了早期版本的模板，則更改對新版本有效。

   您的Workfront管理員會設定自動化工作流程範本，如所述。 如有疑問，請洽詢管理員。

   1. 至少添加一個 **新收件者** 到「工作流模板」中的每個階段。

      您可以開始輸入名稱，然後在出現的下拉式清單中看到名稱時加以選取。

   1. 指定 **證明角色** 和頻率 **電子郵件警報** 為您新增的每個收件者。
   1. （選用）在 **電子郵件通知** 區段中，選取是否要傳送包含關於校樣的選用自訂訊息的電子郵件通知給您新增的所有校樣收件者。

1. 按一下 **建立新校樣版本**.

   您可以檢視校樣建立程式的進度。 警報完成生成後，將顯示該警報。 您可以開啟建立校樣並列在其中的任務。

## 登出Workfront擴充功能

1. 在Adobe應用程式中，按一下 **視窗** > **擴充功能** > Workfront。

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在面板的右上角。

1. （選用）按一下 **意見反應** 開啟簡短的調查，並傳送Workfront您對Workfront for Adobe Creative Cloud的意見。 
1. 按一下 **登出**.\
   「登入」畫面隨即顯示。 如需登入的詳細資訊，請參閱 [從Illustrator登入Workfront擴充功能或InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) 這篇文章。

## 支援的導出檔案格式 {#supported-exported-file-formats}

* [支援的Adobe InDesign匯出檔案格式](#supported-exported-file-formats-for-adobe-indesign)
* [支援的Adobe Illustrator匯出檔案格式](#supported-exported-file-formats-for-adobe-illustrator)

### 支援的Adobe InDesign匯出檔案格式  {#supported-exported-file-formats-for-adobe-indesign}

Workfront支援下列檔案格式，可將檔案從InDesign匯出至Workfront:

* EPS — 封裝的PostScript
* ePub — 固定版面電子出版物
* ePub — 可重排的電子出版物 &#42;
* HTML- HyperText標籤語言
* IDML -InDesign標籤語言 &#42;
* JPG,JPEG — 聯合攝影專家組
* PDF-Adobe可移植文檔檔案
* PNG — 可移植網路圖形
* SWF-Flash Player &#42;
* XML — 可擴展標籤語言 &#42;

&#42; 此檔案格式在 **上傳新校樣** 已啟用(如需此選項的詳細資訊，請參閱 [從Illustrator或InDesign產生校樣](#generate-a-proof-from-illustrator-or-indesign) )。 如果在啟用前已選擇此檔案格式 **上傳新校樣**，系統會將檔案格式變更為PDF。 您可以從清單中選取不同格式。

### 支援的Adobe Illustrator匯出檔案格式  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront支援下列檔案格式，可將檔案從Illustrator匯出至Workfront:

* DWG - AutoCAD繪圖、AutoCAD交換檔案 &#42;
* JPG,JPEG — 聯合攝影專家組
* PNG — 可移植網路圖形
* PSD- Photoshop檔案
* SWF-Flash Player &#42;
* TIFF — 標籤的影像檔案格式

&#42; 此檔案格式在 **上傳新校樣** 已啟用(如需此選項的詳細資訊，請參閱 [從Illustrator或InDesign產生校樣](#generate-a-proof-from-illustrator-or-indesign) )。 如果在啟用前已選擇此檔案格式 **上傳新校樣**，系統會將檔案格式變更為PNG。 您可以從清單中選取不同格式。
