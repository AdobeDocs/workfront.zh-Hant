---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 設定Experience Manager Assets Essentials整合
description: 在Experience Manager Assets Essentials中將您的工作與您的內容連線起來。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 1%

---

# 設定 Experience Manager Assets Essentials 整合

在Experience Manager Assets Essentials&#x200B;中將您的工作與內容連線起來：

* 將資產和中繼資料從Adobe Workfront推送到Experience Manager Assets Essentials&#x200B;。
* 從Experience Manager Assets Essentials將資產連結到Workfront中的專案和任務&#x200B;。
* 促進推送到Experience Manager Assets Essentials的資產版本設定工作流程

>[!NOTE]
>
>您也可以將多個Experience Manager Assets存放庫連線至一個Workfront環境，或連線至跨組織ID的一個Workfront存放庫的多個Experience Manager Assets環境。 針對您要設定的每項整合，請依照本文的設定指示操作。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 計劃
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 授權
   </td>
   <td><p>目前： [!UICONTROL 計畫]</p>
   <p>新增：[!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] 授權
   </td>
   <td>[!UICONTROL 標準]
   </td>
  </tr>
  <tr>
   <td>產品
   </td>
   <td>您必須擁有Experience Manager Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。
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

## 設定整合

{{step-1-to-setup}}

1. 在左側面板中選取&#x200B;**檔案** ![檔案圖示](assets/document-icon.png)，然後選取&#x200B;**Experience Manager整合**。
1. 選取&#x200B;**新增Experience Manager整合**。
1. 指定下列專案：

   <table>
   <tr>
      <td><strong>名稱</strong>
      </td>
      <td>在「檔案」區域的「新增」按鈕中，輸入您要讓使用者看到的名稱。
      </td>
   </tr>
   <tr>
      <td><strong>導覽URL</strong>
      </td>
      <td>系統會自動填入導覽URL。 此URL用於從主選單連結到您組織的Assets Essentials例項以快速訪問。
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

1. 按一下&#x200B;**儲存**&#x200B;或移至本文中的[設定中繼資料（選用）](#set-up-metadata-optional)區段。


## 設定中繼資料（選擇性）

將Workfront物件資料對應至Experience Manager Assets中的資產媒體欄位。 中繼資料會在第一次從Workfront推送資產時進行對應。


### 先決條件

開始之前，您必須

* 在Experience Manager Assets Essentials中設定中繼資料結構，如[設定Adobe Workfront和Experience Manager Assets之間的資產中繼資料對應](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)中所述。
* （選用）在Workfront中設定自訂表單欄位。 Workfront有許多內建的自訂欄位可供您使用。 不過，您也可以建立自己的自訂欄位。 如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 支援的Workfront和Experience Manager Assets欄位

### AEM關鍵字

您可以將任何Workfront支援的欄位對應到Experience Manager Assets Essentials中的關鍵字。

若要將欄位連結至關鍵字，請在中繼資料對應區域的Experience Manager Assets欄位下拉式清單中選取`xcm:keywords`。

若要將多個單行文字欄位對應到關鍵字，請在中繼資料對應的Workfront端輸入關鍵字值的逗號分隔清單，並在Experience Manager Assets端輸入`xcm:keywords`。 每個欄位值都會對應至個別的關鍵字。 您可以使用計算欄位，將多個Workfront欄位合併為單一逗號分隔文字欄位。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=zh-Hant).
-->


### 資產

中繼資料會在第一次從Workfront推送資產時進行對應。 具有內建或自訂欄位的檔案，在首次將資產傳送到Experience Manager Assets Essentials時會自動對應到指定的欄位。

1. 在&#x200B;**Workfront欄位**&#x200B;欄位中，選擇內建或自訂Workfront欄位。

   >[!NOTE]
   >
   >您可以將單一Workfront欄位對應至多個Experience Manager Assets欄位。 您無法將多個Workfront欄位對應至單一Experience Manager Assets欄位。

1. 在&#x200B;**Experience Manager**&#x200B;欄位中，選擇Experience Manager Assets欄位。

   若要將Workfront欄位對應至Experience Manager Assets標籤，請選取「`xcm:keywords`」。

1. 視需要重複步驟1和2。
   ![啟用中繼資料](assets/metadata-assets-essentials.png)
1. 按一下&#x200B;**儲存**&#x200B;或移至本文中的[設定連結資料夾（選用）](#set-up-linked-folders-optional)區段。


## 設定連結的資料夾（選擇性）

{{setup-linked-folder}}
