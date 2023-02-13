---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在預覽沙箱環境中傳送報表
description: 此頁面上的資訊指的是只能在「預覽」和「自訂重新整理沙箱」環境中使用的功能。 此功能在生產環境中無法使用。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 在預覽沙箱環境中傳送報表

此頁面上的資訊指的是只能在「預覽」和「自訂重新整理沙箱」環境中使用的功能。 此功能在生產環境中無法使用。

您可以在任何Adobe Workfront測試環境中設定「報表傳送」選項。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

雖然測試環境的功能應盡可能接近您的生產環境，但有些功能與您的生產環境不同。

您可以在測試環境中排程報表，但其傳送方式與從生產環境傳送報表的方式不同。

如需在生產環境中排程報表以進行傳送的詳細資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

根據您排程報表的位置，「預覽」和「自訂重新整理」沙箱的傳送功能會有所不同。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在預覽環境中排程報表

* [在預覽環境中排程報表](#schedule-reports-in-the-preview-environment)

### 在預覽環境中排程報表

是否在預覽環境中產生傳送的報表，取決於 **從此測試環境接收電子郵件** 是否啟用。

如需從沙箱環境啟用電子郵件的相關資訊，請參閱 [啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在「預覽」環境中傳送的排程報表與在「生產」環境中排程報表相同。 如需排程報表傳送的相關資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

在「預覽」環境中排程要傳送的報表時，會出現下列情況：

* 當 **從此測試環境接收電子郵件** 如果接收報表的使用者已停用，則排程報表進行傳送時不會產生任何檔案。
* 當 **從此測試環境接收電子郵件** 會為接收報表的使用者啟用，排程報表傳送時產生的檔案會新增至使用者的「檔案」索引標籤中。

## 在自訂重新整理沙箱環境中排程報表

是否在自訂重新整理沙箱中產生傳送的報表，取決於是否啟用從此測試環境接收電子郵件設定。

如需從預覽環境啟用電子郵件的相關資訊，請參閱區段 [檢視及修改您的電子郵件通知設定](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 在文章中 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在「自訂重新整理沙箱」環境中傳送的排程報表，與在生產環境中排程報表相同。 如需排程報表傳送的相關資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

在「自訂重新整理沙箱」環境中排程要傳送的報表時，會發生下列情況：

* 當接收報表的使用者停用從此測試環境接收電子郵件時，排程報表傳送時不會產生任何檔案。
* 為接收報表的使用者啟用「從此測試環境接收電子郵件」時，報表會以電子郵件方式與使用者相關聯的電子郵件地址連結。

## 如何通知外部使用者

外部使用者不會收到從Workfront測試環境傳送的報表，也不會收到電子郵件通知。

只有從生產環境傳送的外部使用者會收到電子郵件報表。
