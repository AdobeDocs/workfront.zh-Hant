---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: connections-annd-webhooks
title: 在 [!DNL Adobe Workfront Fusion]中建立連線
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# 在[!DNL Adobe Workfront Fusion]中建立連線

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [連線到應用程式：發行項索引](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-apps-toc.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

<!-- Audited: 3/2024-->

連線必須符合其所連線之應用程式或Web服務的API所設定的需求。 因此，設定連線的指示會因應用程式或Web服務而異。 本文可協助您識別並找出將[!DNL Adobe Workfront Fusion]連線至您所選應用程式或Web服務的指示。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td>  
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>  
   <td> 
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 連線到不需要設定的應用程式或Web服務

在大多數情況下，您可以使用模組來建立連線，幾乎沒有或完全沒有額外資訊。 [!DNL Workfront Fusion]會自動處理驗證。

如需建立連線的說明，不需特別考量，請參閱[建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明](../../workfront-fusion/connections/connect-to-fusion-general.md)。

## 連線至[!DNL Microsoft]應用程式或Web服務

[!DNL Workfront Fusion]中的大部分[!DNL Microsoft]應用程式可讓您建立連線，而不需要額外的資訊。

建立連線時，下列情況需要額外的步驟：

* 使用[!DNL Microsoft Dynamics 365]模組。

  如需指示，請參閱[[!DNL Microsoft Dynamics 365] 模組](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)。

* 使用[!UICONTROL HTTP]模組連線至[!DNL Microsoft Graph API]

  如需指示，請參閱[透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 發出OAuth 2.0要求]模組](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md)來呼叫 [!DNL MS Graph REST API] 。

## 連線至[!DNL Google]應用程式或Web服務

連線至[!DNL Google]應用程式的程式可能會因您使用的[!DNL Google]帳戶型別而有所不同。 此外，當您連線到[!DNL Workfront Fusion]時，[!DNL Google]安全性措施可能需要額外的設定。

如需詳細資訊，請參閱：

* [使用自訂OAuth使用者端連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] ](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [使用更新的安全性措施連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] ](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 需要其他設定的其他應用程式

下列App不遵循[!DNL Workfront Fusion]連線的基本設定。 您可以在文章中找到針對該應用程式連線這些應用程式的指示。

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>應用程式/網頁服務</th> 
   <th>關於連線的其他資訊</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront]模組</a>中將[!DNL Adobe Workfront]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia]模組</a>中將[!DNL Allocadia]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan]模組</a>中將[!DNL Anaplan]連線到[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3]模組</a>中將[!DNL AWS]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps]模組</a>中將[!DNL Azure DevOps]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder]模組</a>中將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert]模組</a>中將[!DNL CloudConvert]連線到[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent]模組</a>中將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog]模組</a>中將[!DNL Datadog]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign]模組</a>中將[!DNL DocuSign]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>電子郵件</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[！UICONTROL Email]模組中，將您的電子郵件連線至</a>[!DNL Workfront Fusion]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail]模組</a>中將[!DNL Gmail]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]模組</a>中將[!DNL Jira Cloud]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]模組</a>中將[!DNL Jira Server]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB]模組</a>中將[!DNL MariaDB]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo]模組</a>中將[!DNL Marketo]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365]模組</a>中將[!DNL Microsoft Dynamics 365]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">正在將[!DNL Qualtrics]連線到<a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics]模組中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow]模組</a>中將[!DNL ServiceNow]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[！UICONTROL SFTP]模組</a>中將SFTP連線至[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint]模組</a>中將[!DNL SharePoint]連線到[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io]模組</a>中將[!DNL Split.io]連線到[!DNL Workfront Fusion] </a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>加寬</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">在<a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen]模組</a>中將[!DNL Widen]連線到[!DNL Workfront Fusion] </a></td> 
  </tr> 
 </tbody> 
</table>
