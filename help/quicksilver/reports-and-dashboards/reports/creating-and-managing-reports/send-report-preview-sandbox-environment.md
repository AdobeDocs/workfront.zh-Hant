---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在預覽Sandbox環境中傳送報告
description: 此頁面上的資訊指出僅在「預覽」和「自訂重新整理沙箱」環境中可用的功能。 生產環境中未提供此功能。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 在預覽Sandbox環境中傳送報告

此頁面上的資訊指出僅在「預覽」和「自訂重新整理沙箱」環境中可用的功能。 生產環境中未提供此功能。

您可以在任何Adobe Workfront測試環境中設定報表傳送選項。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

雖然測試環境的功能儘可能接近您的生產環境，但有些功能與您的生產環境不同。

您可以在測試環境中排程報表，但傳送方式與從生產環境傳送報表的方式不同。

如需生產環境中傳送排程報表的相關資訊，請參閱 [報表傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

根據您排程報告的位置，傳送功能在「預覽」和「自訂重新整理」沙箱中有所不同。

## 存取需求

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 在預覽環境中排程報表

* [在預覽環境中排程報表](#schedule-reports-in-the-preview-environment)

### 在預覽環境中排程報表

是否會在預覽環境中產生傳遞的報表，取決於是否 **接收來自此測試環境的電子郵件** 已啟用或未啟用。

如需有關從沙箱環境啟用電子郵件的資訊，請參閱 [啟用從預覽Sandbox環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在「預覽」環境中排程傳送的報告與在「生產」環境中排程報告相同。 如需排程報表傳送的詳細資訊，請參閱 [報表傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

當您在預覽環境中排程報表以進行傳送時，會出現下列情況：

* 時間 **接收來自此測試環境的電子郵件** 已針對接收報表的使用者停用，在排程報表傳送時不會產生檔案。
* 時間 **接收來自此測試環境的電子郵件** 會針對接收報告的使用者啟用，在排程報告傳送時產生的檔案會新增到使用者的檔案索引標籤中。

## 在自訂重新整理沙箱環境中排程報表

自訂重新整理沙箱中是否會產生傳遞的報表，取決於是否啟用從此測試環境接收電子郵件設定。

如需有關從預覽環境啟用電子郵件的資訊，請參閱區段 [檢視並修改您的電子郵件通知設定](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 在文章中 [修改您自己的電子郵件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在自訂重新整理沙箱環境中排程傳送的報告與在生產環境中排程報告相同。 如需排程報表傳送的詳細資訊，請參閱 [報表傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

當您排程報表以在「自訂重新整理沙箱」環境中傳送時，會出現下列情況：

* 當接收報告的使用者停用從此測試環境接收電子郵件時，排程傳送報告時不會產生任何檔案。
* 當對接收報告的使用者啟用從此測試環境接收電子郵件時，報告將作為與使用者關聯的電子郵件地址的附件以電子郵件形式傳送。

## 如何通知外部使用者

外部使用者不會收到從Workfront測試環境傳送的報告，也不會收到電子郵件通知。

只有從生產環境傳送報表時，外部使用者才會收到電子郵件報表。
