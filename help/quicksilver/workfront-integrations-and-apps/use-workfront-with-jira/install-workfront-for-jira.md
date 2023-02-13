---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 安裝 [!DNL Adobe Workfront] for [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront] for [!DNL Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# 安裝 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。

安裝附加元件後，您可以定義要建立的工作流程 [!DNL Jira] 自動發生 [!DNL Workfront] 工作項目隨即建立。 兩個應用程式中的項都會被連結，並且它們的某些資訊可以在兩個系統中自動更新。

中的所有使用者 [!DNL Workfront] 和 [!DNL Jira] 可從這項整合中獲益。 他們只需要系統的許可證，而不是兩個系統。

此附加元件適用於 [!UICONTROL 伺服器] 和 [!UICONTROL OnDemand] (或 [!UICONTROL 雲])版本 [!DNL Jira] 軟體。 此附加元件不適用於 [!DNL Data Center] 版本 [!DNL Jira] 軟體。

若需 [!DNL Jira] 版本 [!DNL Workfront for Jira] 目前支援，請參閱 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在Atlassian Marketplace

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 計劃</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 授權概述</a>*</td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取</p> <p>重要：建議您在 [!DNL Jira] 和 [!DNL Workfront] 以專用於此整合，而非使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 安裝 [!DNL Workfront] for [!DNL Jira]

安裝 [!DNL Workfront] for [!DNL Jira] OnDemand等同於在 [!DNL Jira] 伺服器實例。

您必須是 [!DNL Jira] 管理員以安裝 [!DNL Workfront] 附加元件。

如果您不是 [!DNL Jira] 管理員，您可以瀏覽 [!DNL Workfront] 附加元件並要求安裝。 您的要求會傳送至 [!DNL Jira] 管理員以進行核准和安裝。

有關請求在 [!DNL Jira] 應用程式，請參閱 [管理用戶對載入項的請求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

安裝 [!DNL Workfront for Jira]:

1. 登入 [!DNL Jira] as a [!DNL Jira] 管理員。
1. 尋找 **[!DNL Workfront for Jira]** 中的附加元件 [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. 按一下 **[!UICONTROL 現在就去]** 來安裝。

   安裝完成後，您可以登入 [!DNL Workfront] 從 [!DNL Jira] 和設定您的整合。
   [!DNL ]
如需詳細資訊，請參閱 [為Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 針對 [!DNL Jira Server] 安裝

>[!NOTE]
>
>這些要求不適用於 [!UICONTROL OnDemand] ([!UICONTROL 雲])版本 [!DNL Jira] 軟體。

雖然安裝 [!DNL Workfront] 兩個 [!DNL Jira] 環境類似，使用 [!DNL Jira Server] 安裝：

* 在中設定附加元件時 [!DNL Jira]，則 **[!DNL JIRA Base URL]** 欄位可能與您用來存取的URL不同 [!DNL Jira] 在您的私人伺服器上。 此 **[!DNL JIRA Base URL]** 必須是使用NAT或反向代理通訊協定連線至私人伺服器的公開存取位址，因此 [!DNL Workfront] 可以存取它以向您的伺服器提出請求。

* 您必須使用SSL加密，以保護 [!DNL Jira] 和 [!DNL Workfront]. 啟用SSL時，您必須擁有憑證授權機構的完整SSL憑證堆疊。 不支援自簽名證書。
* 您必須確保 [!DNL jira.workfront.com] 可從公司伺服器存取網域。 它可作為 [!DNL Workfront] 和 [!DNL Jira] 和是該附加元件運作的必要條件。

   您也必須將下列靜態IP位址新增至防火牆上，以供傳出和傳入連線使用的允許清單。

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   有關配置防火牆以實現最佳功能的詳細資訊，請使用 [!DNL Workfront]，請參閱 [配置防火牆](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
