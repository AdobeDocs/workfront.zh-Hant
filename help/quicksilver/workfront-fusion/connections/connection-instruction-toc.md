---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: connections-annd-webhooks
title: 在中建立連線 [!DNL Adobe Workfront Fusion]
description: 連線必須符合其所連線之應用程式或Web服務的API所設定的需求。 因此，設定連線的指示會因應用程式或Web服務而異。 本文可協助您識別並找出連線的指示 [!DNL Adobe Workfront Fusion] 至您選擇的應用程式或Web服務。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# 在中建立連線 [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

連線必須符合其所連線之應用程式或Web服務的API所設定的需求。 因此，設定連線的指示會因應用程式或Web服務而異。 本文可協助您識別並找出連線的指示 [!DNL Adobe Workfront Fusion] 至您選擇的應用程式或Web服務。

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
   <p>目前：否 [!DNL Workfront Fusion] 授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 計畫： [!DNL Workfront Fusion] 已包括在內。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 連線到不需要設定的應用程式或Web服務

在大多數情況下，您可以使用模組來建立連線，幾乎沒有或完全沒有額外資訊。 [!DNL Workfront Fusion] 會自動處理驗證。

如需有關建立連線的說明，而不需要特別考量，請參閱 [建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md).

## 連線至 [!DNL Microsoft] 應用程式或Web服務

大部分 [!DNL Microsoft] 中的應用程式 [!DNL Workfront Fusion] 可讓您建立不含額外資訊的連線。

建立連線時，下列情況需要額外的步驟：

* 使用 [!DNL Microsoft Dynamics 365] 模組。

  如需指示，請參閱 [[!DNL Microsoft Dynamics 365] 模組](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* 正在連線到 [!DNL Microsoft Graph API] 使用 [!UICONTROL HTTP] 模組

  如需指示，請參閱 [呼叫 [!DNL MS Graph REST API] 透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## 連線至 [!DNL Google] 應用程式或Web服務

連線至的程式 [!DNL Google] 應用程式可能會因類別而異 [!DNL Google] 您正在使用的帳戶。 此外， [!DNL Google] 當您連線到時，安全性措施可能需要額外的組態 [!DNL Workfront Fusion].

如需詳細資訊，請參閱：

* [連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂Oauth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 包含更新的安全性措施](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 需要其他設定的其他應用程式

下列應用程式未遵循的基本設定 [!DNL Workfront Fusion] 連線。 您可以在文章中找到針對該應用程式連線這些應用程式的指示。

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
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">連線 [!DNL Adobe Workfront] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">連線 [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">連線 [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] 模組</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">連線 [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">連線 [!DNL Azure DevOps] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">連線 [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">連線 [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] 模組</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">連線 [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">連線 [!DNL Datadog] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">連線 [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>電子郵件</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">將您的電子郵件連線到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[！UICONTROL電子郵件]模組</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">連線 [!DNL Gmail] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">連線 [!DNL Jira Cloud] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">連線 [!DNL Jira Server] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">連線 [!DNL MariaDB] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">連線 [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">正在連線 [!DNL Qualtrics] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">連線 [!DNL ServiceNow] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[！UICONTROL SFTP]模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">連線 [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">連線 [!DNL Split.io] 至 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] 模組</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>加寬</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">連線 [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] 模組</a></td> 
  </tr> 
 </tbody> 
</table>
