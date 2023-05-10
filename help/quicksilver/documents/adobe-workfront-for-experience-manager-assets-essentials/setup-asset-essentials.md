---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 設定Experience Manager Assets Essentials整合
description: 在Experience Manager Assets Essentials - EDIT ME中連結您的作品和內容。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 9965ec9f436724e438fbbc5977f22761cc673878
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 4%

---

# 設定Experience Manager Assets Essentials整合

使用Experience Manager Assets Essentials中的內容連接您的工作&#x200B;:

* 將資產和中繼資料從Adobe Workfront推送至Experience Manager Assets Essentials &#x200B;
* 將資產從Experience Manager Assets Essentials連結至您在Workfront中的專案和工&#x200B;作
* 加速推送至Experience Manager Assets Essentials之資產的版本設定工作流程

您也可以跨組織ID將數個Experience Manager Assets存放庫連結至一個Workfront環境，或將數個Workfront環境連結至一個Experience Manager Assets存放庫。 針對您要設定的每個整合，請依照本文的設定指示操作。

## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>Adobe Workfront計畫*</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權*</strong>
   </td>
   <td>計劃
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager授權</strong>
   </td>
   <td>標準
   </td>
  </tr>
  <tr>
   <td><strong>產品</strong>
   </td>
   <td>您必須有Experience Manager Assets Essentials，且必須以Admin Console使用者身分新增至產品中。
   </td>
  </tr>
  <tr>
   <td><strong>訪問級別配置</strong>
   </td>
   <td>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱 <strong>授予使用者完整的管理存取權</strong>.
   </td>
  </tr>
</table>


*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。


## 設定整合

1. 按一下 **主菜單** 圖示，然後按一下 **設定**.
1. 選擇  **檔案** ![文檔表徵圖](assets/document-icon.png) 在左側面板中，選取 **Experience Manager整合**.
1. 選擇 **新增Experience Manager整合**.
1. 指定下列項目：

   <table>
   <tr>
      <td><strong>名稱</strong>
      </td>
      <td>在「文檔」區域的「添加新」按鈕中輸入希望用戶看到的名稱。
      </td>
   </tr>
   <tr>
      <td><strong>導覽URL</strong>
      </td>
      <td>系統會自動填入導覽URL。 此URL可從主功能表連結至貴組織的Assets Essentials執行個體，以供快速存取。
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets存放庫</strong>
      </td>
      <td>
      系統會自動填入與您的組織ID相關聯的Experience Manager存放庫。
      </td>
   </tr>
   </table>

1. 按一下 **儲存** 或繼續 [設定中繼資料（選用）](#set-up-metadata-optional) 一節。


## 設定中繼資料（選用）

將 Workfront 物件資料對應到 Experience Manager Assets 中的資產媒體欄位。中繼資料會在第一次從 Workfront 中推播資產時進行對應。


### 必要條件

開始之前，您必須

* 在Experience Manager Assets Essentials中設定中繼資料結構，如 [設定Adobe Workfront和Experience Manager Assets之間的資產中繼資料對應](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* （選用）在Workfront中設定自訂表單欄位。 Workfront有許多內建的自訂欄位可供您使用。 不過，您也可以建立自己的自訂欄位。 如需詳細資訊，請參閱 [建立或編輯自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **支援的Workfront和Experience Manager Assets欄位**

**AEM關鍵字**

您可以將任何Workfront支援的欄位對應至Experience Manager Assets Essentials中的關鍵字。

若要將欄位連結至關鍵字，請選取 `dc:subject` 在中繼資料對應區域的「Experience Manager Assets」欄位下拉式清單中。

若要將多個單行文字欄位對應至關鍵字，請在中繼資料對應的Workfront側輸入以逗號分隔的關鍵字值清單，並 `dc:subject` 在Experience Manager Assets那邊。 每個欄位值對應至個別的關鍵字。 您可以使用計算欄位，將多個Workfront欄位合併為單一逗號分隔的文字欄位。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### 資產

首次從Workfront推送資產時，會對應中繼資料。 內建或自訂欄位的檔案會在第一次將資產傳送至Experience Manager Assets Essentials時，自動對應至指定的欄位。

1. 在 **Workfront欄位** 欄，選擇內建或自訂Workfront欄位。
   >[!NOTE]
   >
   >您可以將單一Workfront欄位對應至多個Experience Manager Assets欄位。 您無法將多個Workfront欄位對應至單一Experience Manager Assets欄位。
1. 在 **Experience Manager** 欄位，選擇Experience Manager Assets欄位。

   若要將Workfront欄位對應至Experience Manager Assets標籤，請選取 `dc:subject`.
1. 視需要重複步驟1和2。
   ![啟用中繼資料](assets/metadata-assets-essentials.png)
1. 按一下 **儲存** 或繼續 [設定連結的資料夾（可選）](#set-up-linked-folders-optional) 一節。


## 設定連結的資料夾（可選）

{{setup-linked-folder}}
