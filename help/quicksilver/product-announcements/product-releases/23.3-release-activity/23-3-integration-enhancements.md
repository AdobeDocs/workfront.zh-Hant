---
title: 23.3整合增強功能
description: 23.3整合增強功能
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3整合增強功能

本頁說明23.3版本的所有整合增強功能。 這些增強功能已在2023年7月20日和21日的23.3版本中在生產環境中提供。

如需23.3版本週期目前可用的所有變更清單，請參閱 [23.3版本總覽](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## 全新G Suite整合現已推出

Google Marketplace現在提供新的G Suite整合。 新的整合使用OAuth2進行驗證，並取代先前的整合。

先前的G Suite整合功能現已棄用，並將自動解除安裝。

如需如何安裝新整合的說明，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

如需適用於G Suite的Workfront的詳細資訊，請參閱 [適用於G Suite的Workfront](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud整合現在支援多個指派使用者

Adobe Creative Cloud整合現在支援在任務或問題有多個指派使用者時，選擇「完成我的部分」和「完成」（或「已解決」）的功能。

以前，整合可讓使用者將任務標示為完成，而不需指定「已完成我的部分」或「完成」/「已解決」。

若要善用此功能，請下載並安裝最新的WorkfrontCreative Cloud外掛程式。

如需功能的詳細資訊，請參閱 [使用Adobe Workfront外掛程式將工作專案標示為完成](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

如需有關安裝適用於Creative Cloud外掛程式的Workfront的資訊，請參閱 [安裝適用於Creative Cloud應用程式的Adobe Workfront外掛程式](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## 從Workfront檢視及管理適用於Creative Cloud外掛程式的Workfront通知

為了讓您更輕鬆地接收所需的通知，我們讓您能夠檢視和管理Workfront通知，而不需要離開Adobe Creative Cloud。 現在，您可以直接從Creative Cloud應用程式的Workfront外掛程式視窗中檢視通知，以及存取與這些通知相關的工作專案和註解。

以前，通知只能在Workfront內透過電子郵件取得。

若要善用此功能，請下載並安裝最新的WorkfrontCreative Cloud外掛程式。

如需詳細資訊，請參閱 [檢視和管理 [!DNL Adobe Workfront] 來自Adobe Creative Cloud的通知](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

如需有關安裝適用於Creative Cloud外掛程式的Workfront的資訊，請參閱 [安裝適用於Creative Cloud應用程式的Adobe Workfront外掛程式](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## 建立專案時自動建立連結至Adobe Experience Manager Assets的資料夾

有了適用於Adobe Experience Manager整合的全新建立連結資料夾工作流程，您可以透過Adobe Experience Manager Assets資料夾的路徑設定整合。 將整合新增至專案範本時，從範本建立的任何專案都會在指定資料夾的Experience Manager Assets中自動建立連結的子資料夾。

以前，建立連結資料夾需要使用者執行動作。

此功能只能與Workfront內的Adobe Experience Manager as a Cloud Service整合搭配使用。 Adobe Experience Manager增強型聯結器不提供此功能。

如需詳細資訊，請參閱 [在Experience Manager Assets整合中使用工作流程](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## 將Workfront欄位值對應至Experience Manager Assets中的標籤

現在，您可以根據Workfront的資料進行分類並快速尋找資產。 您可以在Experience Manager Assets整合的Workfront中，將此資料對應為中繼資料設定的一部分。

之前，將Workfront資料對應至Experience Manager Assets標籤的功能無法使用。

如需Experience Manager Assetsas a Cloud Service中此功能的詳細資訊，請參閱 [設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
如需Experience Manager Assets Essentials中此功能的詳細資訊，請參閱 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 將Workfront欄位對應至自訂Experience Manager Assets中繼資料欄位

透過原生整合，您現在可以將原生和內建Workfront欄位對應到Experience Manager Assetsas a Cloud Service中的自訂中繼資料結構欄位。

如需Experience Manager Assetsas a Cloud Service中此功能的詳細資訊，請參閱 [設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
如需Experience Manager Assets Essentials中此功能的詳細資訊，請參閱 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 使用Adobe Workfront調整自動校樣工作流程範本設定以進行Creative Cloud

您現在可以直接在Creative Cloud中調整現有的自動化工作流程範本設定。 選擇現有的自動化工作流程範本後，您可以：

* 停用階段
* 新增其他收件者
* 變更校訂角色
* 調整期限
* 更新電子郵件通知
* 及更多內容！

如需詳細資訊，請參閱 [使用上傳檔案和校樣 [!DNL Adobe Workfront] 外掛程式 [!DNL Creative Cloud] 應用](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

這些增強功能適用於下列Creative Cloud應用程式：

* Photoshop
* XD
* InDesign
* Illustrator
