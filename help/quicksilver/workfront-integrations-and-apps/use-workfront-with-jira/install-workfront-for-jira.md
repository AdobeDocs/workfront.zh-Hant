---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 為 [!DNL Adobe Workfront] 安裝 [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront]  for [!DNL Jira] 來整合 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# 安裝[!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Jira整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>根據貴組織與Jira的整合需求，我們建議使用Workfront自動化和整合。
>
>8月前，我們將提供8個適用於Jira且現成可用的Workfront自動化和整合範本，以協助複製常見的工作流程並加速實作。 範本是完全可自訂的，可滿足特定的業務需求，且可隨著需求的發展而擴充。
> 
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Jira的Workfront自動化與整合模組特定功能的相關資訊，請參閱[Jira軟體模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

您可以使用[!DNL Adobe Workfront for Jira]來整合您的[!DNL Jira]和[!DNL Workfront]系統。

安裝附加元件後，您可以在建立[!DNL Jira]個工作專案時，定義自動建立[!DNL Workfront]問題的工作流程。 兩個應用程式中的專案會連結，而且其部分資訊可在兩個系統中自動更新。

[!DNL Workfront]和[!DNL Jira]中的所有使用者都可以受益於這項整合。 他們只需要最常使用的系統授權，而不需要兩個系統的授權。

此附加元件適用於[!UICONTROL 軟體的]伺服器[!UICONTROL 和]OnDemand[!UICONTROL &#x200B; （或]雲端[!DNL Jira]）版本。 此附加元件不適用於[!DNL Data Center]軟體的[!DNL Jira]版本。

如需[!DNL Jira]目前支援的[!DNL Workfront for Jira]版本清單，請參閱Atlassian Marketplace上的[[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> 
   <p>新增：任何</p>
   <p>目前： [!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront]授權總覽</td> 
   <td> 
   <p>新增：標準</p>
   <p>目前： [!UICONTROL 計畫]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在[!DNL Jira]和[!DNL Workfront]中建立個別的系統管理員帳戶以專用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>您必須是[!DNL Workfront]管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 安裝[!DNL Workfront]的[!DNL Jira]

為[!DNL Workfront] OnDemand安裝[!DNL Jira]與在[!DNL Jira]伺服器執行個體上安裝它相同。

您必須是[!DNL Jira]管理員才能安裝[!DNL Workfront]附加元件。

如果您不是[!DNL Jira]管理員，可以瀏覽[!DNL Workfront]附加元件並要求安裝。 您的要求已傳送給[!DNL Jira]管理員進行核准和安裝。

如需有關要求在[!DNL Jira]應用程式上安裝附加元件的詳細資訊，請參閱[管理附加元件的使用者要求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

若要安裝[!DNL Workfront for Jira]：

1. 以[!DNL Jira]管理員身分登入[!DNL Jira]。
1. 在&#x200B;**[!DNL Workfront for Jira]**&#x200B;[[!DNL Atlassian Marketplace]&#x200B;中尋找](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)附加元件。

1. 按一下&#x200B;**[!UICONTROL 立即取得]**&#x200B;以進行安裝。

   安裝完成後，您可以從[!DNL Workfront]登入[!DNL Jira]並設定整合。

   如需詳細資訊，請參閱[設定Jira的Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## [!DNL Jira Server]安裝的注意事項

>[!NOTE]
>
>這些需求不適用於[!UICONTROL 軟體的]OnDemand[!UICONTROL &#x200B; （]雲端[!DNL Jira]）版本。

雖然在兩個[!DNL Workfront]環境中安裝[!DNL Jira]附加元件類似，但使用[!DNL Jira Server]安裝時必須考慮下列事項：

* 在[!DNL Jira]中設定附加元件時，**[!DNL JIRA Base URL]**&#x200B;欄位中指定的位址可能與您在私人伺服器上用來存取[!DNL Jira]的URL不同。 **[!DNL JIRA Base URL]**&#x200B;必須是使用NAT或反向Proxy通訊協定連線到您的私人伺服器的可公開存取位址，因此[!DNL Workfront]可以存取它以向您的伺服器提出要求。

* 您必須使用SSL加密來保護[!DNL Jira]與[!DNL Workfront]之間的通訊。 啟用SSL時，您必須擁有來自憑證授權單位的完整SSL憑證棧疊。 我們不支援自我簽署憑證。
* 您必須確定可從您的公司伺服器存取[!DNL jira.workfront.com]網域。 它是介於[!DNL Workfront]和[!DNL Jira]之間的中介環境，是附加元件運作所需。

  您還必須將下列靜態IP位址新增至防火牆上的允許清單，以進行輸出和輸入連線。

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  如需有關設定防火牆以使用[!DNL Workfront]發揮最佳功能的詳細資訊，請參閱[設定防火牆](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
