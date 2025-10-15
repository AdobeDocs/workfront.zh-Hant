---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 適用於Salesforce的Adobe Workfront概觀
description: 您可以為Salesforce安裝 [!DNL Adobe Workfront] ，以允許Salesforce使用者提交 [!DNL Workfront] 請求並自動建立專案，而不需要離開Salesforce。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 概覽

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Salesforce整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>為了滿足貴組織與Salesforce的整合需求，我們建議您使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Salesforce之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Salesforce模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

您可以安裝[!DNL Adobe Workfront for Salesforce]，讓您的[!DNL Salesforce]使用者提交[!DNL Workfront]要求並自動建立專案，而不需離開[!DNL Salesforce]。

作為[!DNL Workfront]管理員，您可以下載並設定[!DNL Workfront for Salesforce]。 然後，您就可以與所有其他[!DNL Salesforce]使用者共用它。

如需有關安裝[!DNL Workfront for Salesforce]的詳細資訊，請參閱[安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

如需有關為所有使用者設定[!DNL Workfront]中的[!DNL Salesforce]區段的詳細資訊，請參閱[為 [!DNL Adobe Workfront] 使用者設定 [!DNL Salesforce] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>規劃</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## [!DNL Workfront for Salesforce]

使用[!DNL Workfront for Salesforce]時，您可以執行下列動作：

* 在機會或帳戶中手動建立來自[!DNL Workfront]的新[!DNL Salesforce]要求。

  如需詳細資訊，請參閱來自[物件 [!DNL Adobe Workfront] 的 [!DNL Salesforce] 提交](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)要求。

* 在[!DNL Workfront]中符合某些條件時，自動觸發在[!DNL Salesforce]中建立專案。 您的[!DNL Salesforce]系統管理員必須設定從[!DNL Salesforce]建立專案的觸發器。

  如需有關從[!DNL Workfront]建立[!DNL Salesforce]專案的詳細資訊，請參閱[從 [!DNL Adobe Workfront] 物件建立 [!DNL Salesforce] 專案](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

處理[!DNL Workfront]的[!DNL Salesforce]時，請考慮下列事項：

* 我們同時支援[!DNL Salesforce Classic]和[!DNL Lightning Experience]架構。
* 只能建立從[!DNL Salesforce]到[!DNL Workfront]的專案。
* 您可以在[!DNL Workfront]中檢視[!DNL Salesforce]專案的部分相關資訊。 無法自訂此資訊。

  如需可從[!DNL Workfront]檢視的[!DNL Salesforce]欄位清單，請參閱[提交來自 [!DNL Adobe Workfront] 物件的 [!DNL Salesforce] 要求](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)以及來自[物件的 [!DNL Adobe Workfront] 建立 [!DNL Salesforce] 專案](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

* 您可以按一下Workfront中的[!DNL Salesforce]前往Salesforce[!UICONTROL 連結，直接存取連結至]的專案。

  您無法在[!DNL Salesforce]中檢視[!DNL Workfront]專案的任何相關資訊，但Workfront中有一個連結，可帶您前往Salesforce中的專案，讓您在該處檢閱該專案。

  [!UICONTROL 前往Salesforce]連結會顯示在下列區域：

   * 專案或問題的[!UICONTROL 詳細資料]區段。
   * 專案或問題的標頭。

     您的系統或群組管理員必須將[!UICONTROL 整合]欄位新增到您的版面配置範本，才能檢視專案或問題標題中的[!UICONTROL 前往Salesforce]連結。
   * 在清單的工具列中按一下[!DNL Summary]開啟摘要摘要面板圖示![後，在清單中選取問題時的問題](assets/summary-panel-icon.png)面板。

     >[!NOTE]
     >
     >所有可以檢視專案或問題的[!UICONTROL 使用者皆可看到]前往Salesforce[!DNL Workfront]連結。 您必須擁有[!DNL Salesforce]帳戶才能移至記錄問題的[!DNL Salesforce]商機或帳戶。

* 更新一個應用程式中一個專案的欄位並不會更新另一個應用程式中連結專案的任何資訊。
