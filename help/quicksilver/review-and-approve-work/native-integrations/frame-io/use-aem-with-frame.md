---
product-area: documents
navigation-topic: approvals
title: 將Adobe Experience Manager與Workfront和Adobe雲端儲存空間搭配使用
description: 將Adobe Experience Manager與Workfront和Adobe雲端儲存空間搭配使用
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 04d0f295-5206-4c5d-8003-bdf333150903
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Riv4jrZbD1vLx6eLq9utk2TIMRJh6ekBxE5ZBVc7D9c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 840211ef726bb638f75158d95f751c5833cc22bb
workflow-type: tm+mt
source-wordcount: 2166
ht-degree: 1%

---

# 將Adobe Experience Manager與Workfront和Adobe雲端儲存空間搭配使用

您可以使用&#x200B;[!DNL Experience Manager Assets]來管理和儲存&#x200B;經過檢閱和核准週期的數位資產。 此整合可讓您運用Adobe Experience Manager、Frame.io和Workfront的功能，簡化您的內容管理和共同作業程式。

## 設定Experience Manager Assets整合

您可以在&#x200B;[!DNL Experience Manager Assets]中將您的工作與您的內容連結：

* 將資產和中繼資料從[!DNL Adobe Workfront]推送到[!DNL Experience Manager Assets]&#x200B;
* 促進版本設定使用案例
* 追蹤資產的中繼資料
* 在[!DNL Workfront]和[!DNL Experience Manager Assets]之間同步專案中繼資料

>[!NOTE]
>
>您也可以將多個[!DNL Experience Manager Assets]存放庫連線至一個[!UICONTROL Workfront]環境，或將多個[!DNL Workfront]環境連線至跨組織ID的一個[!DNL Experience Manager Assets]存放庫。 針對您要設定的每項整合，請依照本文的設定指示操作。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table>
  <tr>
   <td>Adobe Workfront 封裝
   </td>
   <td> <p>Prime或Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront 授權
   </td>
   <td>
  <p>若要設定整合：</p>
   <p>標準</p>
   <p>規劃</p>

<p>若要傳送檔案至Experience Manager Assets：</p>
   <p>投稿人或以上</p>
   <p>要求或更高版本</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Adobe Experience Manager授權
   </td>
   <td>標準
   </td>
  </tr>
  <tr>
   <td>其他產品
   </td>
   <td>您必須有[!DNL Experience Manager Assets as a Cloud Service]，而且您必須以使用者的身分新增到產品中。
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，

* 您必須在[!DNL Adobe Admin Console]中將[!DNL Workfront]和[!DNL Adobe Experience Manager Assets]與組織ID相關聯。 如需詳細資訊，請參閱[平台式管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
* 您的Workfront執行個體必須使用Adobe雲端儲存空間。


## 設定整合資訊

{{step-1-to-setup}}

1. 在左側面板中選取&#x200B;**[!UICONTROL 檔案]**，然後選取&#x200B;**[!UICONTROL [!DNL Experience Manager]整合]**。
1. 選取&#x200B;**[!UICONTROL 新增[!DNL Experience Manager]整合]**。
1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中，輸入您希望使用者在Workfront和Experience Manager Assets中與此整合互動時看到的名稱。
1. 在&#x200B;**[!UICONTROL 導覽URL]**&#x200B;欄位中，系統會自動填入導覽URL。 此唯讀URL是用來從[!UICONTROL 主功能表]連結至您組織的[!DNL Experience Manager]執行個體，以進行快速存取。
1. 從&#x200B;**[!UICONTROL [!DNL Experience Manager]Assets存放庫]**&#x200B;下拉式功能表中選擇存放庫。 系統會自動填入與您的使用者設定檔所指派之組織ID相關聯的任何[!DNL Experience Manager]存放庫。
   ![選擇experience manager存放庫](assets/setup-information.png)

1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;或移至本文中的[設定中繼資料（選用）](#set-up-metadata-optional)區段。

   >[!IMPORTANT]
   >
   >由於整合的複雜性，您在儲存初始設定後無法變更存放庫。


## 設定中繼資料（選用）

您可以將[!DNL Workfront]物件資料對應至[!DNL Experience Manager] Assets中的資產媒體欄位。

>[!NOTE]
>
>您只能在一個方向對應中繼資料：從[!DNL Workfront]到[!DNL Experience Manager]。 從[!DNL Experience Manager]連結至[!DNL Workfront]的檔案的中繼資料無法傳輸至[!DNL Workfront]。

### 設定中繼資料欄位

開始對應中繼資料欄位之前，您必須先在Workfront和Experience Manager Assets中設定中繼資料欄位。

若要設定中繼資料欄位：

1. 依照[設定Adobe [!DNL Workfront] 與 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)之間的資產中繼資料對應，在[!DNL Experience Manager Assets]中設定中繼資料結構描述。


1. 在Workfront中設定自訂表單欄位。 [!DNL Workfront]有許多您可以使用的內建自訂欄位。 不過，您也可以建立自己的自訂欄位，如[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中所述。

+++ **展開以檢視有關支援的Workfront和Experience Manager Assets欄位的詳細資訊** 

**Experience Manager Assets標籤**

您可以將任何Workfront支援的欄位對應到Experience Manager Assets中的標籤。 若要這麼做，您必須確保Experience Manager Assets中的標籤值符合Workfront。

* 標籤和Workfront欄位值在拼字和格式上必須是完全相符的。
* 對應至Workfront assets標籤的Experience Manager欄位值必須全部小寫，即使Experience Manager Assets中的標籤似乎包含大寫字母。
* Workfront欄位值不得包含空格。
* Workfront中的欄位值也必須包含Experience Manager Assets標籤的資料夾結構。
* 若要將多個單行文字欄位對應到標籤，請在中繼資料對應的Workfront端輸入標籤值清單（以逗號分隔），並在Experience Manager Assets端輸入`xcm:keywords`。 每個欄位值對應至個別標籤。 您可以使用計算欄位，將多個Workfront欄位合併為單一逗號分隔文字欄位。
* 您可以透過在下拉式清單、單選按鈕或核取方塊欄位中輸入逗號分隔的可用值清單，來對應該欄位的值。


>[!INFO]
>
>**範例**：若要比對此處資料夾結構中所顯示的標籤，Workfront中的欄位值為`landscapes:trees/spruce`。 請注意Workfront欄位值中的小寫字母。
>
>如果您希望標籤成為標籤樹中最左邊的專案，它後面必須跟一個冒號。 在此範例中，若要對應到景觀標籤，Workfront中的欄位值將是`landscapes:`。
>
>AEM中的![資料夾結構](assets/aem-folder-structure-with-red-boxes.png)


在Experience Manager Assets中建立標籤後，標籤會顯示在中繼資料區段的「標籤」下拉式清單下。 若要將欄位連結至標籤，請在中繼資料對應區域的Experience Manager Assets欄位下拉式清單中選取`xcm:keywords`。

如需Experience Manager Assets中標籤的詳細資訊，包括如何建立和管理標籤，請參閱[管理標籤](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags)。

**Experience Manager Assets自訂中繼資料結構描述欄位**

您可以將內建和自訂Workfront欄位對應到Experience Manager Assets中的自訂中繼資料結構欄位。

在Experience Manager Assets中建立的自訂中繼資料欄位，會整理在中繼資料設定區域的各自區段中。

![自訂中繼資料區段](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront欄位**

您可以將內建和自訂Workfront欄位對應至Experience Manager Assets。 Workfront和Experience Manager Assets之間的下列欄位值大小寫和拼字必須相符：

* 下拉式欄位
* 多選欄位

>[!TIP]
>
> 若要檢查欄位值是否完全相符，請前往
>
> * Workfront中的「設定>自訂Forms」或物件中的欄位
> * Assets > Experience Manager Assets中的中繼資料結構

+++

### 對應資產的中繼資料

中繼資料會在資產第一次從[!DNL Workfront]推送時進行對應。 具有內建或自訂欄位的檔案會在第一次將資產傳送到[!DNL Experience Manager Assets]時自動對應到指定的欄位。

若要對應資產的中繼資料：

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. 在&#x200B;**[!UICONTROL [!DNL Workfront]欄位]**&#x200B;欄位中，選擇內建或自訂Workfront欄位。

   >[!NOTE]
   >
   >您可以將單一[!DNL Workfront]欄位對應到多個[!UICONTROL Experience Manager Assets]欄位。 您無法將多個[!DNL Workfront]欄位對應到單一[!DNL Experience Manager Assets]欄位。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. 在[!DNL Experience Manager Assets]欄位中，搜尋預先填入的類別，或在搜尋欄位中輸入至少兩個字母以存取其他類別。
1. 視需要重複步驟2和3。
   ![中繼資料欄位](assets/metadata-no-asset-toggle.png)
1. 按一下[儲存][!UICONTROL ****]&#x200B;或移至本文中的[物件中繼資料同步]](#object-metadata-sync)區段。[



### 物件中繼資料同步

在[!DNL Workfront]中變更欄位時，對應至[!DNL Workfront]投資組合、方案、專案、任務、問題和檔案欄位的[!DNL Experience Manager]欄位會自動更新。

啟用此選項後，任何已推送至Adobe Experience Manager的資產都會在Workfront的「檔案詳細資訊」頁面上顯示檔案Adobe Experience Manager中繼資料的即時檢視。

1. 啟用&#x200B;**[!UICONTROL 同步處理物件中繼資料]**&#x200B;欄位，然後按一下&#x200B;**儲存**。

>[!IMPORTANT]
>
>使用者必須在[!DNL Experience Manager]中擁有物件中資產的寫入存取權，中繼資料才能在更新時同步。


## 傳送檔案至Experience Manager Assets或Assets Essentials

您可以從Workfront傳送檔案至Experience Manager Assets或Assets Essentials。 從Workfront上傳並傳送到Assets Essentials的檔案仍會計入您的整體檔案儲存空間。

透過此整合傳送至Experience Manager的Assets大小限製為&#x200B;**5o TB**。

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

從Workfront傳送資產至Experience Manager Assets或Assets Essentials時，會先對應中繼資料欄位。 設定為對應父物件的任何中繼資料也會一併傳送。 如需設定中繼資料對應的詳細資訊，請參閱[設定Experience Manager Assets as a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

>[!INFO]
>
>**範例**&#x200B;當您第一次傳送附加至專案的資產時，中繼資料會對應至Experience Manager Assets或Assets Essentials，以及父物件（例如投資組合和方案）的任何對應中繼資料。



### 從Workfront傳送檔案

當使用者將檔案從Workfront傳送到Experience Manager Assets或Assets Essentials時，對應的中繼資料會沿著檔案傳輸。 傳送檔案後，在Workfront中對檔案中繼資料所做的變更不會反映在Assets或Assets Essentials中。 如果Workfront中的對應欄位已變更，您必須將包含更新後中繼資料的新版檔案傳送至Assets或Assets Essentials。

若要傳送檔案：

1. 前往Workfront中的&#x200B;**檔案**&#x200B;區域，並選取您要傳送的檔案。
1. 在熒幕底部的列中，按一下&#x200B;**傳送至**。

1. 選擇系統管理員設定的Experience Manager整合，然後按一下[傳送]。****

   >[!NOTE]
   >
   >Workfront管理員可以選擇任何名稱來進行這項整合，因此可能不會特別提及Assets或Assets Essentials。


1. 選擇要將資產移至何處，然後按一下&#x200B;**選取資料夾**。

## 從Experience Manager Assets連結內容

若要連結內容：

1. 前往您要連結內容的Workfront物件。
1. 按一下左側面板中的&#x200B;**檔案**&#x200B;區段。
1. 按一下頁面右側的「**新增**」，然後按一下「**AEM檔案**」以連結個別資產。
   ![將AEM檔案新增至檔案區域](assets/aem-files.png)

1. 使用「內容建議程式」，您可以：

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>使用AI 搜尋搜尋資產。</strong> 使用AI支援的搜尋，瞭解查詢背後的含意和意圖，支援多種語言、拼寫錯誤和同義字。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">更聰明的資產探索AI 搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>根據內容和意圖檢視智慧型建議。</strong> 使用主機Adobe應用程式提供的內容感知建議，探索符合您內容需求的資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">根據內容與意圖的智慧建議</a>。</td>
      </tr>
      <tr>
         <td><strong>上傳行銷活動簡報以探索相關資產。</strong> 上傳PDF、DOCX或TXT行銷活動簡介檔案，讓「內容顧問」可以分析檔案並建議相關資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">探索相關資產的Campaign簡介</a>。</td>
      </tr>
      <tr>
         <td><strong>檢視並選取Dynamic Media資產轉譯。</strong> 瀏覽頻道最佳化的轉譯，包括影像預設集、智慧型裁切和格式型別，並套用Dynamic Media修飾元以即時預覽調整。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <tr>
         <td><strong>將Dynamic Media修飾元套用至轉譯。</strong> 新增修飾元以即時轉換資產轉譯，並在為您的主機應用程式選取轉譯之前預覽結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <tr>
         <td><strong>探索和瀏覽內容片段。</strong> 搜尋內容片段、檢視即時縮圖預覽、檢查狀態（草稿、已修改或已發佈），以及檢查詳細的屬性、參考和變數。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">探索內容片段</a>。</td>
      </tr>
      <tr>
         <td><strong>存取資產中繼資料。</strong> 檢閱與Assets檢視一致的資產屬性，例如標題、說明、格式、大小和其他中繼資料標籤（產品、行銷活動、標籤）。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">存取與Assets檢視一致的資產中繼資料</a>。</td>
      </tr>
      <tr>
         <td><strong>使用預先定義的篩選器來篩選資產。</strong> 使用檔案型別、檔案格式、資產狀態、檔案大小、影像寬度、影像高度、修改日期和建立日期等篩選器來調整資產結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">與Assets檢視一致的存取篩選器</a>。</td>
      </tr>
      <tr>
         <td><strong>儲存並重複使用搜尋。</strong> 指定搜尋字詞和篩選選項，建立已儲存的搜尋，然後在Experience Manager Assets和其他Adobe應用程式中重複使用。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">存取及重複使用最近和儲存的搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>在集合間和集合內搜尋資產。</strong> 在所有集合中搜尋資產或集合，或將搜尋限制在特定集合中。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">搜尋收藏集間和收藏集中的資產</a>。</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >「內容建議程式」中的「建議內容」會使用下列資料來判斷Workfront中的建議內容：
   >
   >* Workfront物件名稱和說明欄位
   >* 標示為必要的自訂表單欄位
   >* 附加檔案中的資料

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## 考量事項

* 連結的AEM資產不支援檢閱和核准工作流程。
* 從Workfront傳送資產至Experience Manager Assets時，會先對應中繼資料欄位。 如果您的Workfront管理員已啟用物件中繼資料同步，則欄位在任一應用程式中變更後仍會保持最新狀態。

<!--
 not sure if this is in yet

### Send a new version

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Assets Essentials. If a mapped field in Workfront has changed, the new version updates the metadata in Assets Essentials when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. If you upload a new version with the exact same file name as a previous version, only the most recent version can be downloaded from Workfront. All versions can be downloaded from Experience Manager Assets or Assets Essentials regardless of the file name. - is this accuate for ESM?

To send the most recent version:

1. Go to the **Documents** area in Workfront, and locate the document.
1. In the bar at the bottom of the screen, click **Send to**. 

1. Choose the Experience Manager integration your administrator set up, then click **Send**.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Assets or Assets Essentials.

1. Click **Save**. The new version saves in the same location as the previous version.
 
 -->