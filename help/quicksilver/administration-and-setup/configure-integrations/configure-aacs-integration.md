---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets整合
description: 您可以透過下列Adobe Experience Manager Assets整合連結您的工作。
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: b874cb1a99840db11d6d55c86b7f779aa3e6ef35
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# 設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 整合

您可以將工作與內容連結，位於 [!DNL Experience Manager Assets]&#x200B;:

* 推送資產和中繼資料 [!DNL Adobe Workfront] to [!DNL Experience Manager Assets]&#x200B;
* 連結資產來源 [!DNL Experience Manager Assets] 至 [!DNL Workfront&#x200B;]
* 加速版本設定使用案例
* 建立連結到的資料夾 [!DNL Experience Manager Assets]
* 追蹤資產和資料夾的中繼資料
* 在之間同步專案中繼資料 [!DNL Workfront] 和 [!DNL Experience Manager Assets]

您也可以跨組織ID將數個Experience Manager Assets存放庫連結至一個Workfront環境，或將數個Workfront環境連結至一個Experience Manager Assets存放庫。 針對您要設定的每個整合，請依照本文的設定指示操作。

## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 計劃*</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 許可證*</strong>
   </td>
   <td>[!UICONTROL計畫]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] 授權</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>產品</strong>
   </td>
   <td>您必須 [!DNL Experience Manager Assets as a Cloud Service]，且您必須以使用者身分新增至產品。
   </td>
  </tr>
  <tr>
   <td>訪問級別配置*
   </td>
   <td>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <strong>授予使用者完整的管理存取權</strong>.
   </td>
  </tr>
</table>


*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。


## 必要條件

開始之前，

* 您必須 [!DNL Workfront] 和 [!DNL Adobe Experience Manager Assets] 與 [!DNL Adobe Admin Consol]e.如需詳細資訊，請參閱 [平台管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 設定整合資訊

1. 按一下 **[!UICONTROL 主菜單]** 圖示，然後按一下 **[!UICONTROL 設定]** .
1. 選擇 **[!UICONTROL 檔案]** 在左側面板中，選取 **[!UICONTROL [!DNL Experience Manager]整合]**.
   >[!NOTE]
   >
   >此設定區域僅在 [!DNL Workfront] 環境包含在 [!DNL Adobe Admin Console].

1. 選擇 **[!UICONTROL 新增 [!DNL Experience Manager] 整合]**.
1. 在 **[!UICONTROL 名稱]** 欄位中，輸入您要讓使用者在Workfront和Experience Manager Assets中與此整合互動時看到的名稱。
1. 在 **[!UICONTROL 導覽URL]** 欄位，系統會自動填入導覽URL。 此唯讀URL可用來連結至貴組織的 [!DNL Experience Manager] 例項 [!UICONTROL 主菜單] 以快速存取。
1. 從 **[!UICONTROL [!DNL Experience Manager]資產存放庫]** 下拉式功能表。 系統會自動填入 [!DNL Experience Manager] 與您的使用者設定檔所指派之組織ID相關聯的存放庫。
   ![選擇experience manager存放庫](assets/setup-information.png)

1. 按一下 **[!UICONTROL 儲存]** 或繼續 [設定中繼資料（選用）](#set-up-metadata-optional) 一節。

   >[!NOTE]
   >
   >由於整合的複雜性，儲存初始設定後，您無法變更存放庫。

## 設定中繼資料（選用）

您可以對應 [!DNL Workfront] 對象資料，以及 [!DNL Experience Manager] 資產。

>[!IMPORTANT]
>
>您只能將中繼資料對應至一個方向：從 [!DNL Workfront] to [!DNL Experience Manager]. 連結到的文檔的元資料 [!DNL Workfront] 從 [!DNL Experience Manager] 無法轉移到 [!DNL Workfront].



### 設定中繼資料欄位

1. 在 [!DNL Experience Manager Assets] 如 [在Adobe之間設定資產中繼資料對應 [!DNL Workfront] 和 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. 在Workfront中設定自訂表單欄位。 [!DNL Workfront] 有許多內建的自訂欄位可供您使用。 不過，您也可以建立自己的自訂欄位，如 [建立或編輯自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### 資產

從推送資產時的中繼資料對應 [!DNL Workfront] 這是第一次。 內建或自訂欄位的檔案會在第一次將資產傳送至時，自動對應至指定的欄位 [!DNL Experience Manager Assets].

>[!NOTE]
>
>此整合不支援來自 [!DNL Adobe Experience Manager].

若要對應資產的中繼資料：

1. 選擇 **[!UICONTROL 資產]** 元資料表格上方。
1. 在 **[!UICONTROL [!DNL Workfront]欄位]** 欄，選擇內建或自訂Workfront欄位。

   >[!NOTE]
   >
   >您可以對應單一 [!DNL Workfront] 欄位至多個 [!UICONTROL Experience Manager Assets] 欄位。 無法映射多個 [!DNL Workfront] 欄位至單一 [!DNL Experience Manager Assets] 欄位。

1. 在 [!DNL Experience Manager Assets] 欄位中，搜尋預先填入的類別，或在搜尋欄位中至少輸入兩個字母以存取其他類別。
1. 視需要重複步驟2和3。
   ![中繼資料欄位](assets/asset-metadata.png)
1. 按一下 [!UICONTROL 儲存] 或繼續 [資料夾](#folders) 一節。

### 資料夾

當使用者在專案上建立連結的資料夾時，相關聯的專案、產品組合和方案資料會對應至 [!DNL Experience Manager Assets].

>[!NOTE]
>
>此整合不支援來自 [!DNL Adobe Experience Manager].

要映射資料夾的元資料：

1. 選擇 **[!UICONTROL 資料夾]** 元資料表格上方。
1. 在 **[!UICONTROL [!DNL Workfront]欄位]** 欄，選擇內建或自訂Workfront欄位。

   >[!NOTE]
   >
   >您可以將單一Workfront欄位對應至多個Experience Manager Assets欄位。 無法映射多個 [!DNL Workfront] 欄位至單一 [!DNL Experience Manager Assets] 欄位。

1. 在 **[!DNL Experience Manager Assets]** 欄位中，搜尋預先填入的類別，或在搜尋欄位中至少輸入兩個字母以存取其他類別。
1. 視需要重複步驟2和3。
   ![資料夾中繼資料](assets/folder-metadata.png)
1. 按一下 **[!UICONTROL 儲存]** 或繼續 [專案中繼資料同步](#project-metadata-sync) 一節。


### 物件中繼資料同步

安 [!DNL Experience Manager] 映射至的欄位 [!DNL Workfront] 當中的欄位更改時，產品組合、方案、項目、任務、問題和文檔欄位將自動更新 [!DNL Workfront].

>[!IMPORTANT]
>
>用戶必須在 [!DNL Experience Manager] 用於物件中的資產，以便在更新時同步中繼資料。

1. 啟用 **[!UICONTROL 同步對象元資料]** 欄位。
1. 按一下「儲存」 ，或移至 [設定連結的資料夾（可選）](#set-up-linked-folders-optional) 一節。

## 設定連結的資料夾（可選）

您可以讓使用者建立連結至的資料夾 [!DNL Experience Manager] 在 [!DNL Workfront] 專案。 連結資料夾時，新增至資料夾的任何資產都會自動顯示在兩者中 [!DNL Workfront] 和 [!DNL Experience Manager]. 將資產新增至 [!DNL Workfront] 資產的中繼資料首次推送至 [!DNL Experience Manager Assets].

在下列步驟中，您會指出要建立連結資料夾的位置。 每個整合只能有一個位置供所有連結的資料夾使用。

要設定連結的資料夾：

1. 切換 **[!UICONTROL 啟用連結的資料夾]** 開啟。
1. 選擇資料夾路徑，以指出您要將所有連結資料夾與這項整合相關聯的位置。

   >[!NOTE]
   >
   >用戶需要在 [!DNL Adobe Experience Manager Assets] 到指定以建立連結資料夾的資料夾。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
