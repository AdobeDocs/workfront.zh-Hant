---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 使用由Experience Manager Assets提供支援的「內容建議程式」連結內容和資料夾
description: 您可以使用「內容建議程式」，將內容或資料夾從Experience Manager Assets連結至任何支援檔案的Adobe Workfront物件。 Content Advisor將智慧型內容感知探索功能直接匯入Workfront，協助您快速找到相關且經過核准的內容。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 2%

---

# 使用Experience Manager Assets的內容警告器連結內容和資料夾

Content Advisor將智慧型內容感知探索功能直接匯入Workfront，協助您根據內容快速找到相關且核准的內容。 藉由智慧建議、Dynamic Media轉譯和詳細資產中繼資料等功能，您能夠在不離開Workfront的情況下有效評估和重複使用內容，進而加快內容建立速度，同時維持品牌一致性。

您可以使用「內容建議程式」，將內容和資料夾從Experience Manager Assets連結至Workfront。 連結後，您可以在Workfront中檢視和管理內容，對Experience Manager Assets內容所做的任何變更都會反映在Workfront中。

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
   <td>您必須擁有Experience Manager as a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。</td> 
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

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[設定Experience Manager Assets as a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)。

* 若要使用Smart Suggestions或Campaign Briefs功能，您必須簽署GenAI Rider。 如需詳細資訊，請參閱[使用內容警告器存取Adobe應用程式中的AEM內容](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)。



## 使用「內容建議程式」從Experience Manager Assets連結內容

您現在可以使用內容警告器，直接在Workfront中連結Experience Manager Assets的內容。 內容警告器不適用於Assets Essentials。

若要連結內容：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取「**新增**」，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及Experience Manager Assets。

1. 使用「內容建議程式」，您可以：


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>使用AI 搜尋搜尋資產。</strong>使用AI支援的搜尋，可瞭解查詢背後的含意和意圖，支援多種語言、拼寫錯誤和同義字。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">更聰明的資產探索AI 搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>根據內容和意圖檢視智慧型建議。</strong>使用主機Adobe應用程式的內容感知建議，探索符合您內容需求的資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">根據內容與意圖的智慧建議</a>。</td>
      </tr>
      <tr>
         <td><strong>上傳行銷活動簡報，以探索相關資產。</strong>上傳PDF、DOCX或TXT行銷活動簡介檔案，讓內容顧問分析檔案並建議相關資產。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">探索相關資產的Campaign簡介</a>。</td>
      </tr>
      <tr>
         <td><strong>檢視並選取Dynamic Media資產轉譯。</strong>瀏覽頻道最佳化的轉譯，包括影像預設集、智慧型裁切和格式型別，並套用Dynamic Media修飾元以即時預覽調整。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <tr>
         <td><strong>將Dynamic Media修飾元套用至轉譯。</strong>新增修飾元以即時轉換資產轉譯，並在為您的主機應用程式選取轉譯之前預覽結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的動態媒體資產轉譯</a>。</td>
      </tr>
      <tr>
         <td><strong>探索和瀏覽內容片段。</strong>搜尋內容片段、檢視即時縮圖預覽、檢查狀態（草稿、已修改或已發佈），以及檢查詳細的屬性、參考和變數。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">探索內容片段</a>。</td>
      </tr>
      <tr>
         <td><strong>存取資產中繼資料。</strong>檢閱與Assets檢視一致的資產屬性，例如標題、說明、格式、大小和其他中繼資料標籤（產品、行銷活動、標籤）。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">存取與Assets檢視一致的資產中繼資料</a>。</td>
      </tr>
      <tr>
         <td><strong>使用預先定義的篩選器來篩選資產。</strong>使用檔案型別、檔案格式、資產狀態、檔案大小、影像寬度、影像高度、修改日期和建立日期等篩選器來調整資產結果。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">與Assets檢視一致的存取篩選器</a>。</td>
      </tr>
      <tr>
         <td><strong>儲存並重複使用搜尋。</strong>指定搜尋字詞和篩選選項，建立已儲存的搜尋，然後透過Experience Manager Assets和其他Adobe應用程式重複使用。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">存取及重複使用最近和儲存的搜尋</a>。</td>
      </tr>
      <tr>
         <td><strong>在集合間和集合內搜尋資產。</strong>搜尋所有集合中的資產或集合，或將搜尋限制在特定集合中。</td>
         <td>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">搜尋收藏集間和收藏集中的資產</a>。</td>
      </tr>
   </tbody>
   </table>


### 使用「內容建議程式」從Experience Manager Assets連結新版本

您可以從Experience Manager Assets或Assets Essentials提取新內容，並將其作為新版本新增到現有資產。 如果檔案已連結，並在Experience Manager Assets或Assets Essentials中新增了新版本，新版本會自動在Workfront中顯示。

若要連結新版本：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取您要取代為新版本的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 選取「**新增** > **版本**」，然後選取系統管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能未特別提及Experience Manager Assets。

1. 選取您要連結的內容：

   * 選取Assets標籤以瀏覽Experience Manager Assets或Assets Essentials中的資產、資料夾或集合。

     ![內容顧問](assets/content-advisor-full.png)

   * 內容片段不支援版本。 如果您選取內容片段，新版本將會取代現有的內容片段，而不會建立新版本。

1. 按一下「**選取**」。

## 從Experience Manager Assets連結資料夾與內容建議程式

檢視檔案夾內個別資產的許可權取決於Experience Manager Assets許可權。

連結資料夾：

1. 移至Workfront中您想要資料夾的&#x200B;**檔案**&#x200B;區域。
1. 選取「**新增**」，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能未特別提及Experience Manager Assets。

1. 按一下&#x200B;**Assets** > **檔案與資料夾**。

1. 按一下&#x200B;**篩選器**&#x200B;圖示，然後在&#x200B;**資產型別**&#x200B;區段中，選擇&#x200B;**資料夾**。

1. 選取您要連結的資料夾。

1. 按一下「**選取**」。

## 考量事項

* 使用Adobe Enterprise Storage的物件無法使用「內容建議程式」功能。 如果您的組織使用Adobe企業儲存空間，您仍然可以從Experience Manager Assets或Assets Essentials連結資產和資料夾，但您將無法存取Content Advisor功能，例如AI 搜尋、智慧建議或Dynamic Media轉譯。 如需詳細資訊，請參閱[使用Adobe Experience Manager與Frame.io整合](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

* 內容警告器功能不適用於Assets Essentials。 若要從Assets Essentials連結資產和資料夾，請參閱[從Experience Manager Assets Essentials連結資產和資料夾](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md)。

* 從Workfront傳送資產至Experience Manager Assets時，會先對應中繼資料欄位。 如果您的Workfront管理員已啟用物件中繼資料同步，則欄位在任一應用程式中變更後仍會保持最新狀態。
