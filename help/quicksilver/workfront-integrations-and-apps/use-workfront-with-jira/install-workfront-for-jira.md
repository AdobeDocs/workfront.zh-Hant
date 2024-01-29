---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 安裝 [!DNL Adobe Workfront] 的 [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront] 的 [!DNL Jira] 若要整合您的 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: b98a7fa48e60f1f2c2ea938b14b88e0c5a2ee418
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 安裝 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 若要整合您的 [!DNL Jira] 和 [!DNL Workfront] 系統。

安裝附加元件後，您可以定義要建立的工作流程 [!DNL Jira] 發生以下情況時自動問題： [!DNL Workfront] 工作專案已建立。 兩個應用程式中的專案會連結，而且其部分資訊可在兩個系統中自動更新。

中的所有使用者 [!DNL Workfront] 和 [!DNL Jira] 可受惠於這項整合。 他們只需要最常使用的系統授權，而不需要兩個系統的授權。

此附加元件適用於 [!UICONTROL 伺服器] 和 [!UICONTROL 隨選] (或 [!UICONTROL 雲端])個版本的 [!DNL Jira] 軟體。 此附加元件不適用於 [!DNL Data Center] 版本 [!DNL Jira] 軟體。

針對清單 [!DNL Jira] 版本為 [!DNL Workfront for Jira] 目前支援，請參閱 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在Atlassian Marketplace。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> 
   <p>新增：任何</p>
   <p>目前： [！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] 授權總覽</td> 
   <td> 
   <p>新增：標準</p>
   <p>目前： [！UICONTROL計畫]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在中建立個別的系統管理員帳戶 [!DNL Jira] 和 [!DNL Workfront] 以專門用於此整合，而不使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>您必須是 [!DNL Workfront] 管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 安裝 [!DNL Workfront] 的 [!DNL Jira]

安裝 [!DNL Workfront] 的 [!DNL Jira] OnDemand等同於在 [!DNL Jira] 伺服器例項。

您必須是 [!DNL Jira] 管理員以安裝 [!DNL Workfront] 附加元件。

如果您不是 [!DNL Jira] 管理員，您可以瀏覽 [!DNL Workfront] 附加元件並要求安裝。 您的請求會傳送至 [!DNL Jira] 管理員核准與安裝。

如需關於要求將附加元件安裝在您的電腦上的詳細資訊， [!DNL Jira] 應用程式，請參閱 [管理附加元件的使用者請求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

若要安裝 [!DNL Workfront for Jira]：

1. 登入 [!DNL Jira] as a [!DNL Jira] 管理員。
1. 尋找 **[!DNL Workfront for Jira]** 中的附加元件 [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. 按一下 **[!UICONTROL 立即取得]** 以安裝。

   安裝完成後，您可以登入 [!DNL Workfront] 從 [!DNL Jira] 並設定您的整合。

   如需詳細資訊，請參閱 [設定Jira適用的Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 的考量事項 [!DNL Jira Server] 安裝

>[!NOTE]
>
>這些要求不適用於 [!UICONTROL 隨選] ([!UICONTROL 雲端])版本 [!DNL Jira] 軟體。

雖然已安裝 [!DNL Workfront] 兩個中的附加元件 [!DNL Jira] 環境類似，使用時必須考慮以下事項 [!DNL Jira Server] 安裝：

* 在中設定附加元件時 [!DNL Jira]，中指定的位址 **[!DNL JIRA Base URL]** 欄位可能與您用來存取的URL不同 [!DNL Jira] 私人伺服器上。 此 **[!DNL JIRA Base URL]** 必須是可公開存取的位址，且必須使用NAT或反向Proxy通訊協定連線至您的私人伺服器，因此 [!DNL Workfront] 可以存取該檔案以向伺服器提出要求。

* 您必須使用SSL加密來保護兩者之間的通訊 [!DNL Jira] 和 [!DNL Workfront]. 啟用SSL時，您必須擁有來自憑證授權單位的完整SSL憑證棧疊。 我們不支援自我簽署憑證。
* 您必須確保 [!DNL jira.workfront.com] 網域可從您的公司伺服器存取。 它是介於兩者之間的中介軟體環境 [!DNL Workfront] 和 [!DNL Jira] 且是附加元件運作的必要專案。

  您還必須將下列靜態IP位址新增至防火牆上的允許清單，以進行輸出和輸入連線。

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  如需有關設定防火牆以發揮最佳功能的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [設定防火牆](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
