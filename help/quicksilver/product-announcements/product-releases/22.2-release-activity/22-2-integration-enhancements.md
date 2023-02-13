---
title: 22.2整合增強功能
description: 22.2整合增強功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 22.2整合增強功能

本頁說明在「預覽」環境中22.2版所進行的所有整合增強功能。 這些增強功能將可在生產環境中使用

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當周。

如需22.2版所有可用變更的清單，請參閱 [22.2版本概觀](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront與Anaplan整合現已推出

為了讓您對Workfront專案的財務層面有更高的彈性和洞察力，Workfront現在可以與您的Anaplan帳戶整合。 通過將Workfront對象連結到Anaplan對象，可以自動更新兩個帳戶之間的資訊，確保這兩個帳戶中的資訊都是最新的且相同的。 您也可以根據Workfront中的動作，在Anaplan中觸發自動化流程（反之亦然）。

例如，您可以在Anaplan中建立促銷活動，然後建立連結至促銷活動的Workfront專案或方案。 接著，在Workfront中追蹤的任何成本都可上傳回Anaplan以檢閱促銷活動績效。

您可考慮使用Workfront以Anaplan整合的其他工作流程包括：

* 從新的Workfront專案建立Anaplan預算請求
* 從新的Anaplan清單項建立Workfront項目
* 從Workfront項目起動Anaplan供應商請求

如需詳細資訊，請參閱 [Adobe Workfront與阿納普蘭](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront for Experience Manager增強連接器更新

Workfront for Experience Manager增強連接器現在包含下列更新：

* 您現在可以在Adobe Workfront和Adobe Experience Manager Assets之間建立as a Cloud Service的連結資料夾，即使有多個專案連結資料夾設定亦然。
* 新增事件訂閱分頁支援
* 新增對AEM 6.4.x的支援
* 新增對Proxy環境的支援
* 根據合作夥伴和客戶意見的數個錯誤修正

如需詳細資訊，請參閱 [Workfront for Experience Manager增強連接器概觀](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>此連接器的部署和配置需要經過認證的合作夥伴。 請參閱 [安裝Workfront for Experience Manager增強連接器](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) 以取得更多資訊。

## Adobe Creative Cloud整合現已使用OAuth2

為獲得更高的安全性，並在整合之間提供更一致的體驗，我們已更新Adobe Creative Cloud整合，以使用OAuth2驗證，這是驗證使用者的業界標準方式。 現在，當您的使用者登入時，他們可以看到整合功能可存取及允許存取的特定動作和區域。 之後，使用者就不需要以同樣頻率登入。

如需詳細資訊，請參閱 [使用適用於Illustrator的Workfront擴充功能和InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## 請參閱自訂OAuth2或JWT整合的用戶端密碼詳細資訊

為了透明地使用您的自訂OAuth2和JWT整合，我們讓您能夠查看您整合使用之用戶端密碼的詳細資訊。 現在，您可以查看用戶端密碼的建立和上次使用日期。 您也可以新增及檢視自己有關用戶端密碼的附註。

以前，無法取得這些詳細資訊。

如需OAuth2或JWT自訂整合中用戶端密碼的詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 請參閱自訂OAuth2應用程式清單中的驗證類型

現在，當您檢視組織中的自訂OAuth2應用程式清單時，可以查看每個應用程式是使用使用者驗證還是伺服器驗證。

以前，您只能前往每個應用程式的編輯選項，才能查看此資訊。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 在您的自訂OAuth2整合中，為重新整理Token設定到期日

為了更妥善地控制自訂OAuth2整合的存取權和安全性，您現在可以自訂重新整理Token的有效期限。 使用者的重新整理Token過期後，就必須重新登入整合。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 在自訂OAuth2整合中，針對伺服器對伺服器應用程式使用公開和私密金鑰

您現在可以在自訂整合中設定伺服器對伺服器OAuth2應用程式。 透過設定公開金鑰和私密金鑰，您可讓Workfront不使用登入憑證與其他應用程式通訊。

之前，您自訂OAuth2應用程式中的所有驗證都使用使用者的登入憑證。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Google G套裝整合現在使用OAuth2

為提升安全性，並在整合之間提供更一致的體驗，我們已更新Google G Suite整合，以使用OAuth2驗證，此為驗證使用者的業界標準方式。 現在，當您的使用者登入時，他們可以看到整合功能可存取及允許存取的特定動作和區域。 之後，使用者就不需要以同樣頻率登入。

如需詳細資訊，請參閱 [登入和登出G Suite適用的Adobe Workfront](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
