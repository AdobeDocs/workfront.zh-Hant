---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 提交 [!DNL Adobe Workfront] 請求 [!DNL Salesforce] 物件
description: 安裝後 [!DNL Adobe Workfront] for [!DNL Salesforce], you can submit [!DNL Workfront] 請求 [!DNL Salesforce] 機會和客戶。 Classic和Lightning Experience架構中都有此功能。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# 提交 [!DNL Adobe Workfront] 請求 [!DNL Salesforce] 物件

安裝後 [!DNL Adobe Workfront for Salesforce]，您可以提交 [!DNL Workfront] 請求 [!DNL Salesforce] 機會和客戶。 此功能存在於 [!DNL Classic] 和 [!DNL Lightning Experience] 框架。

## 存取需求

您必須具備下列存取權，才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 計劃*</p></td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 授權*</p></td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

提交 [!DNL Workfront] 來自 [!DNL Salesforce] 機會或帳戶確保您的環境中具有以下內容：

* 您的 [!DNL Workfront] 已安裝管理員 [!DNL Workfront for Salesforce].\
   有關安裝的詳細資訊 [!DNL Workfront for Salesforce]，請參閱 [安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的 [!DNL Workfront] 管理員已新增 [!DNL Workfront] 區段 [!UICONTROL 機會] 和 [!UICONTROL 帳戶] 頁面配置。\
   如需新增 [!DNL Workfront] 區段至頁面配置，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 您有 [!DNL Workfront] 帳戶，您可從 [!DNL Workfront] 部分。\
   登入後，您可以看到 [!UICONTROL 新請求] 標籤中，您可以開始輸入請求。

## 提交 [!DNL Workfront] 請求 [!DNL Salesforce]

1. 轉到Salesforce中的Opportunity或Account。
1. 前往 [!DNL Workfront] 區段。
1. 在 **[!UICONTROL 新請求]** 索引標籤，請在 **[!UICONTROL 選擇請求類型]** 下拉式功能表。

   您可以看到您有權存取的相同請求佇列，這些佇列在Workfront中皆會顯示。

1. 開始填寫請求的可用欄位。

   從 [!DNL Salesforce] 等同於在 [!DNL Workfront] 網頁應用程式。

   >[!NOTE]
   >
   >使用 [!DNL Workfront] 外掛程式 [!DNL Salesforce] 暫時不可用。

   繼續遵循 [建立和提交 [!DNL Adobe Workfront] 請求](../../manage-work/requests/create-requests/create-submit-requests.md).

1. 按一下 **[!UICONTROL 提交]**.

## 檢視 [!DNL Workfront] 請求

1. 轉到 [!DNL Salesforce].
1. 前往 **[!DNL Workfront]** 區段。

   >[!NOTE]
   >
   >視您的 [!DNL Workfront] 管理員已配置此部分，其名稱可能不同。

1. 選取 **[!UICONTROL 已提交請求]** 標籤。

   您可以在此頁簽中查看您或其他人從此Opportunity或帳戶提交的所有請求。在Web應用程式中提交到此請求隊列的請求不會顯示在 [!DNL Salesforce].

   >[!NOTE]
   >
   >提交到Web應用程式中此請求隊列的請求不會顯示在Salesforce中的此清單中。

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   您可以檢視下列已提交請求的相關資訊：

   * 請求名稱(在 [!UICONTROL 主旨] column)
   * 參考號碼
   * 請求類型
   * 狀態
   * 日期提交
   * 按名稱請求
   * 已分配給名稱\

      此資訊在 [!DNL Workfront]，此清單中也會更新。

1. （選用）按一下請求的名稱，以在中開啟 [!DNL Workfront].

1. （選用）按一下 **[!UICONTROL 前往[!DNL Salesforce]]** 訪問問題源自以下Workfront領域的Opportunity或Account :

   * 在 [!UICONTROL 詳細資料] 問題一節
   * 按一下「摘要」後，在清單中選取問題時，請在「摘要」面板中 [!UICONTROL 開啟摘要] ![](assets/summary-panel-icon.png) 的子菜單。
   * 在問題標題中，當 [!UICONTROL 整合] 欄位可用。 您的系統或群組管理員必須將 [!UICONTROL 整合] 欄位至您的「配置範本」，以檢視問題標題中的「移至Salesforce」連結。 如需詳細資訊，請參閱 [使用版面範本自訂物件標題](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >此 [!UICONTROL 轉到Salesforce] 連結可顯示給所有 [!DNL Workfront] 可檢視問題的使用者。 您必須有 [!DNL Salesforce] 帳戶，才能前往 [!DNL Salesforce] 記錄問題的機會或帳戶。
