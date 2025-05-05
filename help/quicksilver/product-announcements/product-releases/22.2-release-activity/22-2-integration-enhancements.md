---
title: 22.2整合增強功能
description: 22.2整合增強功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2整合增強功能

本頁說明22.2版對預覽環境所做的所有整合增強功能。 這些增強功能將在生產環境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當週。

如需22.2版本可用的所有變更清單，請參閱[22.2版本概觀](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)。

## Adobe Workfront與Anaplan整合現已推出

為了讓您在Workfront專案的財務方面有更好的彈性和insight，Workfront現在可與您的Anaplan帳戶整合。 透過將Workfront物件連結至Anaplan物件，您可以自動更新兩個帳戶之間的資訊，確保兩個帳戶中的資訊都是最新且相同的。 您也可以根據Workfront中的動作在Anaplan中觸發自動化程式（反之亦然）。

例如，您可以在Anaplan中建立行銷活動，然後建立連結至行銷活動的Workfront專案或方案。 Workfront中追蹤的所有成本都可以上傳回Anaplan以審查行銷活動績效。

您可能考慮使用Workfront來Anaplan整合的其他工作流程包括：

* 從新的Workfront專案建立Anaplan預算請求
* 從新的Anaplan清單專案建立Workfront專案
* 從Workfront專案起始Anaplan供應商請求

如需詳細資訊，請參閱[具有Anaplan的Adobe Workfront](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md)。

## 適用於Experience Manager的Workfront增強型聯結器更新

適用於Experience Manager的Workfront增強型聯結器現在包含下列更新：

* 現在，即使有多個專案連結資料夾設定，您仍可以在Adobe Workfront和Adobe Experience Manager Assets as a Cloud Service之間建立連結資料夾。
* 新增對事件訂閱分頁的支援
* 新增對AEM 6.4.x的支援
* 新增對Proxy環境的支援
* 根據合作夥伴和客戶的意見回應進行多項錯誤修正

如需詳細資訊，請參閱[適用於Experience Manager的Workfront增強型聯結器總覽](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md)。

>[!NOTE]
>
>此聯結器的部署和設定需要經過認證的合作夥伴。 如需詳細資訊，請參閱[安裝Workfront for Experience Manager增強型聯結器](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install)。

## Adobe Creative Cloud整合現在使用OAuth2

為了提高安全性，也為了在整合間提供更一致的體驗，我們已更新Adobe Creative Cloud整合，以使用OAuth2驗證（驗證使用者的業界標準方式）。 現在，當您的使用者登入時，他們可以檢視整合有權存取的特定動作和區域，並允許存取。 之後，他們不需要如此頻繁地登入。

如需詳細資訊，請參閱[使用適用於Illustrator和InDesign的Workfront擴充功能](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md)。

## 檢視自訂OAuth2或JWT整合的使用者端密碼詳細資訊

為了讓您更透明地使用自訂OAuth2和JWT整合，我們讓您能夠檢視您的整合所使用使用者端密碼的詳細資訊。 現在，您可以檢視使用者端密碼的建立和上次使用日期。 您也可以新增並檢視您自己的使用者端密碼相關備註。

以前這些詳細資料無法使用。

如需有關OAuth2或JWT自訂整合中的使用者端密碼的詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 檢視自訂OAuth2應用程式清單中的驗證型別

現在，當您檢視組織中的自訂OAuth2應用程式清單時，您可以檢視每個應用程式是使用使用者驗證還是伺服器驗證。

之前，您只能前往每個應用程式上的編輯選項檢視此資訊。

如需詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 設定自訂OAuth2整合中重新整理權杖的有效期

為了更妥善地控制自訂OAuth2整合的存取和安全性，您現在可以自訂重新整理權杖的有效期限。 使用者的重新整理Token過期後，他們需要重新登入整合。

如需詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 在伺服器對伺服器應用程式的自訂OAuth2整合中使用公開和私密金鑰

您現在可以在自訂整合中設定伺服器對伺服器OAuth2應用程式。 透過設定公開和私密金鑰，您可以允許Workfront在不使用登入憑證的情況下與其他應用程式通訊。

以往，您的自訂OAuth2應用程式中的所有驗證都使用使用者的登入認證。

如需詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## Google Google Workspace整合現在使用OAuth2

為了提高安全性，也為了在整合間提供更一致的體驗，我們已更新Google Google Workspace整合，以使用OAuth2驗證（驗證使用者的業界標準方式）。 現在，當您的使用者登入時，他們可以檢視整合有權存取的特定動作和區域，並允許存取。 之後，他們不需要如此頻繁地登入。

如需詳細資訊，請參閱[登入和登出Google Workspace的Adobe Workfront](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md)。
