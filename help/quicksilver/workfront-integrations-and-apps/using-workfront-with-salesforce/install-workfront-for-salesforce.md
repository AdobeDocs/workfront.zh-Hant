---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 安裝 [!DNL Adobe Workfront] for [!DNL Salesforce]
description: 若要在應用程式可供使用前先行安裝，請在 [!DNL Salesforce] AppExchange，請參閱安裝 [!DNL Workfront] (在AppExchange市集中可用之前)。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# 安裝 [!DNL Adobe Workfront for Salesforce]

若要在應用程式可供使用前先行安裝，請在 [!DNL Salesforce AppExchange]，請參閱 [安裝 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] 和 [!DNL Adobe Workfront] 管理員，您可以安裝 [!DNL Workfront for Salesforce] 允許 [!DNL Salesforce] 提交使用者 [!DNL Workfront] 請求並自動建立專案，永遠不需要離開Salesforce。

了解安裝後您可預期的項目 [!DNL Workfront for Salesforce]，請參閱 [[!DNL Adobe Workfront for Salesforce] 概述](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [安裝和使用的必要條件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [安裝 [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

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
  </tr>  </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 安裝和使用的必要條件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必須有 [!DNL Salesforce] 具有系統管理員帳戶存取權以安裝應用程式的執行個體。
* 您必須有 [!DNL Workfront] 具有系統管理員帳戶存取權以設定整合的例項。
* [!UICONTROL Salesforce] 使用者必須 [!DNL Workfront] 帳戶

   * 建立 [!DNL Workfront] 請求 [!DNL Salesforce] 或
   * 檢視 [!DNL Workfront] 請求或專案。

## 安裝 [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

您必須是 [!DNL Salesforce] 和 [!DNL Workfront] 系統管理員安裝和配置 [!DNL Workfront for Salesforce].

以下小節說明如何安裝 [!DNL Workfront] 為 [!DNL Salesforce] 生產環境。 您可以依照相同的步驟進行安裝 [!DNL Workfront] 為 [!DNL Salesforce] 沙箱環境。

* [安裝 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Classic] 框架](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 安裝 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 將可在 [!DNL Salesforce AppExchange] 很快。

若要在應用程式可用之前先進行安裝：

1. 在您的生產環境中，前往

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

   在沙箱環境中，前往

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

1. 檢查 **[!UICONTROL 是，授予這些第三方網站的存取權]** 框。

   載入畫面隨即顯示，安裝可能需要一段時間。

1. 按一下 **[!UICONTROL 完成]** 安裝完成後。

1. 導覽至 **[!UICONTROL 「設定」>「安全控制」>「遠程站點設定」]**.
1. （視條件而定）如果您沒有看到 [!DNL Workfront] 列於 **[!UICONTROL 所有遠程站點]** 清單，按一下 **[!UICONTROL 新遠程站點]**.

1. 指定 **[!UICONTROL 遠程站點名稱]**.

   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 遠程站點URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   此 [!DNL Workfront] 應用程式現在已安裝在您的 [!DNL Salesforce] 例項和 **[!UICONTROL WorkfrontOpportunity]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 頁面已在您的環境中建立。

   [!DNL Salesforce] 新增 [!DNL Workfront] 區段 [!UICONTROL 機會] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需為使用者設定Workfront區段的相關資訊，請參閱 [為Salesforce使用者設定Adobe Workfront區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安裝 [!DNL Workfront] for [!DNL Salesforce] 在 [!DNL Salesforce Classic] 框架

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 前往 **設定。**
1. 在 **建置** ，按一下 **AppExchange市集**.

1. 在 **搜尋AppExchange應用程式** 框，類型 **Workfront**.

1. 找到應用程式時按一下，然後按一下 **立即獲取**.
1. 按一下 **[!UICONTROL 在生產環境中安裝]** 安裝 [!DNL Workfront] 應用程式 [!DNL Salesforce] 生產環境。 （建議）
1. 選取 **[!UICONTROL 我已閱讀並同意條款與條件]** 欄位（在您已閱讀並同意條款與條件後）。
1. 按一下 **[!UICONTROL 確認和安裝]**.
1. 選擇 **[!UICONTROL 為所有用戶安裝]** （建議），然後按一下 **[!UICONTROL 安裝]**.

1. （條件性）如果詢問您是否要核准協力廠商存取權，您必須選取 **[!UICONTROL 是，授予這些第三方網站的存取權]**，然後按一下 **[!UICONTROL 繼續]**.

1. 按一下 **[!UICONTROL 完成]** 安裝完成後。

   此 [!DNL Workfront] 「應用程式」列於 **[!UICONTROL 已安裝的軟體包]**.


1. 導覽至 **[!UICONTROL 「設定」>「安全控制」>「遠程站點設定」]**.
1. （視條件而定）如果您沒有看到 [!DNL Workfront] 列於 **[!UICONTROL 所有遠程站點]** 清單，按一下 **[!UICONTROL 新遠程站點]**.\

1. 指定 **[!UICONTROL 遠程站點名稱]**.\
   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 遠程站點URL]**.\
   例如， *yourDomain.my.workfront.com*.

1. 按一下&#x200B;**[!UICONTROL 儲存]**。\
   此 [!DNL Workfront] 應用程式現在已安裝在您的 [!DNL Salesforce] 例項和 **[!UICONTROL WorkfrontOpportunity]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 頁面已在您的環境中建立。\
   [!DNL Salesforce] 在您新增 [!DNL Workfront] 區段 [!UICONTROL 機會] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需設定 [!DNL Workfront] 區段，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 按一下 **[!UICONTROL 設定] 圖示**，然後按一下 **[!UICONTROL 設定]**.

1. 在 **[!UICONTROL 平台工具]** 區段，展開 **[!UICONTROL 應用程式].**

1. 按一下 **[!DNL AppExchange Marketplace]**.
1. 在 **[!UICONTROL 搜尋 [!DNL AppExchange] 應用程式]** 框，類型 **[!DNL Workfront]**.

1. 找到應用程式時按一下，然後按一下 **[!UICONTROL 立即獲取]**.
1. 按一下 **[!UICONTROL 開啟登入畫面]**.\
   您必須使用 [!DNL Workfront] 管理員帳戶 [!DNL Salesforce].

1. 按一下 **[!UICONTROL 允許]**.
1. 在 **[!UICONTROL 在此組織中安裝]** 按一下 **[!UICONTROL 在這裡安裝]** 安裝 [!DNL Workfront] 在 [!DNL Salesforce] 生產環境。 （建議）

1. 選取 **[!UICONTROL 我已閱讀並同意條款與條件]** 欄位（在您已閱讀並同意條款與條件後）。
1. 按一下 **[!UICONTROL 確認和安裝]**.
1. 選擇 **[!UICONTROL 為所有用戶安裝]** （建議），然後按一下 **[!UICONTROL 安裝]**.

1. （條件性）如果詢問您是否要核准協力廠商存取權，您必須選取 **[!UICONTROL 是，授予這些第三方網站的存取權]**，然後按一下 **[!UICONTROL 繼續]**.

1. 按一下 **[!UICONTROL 完成]** 安裝完成後。

   此 [!DNL Workfront] 「應用程式」列於 **[!UICONTROL 已安裝的軟體包]**.

1. 導覽至 **[!UICONTROL 設定].**
1. 在 **[!UICONTROL 設定]** 區段，展&#x200B;開&#x200B;**[!UICONTROL 安全性].**

1. 按一下 **[!UICONTROL 遠程站點設定]**.
1. （視條件而定）如果您沒有看到 [!DNL Workfront] 列於 **[!UICONTROL 所有遠程站點]** 清單，按一下 **[!UICONTROL 新遠程站點]**.

1. 指定 **[!UICONTROL 遠程站點名稱]**.

   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 遠程站點URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   此 [!DNL Workfront] 應用程式現在已安裝在您的 [!DNL Salesforce] 例項和 **[!DNL Workfront]** 元件現在已新增至您的環境。

   [!UICONTROL Salesforce] 使用者可使用 [!DNL Workfront] 新增應用程式後 [!DNL Workfront] 區段 [!UICONTROL 機會] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需設定 [!DNL Workfront] 區段，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
