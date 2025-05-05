---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 設定[!UICONTROL Experience Manager Assets as a Cloud Service]整合
description: 您可以在 [!DNL Experience Manager Assets]中將您的工作與您的內容連結。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1708'
ht-degree: 0%

---

# 設定[!UICONTROL Experience Manager Assets as a Cloud Service]整合

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>此功能僅適用於已加入[!DNL Adobe Admin Console]的組織。

您可以在&#x200B;[!DNL Experience Manager Assets]中將您的工作與您的內容連結：

* 將資產和中繼資料從[!DNL Adobe Workfront]推送到[!DNL Experience Manager Assets]&#x200B;
* 從[!DNL Experience Manager Assets]連結資產至您在[!DNL Workfront&#x200B;]中的專案和任務
* 促進版本設定使用案例
* 建立連結至[!DNL Experience Manager Assets]的資料夾
* 追蹤資產和資料夾的中繼資料
* 在[!DNL Workfront]和[!DNL Experience Manager Assets]之間同步專案中繼資料

>[!NOTE]
>
>您也可以將多個[!DNL Experience Manager Assets]存放庫連線至一個[!UICONTROL Workfront]環境，或將多個[!DNL Workfront]環境連線至跨組織ID的一個[!DNL Experience Manager Assets]存放庫。 針對您要設定的每項整合，請依照本文的設定指示操作。

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


## 設定整合資訊

{{step-1-to-setup}}

1. 在左側面板中選取&#x200B;**[!UICONTROL 檔案]**，然後選取&#x200B;**[!UICONTROL [!DNL Experience Manager]整合]**。

   >[!NOTE]
   >
   >只有在[!DNL Workfront]環境包含在[!DNL Adobe Admin Console]之下時，此設定區域才會出現。

1. 選取&#x200B;**[!UICONTROL 新增[!DNL Experience Manager]整合]**。
1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中，輸入您希望使用者在Workfront和Experience Manager Assets中與此整合互動時看到的名稱。
1. 在&#x200B;**[!UICONTROL 導覽URL]**&#x200B;欄位中，系統會自動填入導覽URL。 此唯讀URL是用來從[!UICONTROL 主功能表]連結至您組織的[!DNL Experience Manager]執行個體，以進行快速存取。
1. 從&#x200B;**[!UICONTROL [!DNL Experience Manager]Assets存放庫]**&#x200B;下拉式功能表中選擇存放庫。 系統會自動填入與您的使用者設定檔所指派之組織ID相關聯的任何[!DNL Experience Manager]存放庫。
   ![選擇experience manager存放庫](assets/setup-information.png)

1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;或移至本文中的[設定中繼資料（選用）](#set-up-metadata-optional)區段。

   >[!NOTE]
   >
   >由於整合的複雜性，您在儲存初始設定後無法變更存放庫。

## 設定中繼資料（選用）

您可以將[!DNL Workfront]物件資料對應至[!DNL Experience Manager] Assets中的資產媒體欄位。

>[!IMPORTANT]
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
1. 按一下[!UICONTROL 儲存]或移至本文中的[設定工作流程](#set-up-workflows-optional)區段。

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## 設定工作流程（選用）

工作流程是一組將Workfront連線至Adobe Experience Manager as a Cloud Service的動作。 身為Workfront管理員，您可以在Workfront中設定工作流程，然後將它們指派給專案範本。

使用指派了工作流程的專案範本建立專案時，會觸發工作流程中定義的動作。

已啟用並設定整個Adobe Experience Manager的工作流程。 這些工作流程隨後可套用至專案範本。 可在範本層級，或在從該範本建立專案時於專案層級調整或自訂這些引數。

Adobe Experience Manager整合提供下列工作流程：

* [建立Adobe Experience Manager連結資料夾](#create-adobe-experience-manager-linked-folders)
* [發佈傳送至Adobe Experience Manager Assets的資產](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### 建立Adobe Experience Manager連結資料夾

每個資料夾樹狀結構最多可建立100個連結資料夾。

1. 將&#x200B;**[!UICONTROL 建立連結資料夾]**&#x200B;切換為開啟。
1. 輸入您正在建立的連結資料夾名稱。
1. （視條件而定）如果您想要此連結資料夾成為使用使用此整合之範本所建立專案的預設資料夾，請啟用&#x200B;**預設資料夾樹狀結構**&#x200B;選項。 您可以選取一或多個預設資料夾。
1. 選擇資料夾路徑，以指出您要將所有連結的資料夾與此整合相關聯的位置。
1. （視條件而定）若要將資料夾樹狀結構（巢狀資料夾）新增至此整合，請執行下列動作：

   1. 按一下&#x200B;**新增資料夾**&#x200B;圖示![新增資料夾](assets/add-folder-aem.png)。
   1. 在&#x200B;**名稱型別**&#x200B;欄位中，選取您要如何命名資料夾：

      * **名稱**：輸入資料夾的名稱。
      * **物件資料**：選取資料夾名稱的來源，例如專案名稱。

      >[!NOTE]
      >
      >* 資料夾名稱必須少於100個字元。
      >* 下列字元將會從資料夾名稱中移除：
      >
      >   `/`，`:`，`[`，`]`，`|`，`*`

   1. 若要將巢狀資料夾新增至資料夾樹狀結構，請按一下您要在其中建立巢狀資料夾的資料夾旁邊的三個點功能表，然後選取&#x200B;**新增資料夾**。 依照上一步驟中的說明填寫欄位。
   1. 若要將資料夾連結至Workfront，請選取該資料夾，然後按一下&#x200B;**建立連結的資料夾**   圖示![連結資料夾](assets/link-folder.png)。
   1. （選擇性）若要編輯資料夾，請選取資料夾並按一下&#x200B;**編輯資料夾**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
   1. （選擇性）若要刪除資料夾，請選取資料夾並按一下&#x200B;**刪除資料夾**&#x200B;圖示![刪除資料夾](assets/delete-folder.png)。
1. （視條件而定）若要新增另一個資料夾樹狀結構，請按一下&#x200B;**+新增資料夾樹狀結構**，並依照步驟5中的步驟進行。

1. 按一下&#x200B;**[!UICONTROL 儲存]**，或繼續前往本文中傳送至Adobe Experience Manager Assets[&#128279;](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)的發佈資產區段。

>[!NOTE]
>
>* 此整合最多只會建立100個資料夾，無論已建立多少資料夾樹狀結構。 例如，與4個資料夾樹狀結構的整合最多可建立100個資料夾，而不是400個資料夾。
>* 資料夾樹狀結構中的第一個資料夾會自動標示為連結至Workfront。 如果您不想要連結此資料夾，可以取消其連結。
>* 如果未提供資料夾樹狀結構，則根資料夾會成為連結的資料夾。


### 發佈傳送至Adobe Experience Manager Assets的資產

1. 開啟&#x200B;**[!UICONTROL 自動發佈資產]**。
1. 勾選您要發佈傳送至Adobe Experience Manager資產之資產的位置旁的方塊。 您可以啟用任一或兩個選項。
1. （視條件而定）如果您已啟用Brand Portal選項，請選取您要發佈資產的Brand Portal 。
1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;或移至本文中的[設定連結資料夾（選用）](#set-up-linked-folders-optional)區段。

## 設定連結的資料夾（選擇性）

您可以在[!DNL Workfront]專案中允許使用者建立連結至[!DNL Experience Manager]的資料夾。 連結資料夾時，新增至資料夾的任何資產都會自動顯示在[!DNL Workfront]和[!DNL Experience Manager]中。 當資產第一次新增到[!DNL Workfront]中的連結資料夾時，資產的中繼資料會被推送到[!DNL Experience Manager Assets]。

在下列步驟中，您會指示您要在哪個位置建立連結資料夾。 每個整合只能有一個位置用於所有連結的資料夾。

若要設定連結的資料夾：

1. 將&#x200B;**[!UICONTROL 啟用連結資料夾]**&#x200B;切換為開啟。
1. 選擇資料夾路徑，以指出您要將所有連結的資料夾與此整合相關聯的位置。

   >[!NOTE]
   >
   >使用者需要[!DNL Adobe Experience Manager Assets]中的寫入許可權，才能建立連結資料夾。

1. 按一下「**[!UICONTROL 儲存]**」。
