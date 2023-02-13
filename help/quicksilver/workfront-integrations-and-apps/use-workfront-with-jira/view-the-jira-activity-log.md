---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 查看Jira活動日誌
description: As a [!DNL Jira] 管理員，您可以查看在同步或建立票證之間發生的異常和錯誤 [!DNL Adobe Workfront] 和 [!DNL Jira] 在活動記錄中。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 檢視 [!UICONTROL [!DNL Jira] 活動記錄]

As a [!DNL Jira] 管理員，您可以查看在同步或建立票證之間發生的異常和錯誤 [!DNL Adobe Workfront] 和 [!DNL Jira] 在 [!UICONTROL 活動記錄].

您可以在活動記錄中看到最多500個項目，並從最近的項目開始列出。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

## 必要條件

在您可以連結項目之間之前 [!DNL Workfront] 和 [!DNL Jira]，您必須

* 安裝 [!DNL Workfront for Jira]

   安裝說明 [!DNL Workfront for Jira]，請參閱 [安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 存取 [!UICONTROL [!DNL Jira] 活動記錄]:

1. 以系統管理員身分登入Jira。
1. 按一下 **[!UICONTROL 設定]** 在 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後 **[!UICONTROL 管理附加元件]**.

1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 登入 [!DNL Workfront] 作為系統管理員。
1. 選取 **[!UICONTROL 活動記錄]** 標籤。

   查看在建立項目或同步兩個應用程式之間的欄位期間發生的異常和錯誤的資訊。

   記錄檔包含下列欄位：

   * 發生日期
   * Jira中的用戶名
   * Jira問題編號
   * 發生錯誤的簡短說明。
