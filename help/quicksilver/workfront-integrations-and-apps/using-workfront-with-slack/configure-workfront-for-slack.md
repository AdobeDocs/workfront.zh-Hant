---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: '設定Slack的 [!DNL Adobe Workfront] '
description: 將 [!DNL Adobe Workfront] 與Slack整合可讓您從Slack存取及建立 [!DNL Workfront] 個工作專案、核准、我的最愛、最近專案。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
TQID: https://experienceleague.adobe.com/rOccEnbPoWVh5LFVPCeX81S3Nl-VpEBGGfcNDNXEdPk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 417
ht-degree: 4%

---

# 設定 [!DNL Adobe Workfront for Slack]

將[!DNL Adobe Workfront]與[!DNL Slack]整合可讓您執行下列動作：

* 從[!DNL Slack]存取您的[!DNL Workfront]工作專案、核准、我的最愛、最近專案。
* 從[!DNL Slack]訂閱、核准、指派工作。
* 從[!DNL Slack]建立任務和問題。
* 在[!DNL Slack]中接收一些[!DNL Workfront]通知。

視您的[!DNL Slack]環境設定方式而定，您可以自行安裝及設定[!DNL Workfront for Slack]，或您的[!DNL Workfront]管理員必須先安裝及設定，您才能自行設定。

當您將[!DNL Slack]執行個體與[!DNL Workfront]整合時，使用者可在其[!DNL Slack]管道內共同作業時使用[!DNL Workfront]。 整合可從任何[!DNL Slack]環境使用，包括[!DNL Slack]行動應用程式。 ##存取需求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 搭配[!DNL Slack]使用[!DNL Workfront]的必要條件

* 您必須有[!DNL Slack]個執行個體。
* 您的[!DNL Slack]系統管理員必須允許所有[!DNL Slack]使用者安裝[!DNL Workfront for Slack]。
* 您必須擁有[!DNL Workfront]授權才能使用[!DNL Workfront]中的整合功能。

  >[!NOTE]
  >
  >具有任何[!DNL Workfront]授權型別的使用者可以從[!DNL Slack]存取[!DNL Workfront]。 您可以從[!DNL Slack]執行的動作僅限於您的[!DNL Workfront]授權和許可權層級。

如需在[!DNL Slack]中管理應用程式的詳細資訊，請參閱[為您的Workspace管理應用程式。](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## 安裝[!DNL Workfront for Slack]

每個[!DNL Slack]使用者必須自行安裝[!DNL Workfront]應用程式，才能使用來自[!DNL Slack]的[!DNL Workfront]。

您可以透過下列方式安裝應用程式：

* [在 [!DNL Slack]外部安裝 [!DNL Workfront] 應用程式](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [在 [!DNL Slack]內安裝 [!DNL Workfront] 應用程式](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### 在[!DNL Slack]外部安裝[!DNL Workfront]應用程式 {#install-the-workfront-app-outside-slack}

請依照下列步驟執行安裝程式，並在您的[!DNL Slack]執行個體上授權[!DNL Workfront for Slack]。

>[!IMPORTANT]
>
>發行Slack適用的[!DNL Workfront]新版本時，您必須重新授權應用程式才能繼續使用。

1. 在[[!DNL Slack] 存放區](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info)中找到[!DNL Adobe Workfront]附加元件。

1. 按一下&#x200B;**[!UICONTROL 在[!DNL Slack]]**&#x200B;中開啟。

1. 指定您的[!DNL Slack] URL並按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以登入您的工作區。\

1. 檢查[!DNL Slack]要求的存取權。 如果您同意此存取權，請按一下[允許存取] ****&#x200B;來授權[!DNL Workfront]應用程式。

您現在可以從[!DNL Slack]存取[!DNL Workfront]，如[從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 存取 [!DNL Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中所述。

### 在[!DNL Slack]內安裝[!DNL Workfront]應用程式 {#install-the-workfront-app-within-slack}

您可以直接從[!DNL Slack]應用程式安裝[!DNL Workfront]應用程式：

1. 導覽至您的[!DNL Slack] URL。

   例如： *`<YourTeamName>`.slack.com/apps*。

   或

   按一下[!DNL Slack]執行個體中的&#x200B;**[!UICONTROL 新增應用程式]**&#x200B;圖示。

1. 開始在搜尋欄位中輸入&#x200B;*[!DNL Workfront]*。
1. 按Enter鍵。
1. 選取&#x200B;**[!DNL Workfront]**&#x200B;應用程式。
1. 按一下&#x200B;**[!UICONTROL 設定]**。

   此時會顯示「應用程式目錄」頁面。

1. 按一下&#x200B;**[!UICONTROL 造訪應用程式網站]**。
1. 按一下「**[!UICONTROL 新增至[!DNL Slack]]**」。
1. 請依照步驟完成安裝。
1. 安裝完成時，您可以從[!DNL Slack]存取[!DNL Workfront]，如[[！UICONTROL Access [!DNL Workfront]  from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中所述。
