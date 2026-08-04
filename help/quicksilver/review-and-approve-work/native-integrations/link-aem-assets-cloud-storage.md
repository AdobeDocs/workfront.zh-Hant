---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: 將Experience Manager Assets中的內容和資料夾與Adobe雲端儲存空間連結
description: 如果您的組織使用Adobe雲端儲存空間，您可以從Experience Manager Assets將內容和資料夾連結至支援檔案的任何Adobe Workfront物件。
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# 將Experience Manager Assets中的內容和資料夾與Adobe雲端儲存空間連結

如果您的組織使用Adobe雲端儲存空間，您可以將內容和資料夾從Experience Manager Assets連結至Workfront。 連結後，您可以在Workfront中檢視和管理內容，對Experience Manager Assets內容所做的任何變更都會反映在Workfront中。

>[!IMPORTANT]
>
>如果貴組織拒絕簽署GenAI Rider合約，您仍可使用「內容警告器」在Experience Manager Assets中選擇資產和資料夾，但您將無法存取AI支援的功能，例如AI 搜尋、智慧建議或分析行銷活動簡報。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td>您必須擁有Experience Manager as a Cloud Service，且您必須在Admin Console中新增為產品使用者。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager許可權</td> 
    <td>您必須擁有資料夾的寫入許可權。</td> 
   </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視存取許可權或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前：

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[使用Adobe Experience Manager與Frame.io整合](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

* 若要使用Smart Suggestions或Campaign Briefs功能，您必須簽署GenAI Rider。 如需詳細資訊，請參閱[使用內容警告器存取Adobe應用程式中的AEM內容](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)。

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
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">更聰明的資產探索AI 搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>根據內容和意圖檢視智慧型建議。</strong> 使用主機Adobe應用程式提供的內容感知建議，探索符合您內容需求的資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">根據內容與意圖的智慧建議</a>。</td>
      </tr>
      <tr>
         <td><strong>上傳行銷活動簡報以探索相關資產。</strong> 上傳PDF、DOCX或TXT行銷活動簡介檔案，讓「內容顧問」可以分析檔案並建議相關資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">探索相關資產的Campaign簡介</a>。</td>
      </tr>
      <tr>
         <td><strong>檢視並選取Dynamic Media資產轉譯。</strong> 瀏覽頻道最佳化的轉譯，包括影像預設集、智慧型裁切和格式型別，並套用Dynamic Media修飾元以即時預覽調整。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <tr>
         <td><strong>將Dynamic Media修飾元套用至轉譯。</strong> 新增修飾元以即時轉換資產轉譯，並在為您的主機應用程式選取轉譯之前預覽結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>存取資產中繼資料。</strong> 檢閱與Assets檢視一致的資產屬性，例如標題、說明、格式、大小和其他中繼資料標籤（產品、行銷活動、標籤）。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">存取與Assets檢視一致的資產中繼資料</a>。</td>
      </tr>
      <tr>
         <td><strong>使用預先定義的篩選器來篩選資產。</strong> 使用檔案型別、檔案格式、資產狀態、檔案大小、影像寬度、影像高度、修改日期和建立日期等篩選器來調整資產結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">與Assets檢視一致的存取篩選器</a>。</td>
      </tr>
      <tr>
         <td><strong>儲存並重複使用搜尋。</strong> 指定搜尋字詞和篩選選項，建立已儲存的搜尋，然後在Experience Manager Assets和其他Adobe應用程式中重複使用。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">存取及重複使用最近和儲存的搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>在集合間和集合內搜尋資產。</strong> 在所有集合中搜尋資產或集合，或將搜尋限制在特定集合中。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">搜尋收藏集間和收藏集中的資產</a>。</td>
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
