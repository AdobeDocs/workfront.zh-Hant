---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 設定Experience Manager Assets Essentials整合
description: 在Experience Manager Assets Essentials中將您的工作與您的內容連線起來。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 3%

---

# 設定 Experience Manager Assets Essentials 整合

在Experience Manager Assets Essentials&#x200B;中將您的工作與內容連線起來：

* 將資產和中繼資料從Adobe Workfront推送到Experience Manager Assets Essentials&#x200B;。
* 從Experience Manager Assets Essentials將資產連結到Workfront中的專案和任務&#x200B;。
* 促進推送到Experience Manager Assets Essentials的資產版本設定工作流程

>[!NOTE]
>
>您也可以將多個Experience Manager Assets存放庫連線至一個Workfront環境，或連線至跨組織ID的一個Workfront存放庫的多個Experience Manager Assets環境。 針對您要設定的每項整合，請依照本文的設定指示操作。<br>
>新檔案區域未提供此功能。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table>
  <tr>
   <td><strong>Adobe Workfront封裝</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權</strong>
   </td>
   <td>
   <p>標準</p>
   <p>規劃</p>
   </td>
  </tr>
  <tr>
   <td><strong>其他產品</strong>
   </td>
   <td>您必須擁有Experience Manager Assets as a Cloud Service或Assets Essentials，並且您必須以使用者身分新增到產品中。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager許可權</strong>
   </td>
   <td>您必須擁有Experience Manger整合中目的地資料夾的寫入許可權。
   </td>
  </tr>
  <tr>
   <td><strong>存取層級設定</strong>
   </td>
   <td>您必須是Workfront管理員才能設定Experience Manager整合。 完成設定後，擁有計畫授權的使用者可以在個別專案上設定連結資料夾。
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
      <td><strong>Navigation URL</strong>
      </td>
      <td>The system automatically populates the Navigation URL. This URL is used to link to your organization's Assets Essentials instance from the Main Menu for quick access.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets repository</strong>
      </td>
      <td>
      The system automatically populates the Experience Manager repository associated with your Organization ID.
      </td>
   </tr>
   </table>

1. Click **Save** or move on to the [Set up metadata (optional)](#set-up-metadata-optional) section in this article.


## Set up metadata (optional)

Map Workfront object data to asset media fields in Experience Manager Assets. Metadata maps when an asset is pushed from Workfront for the first time.


### 先決條件

開始之前，您必須

* Configure a metadata schema in Experience Manager Assets Essentials as explained in [Configure asset metadata mapping between Adobe Workfront and Experience Manager Assets](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
* (Optional) Configure custom form fields in Workfront. Workfront has many built-in custom fields you can use. However, you can also create your own custom fields. For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Supported Workfront and Experience Manager Assets fields

### AEM Keyword

You can map any Workfront supported field to a keyword in Experience Manager Assets Essentials.

To link a field to a keyword, select `xcm:keywords` in the Experience Manager Assets field dropdown in the metadata mapping area.

To map multiple single-line text fields to keywords, enter a comma-separated list of the keyword values into the Workfront side of the metadata mapping, and `xcm:keywords` on the Experience Manager Assets side. Each field value maps to a separate keyword. You can use a calculated field to combine multiple Workfront fields into a single comma-separated text field.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=zh-Hant).
-->


### 資產

Metadata maps when an asset is pushed from Workfront for the first time. Documents with the built-in or custom fields automatically map to the specified fields the first time an asset is sent to Experience Manager Assets Essentials.

1. In the **Workfront field** column, choose a built-in or custom Workfront field.

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
