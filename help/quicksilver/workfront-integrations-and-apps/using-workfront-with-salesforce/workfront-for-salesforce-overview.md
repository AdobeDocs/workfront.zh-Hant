---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 適用於Salesforce的Adobe Workfront概觀
description: 您可以為Salesforce安裝 [!DNL Adobe Workfront] ，以允許Salesforce使用者提交 [!DNL Workfront] 請求並自動建立專案，而不需要離開Salesforce。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce]總覽

需要[!UICONTROL Pro] [!DNL Workfront]計畫才能使用此功能。 如需各種可用計畫的詳細資訊，請參閱[[!DNL Workfront] 計畫。](https://business.adobe.com/products/workfront/pricing.html)

您可以安裝[!DNL Adobe Workfront for Salesforce]，讓您的[!DNL Salesforce]使用者提交[!DNL Workfront]要求並自動建立專案，而不需離開[!DNL Salesforce]。

作為[!DNL Workfront]管理員，您可以下載並設定[!DNL Workfront for Salesforce]。 然後，您可以將其與所有其他[!DNL Salesforce]使用者共用。

如需有關安裝[!DNL Workfront for Salesforce]的詳細資訊，請參閱[安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。\
如需有關為所有使用者設定[!DNL Salesforce]中的[!DNL Workfront]區段的詳細資訊，請參閱[為 [!DNL Salesforce] 使用者設定 [!DNL Adobe Workfront] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

## 存取需求

您必須具有下列存取權才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## [!DNL Workfront for Salesforce]

使用[!DNL Workfront for Salesforce]時，您可以執行下列動作：

* 在機會或帳戶中手動建立來自[!DNL Salesforce]的新[!DNL Workfront]要求。

  如需有關從[!DNL Salesforce]建立[!DNL Workfront]要求的詳細資訊，請參閱來自 [!DNL Salesforce] 物件](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)的[提交 [!DNL Adobe Workfront] 要求。

* 在[!DNL Salesforce]中符合某些條件時，自動觸發在[!DNL Workfront]中建立專案。 您的[!DNL Salesforce]系統管理員必須設定從[!DNL Salesforce]建立專案的觸發器。

  如需有關從[!DNL Salesforce]建立[!DNL Workfront]專案的詳細資訊，請參閱[從 [!DNL Salesforce] 物件建立 [!DNL Adobe Workfront] 專案](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

處理[!DNL Salesforce]的[!DNL Workfront]時，請考慮下列事項：

* 我們同時支援[!DNL Salesforce Classic]和[!DNL Lightning Experience]架構。
* 只能從[!DNL Salesforce]到[!DNL Workfront]建立專案。
* 您可以在[!DNL Salesforce]中檢視[!DNL Workfront]專案的部分相關資訊。

  無法自訂此資訊。

  如需可從[!DNL Salesforce]檢視的[!DNL Workfront]欄位清單，請參閱[提交來自 [!DNL Salesforce] 物件的 [!DNL Adobe Workfront] 要求](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)以及來自 [!DNL Salesforce] 物件的[建立 [!DNL Adobe Workfront] 專案](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

* 您可以按一下Workfront中的&#x200B;**[!UICONTROL 前往Salesforce]**&#x200B;連結，直接存取連結至[!DNL Salesforce]的專案。

  您無法檢視[!DNL Workfront]中[!DNL Salesforce]專案的任何相關資訊，但您擁有來自[!DNL Workfront]的[!UICONTROL Salesforce]專案連結，可在[!DNL Salesforce]中檢閱。

  [!UICONTROL 此&#x200B;**前往Salesforce**]&#x200B;連結會顯示在下列區域中：

   * 專案或和問題的[!UICONTROL 詳細資料]區段
   * 專案或問題的標頭。

     您的系統或群組管理員必須將[!UICONTROL 整合]欄位新增到您的版面配置範本，才能檢視專案或問題標題中的[!UICONTROL 前往Salesforce]連結。
   * 在清單的工具列中按一下[!UICONTROL 開啟摘要] ![摘要面板圖示](assets/summary-panel-icon.png)後，在清單中選取問題時的問題[!DNL Summary]面板。

     >[!NOTE]
     >
     >所有可以檢視專案或問題的[!DNL Workfront]使用者皆可看到[!UICONTROL 前往Salesforce]連結。 您必須擁有[!DNL Salesforce]帳戶才能移至記錄問題的[!DNL Salesforce]商機或帳戶。

* 更新一個應用程式中一個專案的欄位並不會更新另一個應用程式中連結專案的任何資訊。
