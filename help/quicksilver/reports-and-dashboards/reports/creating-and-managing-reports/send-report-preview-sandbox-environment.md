---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在預覽Sandbox環境中傳送報告
description: 此頁面上的資訊指出僅在「預覽」和「自訂重新整理沙箱」環境中可用的功能。 生產環境中未提供此功能。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# 在預覽Sandbox環境中傳送報告

<!-- Audited: 11/2024 -->

此頁面上的資訊指出僅在「預覽」和「自訂重新整理沙箱」環境中可用的功能。 生產環境中未提供此功能。

您可以在任何Adobe Workfront測試環境中設定報表傳送選項。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

雖然測試環境的功能儘可能接近您的生產環境，但有些功能與您的生產環境不同。

您可以在測試環境中排程報表，但傳送方式與從生產環境傳送報表的方式不同。

如需有關在生產環境中排程傳送報告的資訊，請參閱[報告傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

根據您排程報告的位置，傳送功能在「預覽」和「自訂重新整理」沙箱中有所不同。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在預覽環境中排程報表

* [在預覽環境中排程報表](#schedule-reports-in-the-preview-environment)

### 在預覽環境中排程報表

是否在[預覽]環境中產生傳遞的報表，取決於&#x200B;**是否啟用從此測試環境接收電子郵件**。

如需有關啟用來自沙箱環境的電子郵件的資訊，請參閱[啟用來自預覽沙箱環境的電子郵件傳遞](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

![接收來自沙箱選項的電子郵件](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在「預覽」環境中排程傳送的報告與在「生產」環境中排程報告相同。 如需排程報表傳送的相關資訊，請參閱[報表傳送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

當您在預覽環境中排程報表以進行傳送時，會出現下列情況：

* 當&#x200B;**從此測試環境接收電子郵件**&#x200B;對接收報告的使用者停用時，排程傳送報告時不會產生任何檔案。
* 當針對接收報告的使用者啟用&#x200B;**接收來自此測試環境的電子郵件**&#x200B;時，排程傳送報告時產生的檔案會新增到使用者的[檔案]索引標籤中。

## 在自訂重新整理沙箱環境中排程報表

自訂重新整理沙箱中是否會產生傳遞的報表，取決於是否啟用從此測試環境接收電子郵件設定。

如需有關從預覽環境啟用電子郵件的資訊，請參閱[修改您自己的電子郵件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)一節中的[檢視並修改您的電子郵件通知設定](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view)。

![接收來自沙箱選項的電子郵件](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在自訂重新整理沙箱環境中排程傳送的報告與在生產環境中排程報告相同。 如需排程報表傳送的相關資訊，請參閱[報表傳送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

當您排程報表以在「自訂重新整理沙箱」環境中傳送時，會出現下列情況：

* 當接收報告的使用者停用從此測試環境接收電子郵件時，排程傳送報告時不會產生任何檔案。
* 當對接收報告的使用者啟用從此測試環境接收電子郵件時，報告將作為與使用者關聯的電子郵件地址的附件以電子郵件形式傳送。

## 如何通知外部使用者

外部使用者不會收到從Workfront測試環境傳送的報告，也不會收到電子郵件通知。

只有從生產環境傳送報表時，外部使用者才會收到電子郵件報表。
