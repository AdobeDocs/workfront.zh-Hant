---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce概觀
description: 您可以安裝 [!DNL Adobe Workfront] 讓Salesforce允許您的Salesforce使用者提交 [!DNL Workfront] 請求並自動建立專案，永遠不需要離開Salesforce。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 概述

A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要計畫。 如需各種可用計畫的詳細資訊，請參閱 [[!DNL Workfront] 計畫。](https://www.workfront.com/plans)

您可以安裝 [!DNL Adobe Workfront for Salesforce] 允許 [!DNL Salesforce] 提交使用者 [!DNL Workfront] 請求並自動建立專案，無需離開 [!DNL Salesforce].

As a [!DNL Workfront] 管理員，您可以 [!DNL Workfront for Salesforce]. 然後，您可以共用其他 [!DNL Salesforce] 使用者。

有關安裝的詳細資訊 [!DNL Workfront for Salesforce]，請參閱 [安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
如需有關設定 [!DNL Workfront] 區段 [!DNL Salesforce] 對於所有用戶，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## 存取需求

您必須具備下列存取權，才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## [!DNL Workfront for Salesforce]

使用 [!DNL Workfront for Salesforce]:

* 手動建立新 [!DNL Workfront] 請求 [!DNL Salesforce] 在Opportunity或Account中。

   如需有關建立 [!DNL Workfront] 請求 [!DNL Salesforce]，請參閱 [提交 [!DNL Adobe Workfront] 請求 [!DNL Salesforce] 物件](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* 自動觸發在中建立專案 [!DNL Workfront] 當符合特定條件時 [!DNL Salesforce]. 您的 [!DNL Salesforce] 系統管理員必須配置觸發器以從 [!DNL Salesforce].

   如需有關建立 [!DNL Workfront] 項目來源 [!DNL Salesforce]，請參閱 [建立 [!DNL Adobe Workfront] 項目來源 [!DNL Salesforce] 物件](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

使用時請考量下列事項 [!DNL Workfront] for [!DNL Salesforce]:

* 我們支援 [!DNL Salesforce Classic] 和 [!DNL Lightning Experience] 框架。
* 項目只能從 [!DNL Salesforce] 在 [!DNL Workfront].
* 您可以檢視 [!DNL Workfront] 項目 [!DNL Salesforce].

   無法自訂此資訊。

   若需 [!DNL Workfront] 欄位 [!DNL Salesforce]，請參閱  [提交 [!DNL Adobe Workfront] 請求 [!DNL Salesforce] 物件](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  和 [建立 [!DNL Adobe Workfront] 項目來源 [!DNL Salesforce] 物件](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* 您可以直接存取連結至的項目 [!DNL Salesforce] 按一下 **[!UICONTROL 轉到Salesforce]** 連結至Workfront。

   您無法檢視 [!DNL Salesforce] 項目 [!DNL Workfront]，但您有 [!UICONTROL Salesforce] 項目自 [!DNL Workfront] 查看 [!DNL Salesforce].

   [!UICONTROL 此 **轉到Salesforce**] 連結會顯示在下列區域：

   * 此 [!UICONTROL 詳細資料] 項目或問題部分
   * 專案或問題的標題。

      您的系統或群組管理員必須將 [!UICONTROL 整合] 欄位以檢視版面範本 [!UICONTROL 轉到Salesforce] 項目或問題標題中的連結。
   * 此 [!DNL Summary] 按一下 [!UICONTROL 開啟摘要] ![](assets/summary-panel-icon.png) 的子菜單。

      >[!NOTE]
      >
      >此 [!UICONTROL 轉到Salesforce] 連結可顯示給所有 [!DNL Workfront] 可檢視專案或問題的使用者。 您必須有 [!DNL Salesforce] 帳戶，才能前往 [!DNL Salesforce] 記錄問題的機會或帳戶。

* 更新一個應用程式中某個項目的欄位時，不會更新另一個應用程式中連結項目的任何資訊。
