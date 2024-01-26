---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 安裝 [!DNL Adobe Workfront] 的 [!DNL Salesforce]
description: 若要在應用程式於 [!DNL Salesforce] AppExchange，請參閱安裝 [!DNL Workfront] 在Salesforce於AppExchange市集中可用之前使用。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: e823589247a2231e038142ae8d19f366769060e2
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# 安裝 [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>若要在應用程式於 [!DNL Salesforce AppExchange]，請參閱 [安裝 [!DNL Workfront for Salesforce] 在它於以下位置變得可用之前： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

作為 [!DNL Salesforce] 和 [!DNL Adobe Workfront] 管理員，您可以安裝 [!DNL Workfront for Salesforce] 允許您的 [!DNL Salesforce] 要提交的使用者 [!DNL Workfront] 要求並自動建立專案，無需離開Salesforce。

以取得安裝後的一般瞭解 [!DNL Workfront for Salesforce]，請參閱 [[!DNL Adobe Workfront for Salesforce] 概述](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [安裝及使用的先決條件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [安裝 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## 存取需求

您必須具有下列存取權才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL計畫]</p> </td> 
  </tr>  </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 安裝及使用的先決條件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必須擁有 [!DNL Salesforce] 具有系統管理員帳戶存取權的執行個體，以安裝應用程式。
* 您必須擁有 [!DNL Workfront] 具有系統管理員帳戶存取權的執行個體，以設定整合。
* [!UICONTROL Salesforce] 使用者必須擁有 [!DNL Workfront] 帳戶以便能夠：

   * 建立 [!DNL Workfront] 請求來源 [!DNL Salesforce]
   * 檢視 [!DNL Workfront] Salesforce中的請求或專案

## 安裝 [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

您必須是 [!DNL Salesforce] 和 [!DNL Workfront] 系統管理員以安裝和設定 [!DNL Workfront for Salesforce].

以下小節說明如何安裝 [!DNL Workfront] 針對您的 [!DNL Salesforce] 生產環境。 您可以依照相同的步驟進行安裝 [!DNL Workfront] 針對您的 [!DNL Salesforce] 沙箱環境。

* [安裝 [!DNL Workfront for Salesforce] 在它於以下位置變得可用之前： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Classic] 框架](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 安裝 [!DNL Workfront for Salesforce] 在它於以下位置變得可用之前： [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 將於以下位置提供： [!DNL Salesforce AppExchange] 即將推出。

若要在可用之前安裝應用程式：

1. 在您的生產環境中，前往

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   在您的沙箱環境中，前往

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >您必須登入Salesforce才能存取這些頁面。

1. 檢查 **[!UICONTROL 是，授與這些協力廠商網站的存取權]** 方塊。

   載入畫面隨即顯示。 安裝可能需要一些時間。

1. 按一下 **[!UICONTROL 完成]** 安裝完成時。

1. 瀏覽至 **[!UICONTROL 設定]** > **[!UICONTROL 安全性] 控制項** > **[!UICONTROL 遠端站台設定]**.
1. （視條件而定）從清單中選取Workfront 。

   或

   如果您沒有看到 [!DNL Workfront] URL列於 **[!UICONTROL 所有遠端站台]** 清單，按一下 **[!UICONTROL 新增遠端站台]**.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台名稱]**.

   例如， *[!DNL Workfront]*.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 按一下「**[!UICONTROL 儲存]**」。

   此 [!DNL Workfront] 應用程式現已安裝在您的 [!DNL Salesforce] 執行個體和 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的環境中建立頁面。

   [!DNL Salesforce] 一旦您新增 [!DNL Workfront] 區段至其 [!UICONTROL 商機] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需為使用者設定Workfront區段的詳細資訊，請參閱 [為Salesforce使用者設定Adobe Workfront區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安裝 [!DNL Workfront] 的 [!DNL Salesforce] 在 [!DNL Salesforce Classic] 框架

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 前往 **設定。**
1. 在 **建置** 區段，按一下 **AppExchange市集**.

1. 在 **搜尋AppExchange應用程式** 方塊，輸入 **Workfront**.

1. 找到時，請按一下Workfront應用程式，然後按一下 **立即取得**.
1. 按一下 **[!UICONTROL 在生產環境中安裝]** 安裝 [!DNL Workfront] 您的應用程式 [!DNL Salesforce] 生產環境。 （建議）
1. 閱讀並同意條款與條件後，請啟用 **[!UICONTROL 我已閱讀並同意條款及條件]** 欄位。
1. 按一下 **[!UICONTROL 確認並安裝]**.
1. 選取 **[!UICONTROL 為所有使用者安裝]** （建議），然後按一下 **[!UICONTROL 安裝]**.

1. （視條件而定）若系統詢問您是否要核准第三方存取權，您必須選取 **[!UICONTROL 是，授與這些協力廠商網站的存取權]**，然後按一下 **[!UICONTROL 繼續]**.

1. 按一下 **[!UICONTROL 完成]** 安裝完成時。

   此 [!DNL Workfront] 應用程式列於下 **[!UICONTROL 已安裝的封裝]**.


1. 瀏覽至 **[!UICONTROL 設定>安全性控制>遠端站台設定]**.
1. （視條件而定）如果您沒有看見 [!DNL Workfront] URL列於 **[!UICONTROL 所有遠端站台]** 清單，按一下 **[!UICONTROL 新增遠端站台]**.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台名稱]**.
例如， *[!DNL Workfront]*.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台URL]**.
例如， *yourDomain.my.workfront.com*.

1. 按一下「**[!UICONTROL 儲存]**」。\
   此 [!DNL Workfront] 應用程式現已安裝在您的 [!DNL Salesforce] 執行個體。 此 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的環境中建立頁面。\
   [!DNL Salesforce] 在您新增 [!DNL Workfront] 區段至其 [!UICONTROL 商機] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需有關設定的資訊 [!DNL Workfront] 區段若為使用者，請參閱 [設定 [!DNL Adobe Workfront] 「 」部分 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安裝 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 按一下 **[!UICONTROL 設定] 圖示**，然後按一下 **[!UICONTROL 設定]**.

1. 在 **[!UICONTROL 平台工具]** 區段，展開 **[!UICONTROL 應用程式].**

1. 按一下 **[!DNL AppExchange Marketplace]**.
1. 在 **[!UICONTROL 搜尋 [!DNL AppExchange] 應用程式]** 方塊，輸入 **[!DNL Workfront]**.

1. 找到時，請按一下Workfront應用程式，然後按一下 **立即取得**.
1. 按一下 **[!UICONTROL 開啟登入畫面]**.\
   您必須使用登入 [!DNL Workfront] 管理員帳戶 [!DNL Salesforce].

1. 按一下 **[!UICONTROL 允許]**.
1. 在 **[!UICONTROL 在此組織中安裝]** 方塊，按一下 **[!UICONTROL 請在此處安裝]** 以安裝 [!DNL Workfront] 在您的 [!DNL Salesforce] 生產環境。 （建議）

1. 閱讀並同意條款與條件後，請啟用 **[!UICONTROL 我已閱讀並同意條款及條件]** 欄位。
1. 按一下 **[!UICONTROL 確認並安裝]**.
1. 選取 **[!UICONTROL 為所有使用者安裝]** （建議），然後按一下 **[!UICONTROL 安裝]**.

1. （視條件而定）若系統詢問您是否要核准第三方存取權，您必須選取 **[!UICONTROL 是，授與這些協力廠商網站的存取權]**，然後按一下 **[!UICONTROL 繼續]**.

1. 按一下 **[!UICONTROL 完成]** 安裝完成時。

   此 [!DNL Workfront] 應用程式列於下 **[!UICONTROL 已安裝的封裝]**.

1. 瀏覽至 **[!UICONTROL 設定].**
1. 在 **[!UICONTROL 設定]** 區段，展開 **[!UICONTROL 安全性].**

1. 按一下 **[!UICONTROL 遠端站台設定]**.
1. （視條件而定）如果您沒有看見 [!DNL Workfront] URL列於 **[!UICONTROL 所有遠端站台]** 清單，按一下 **[!UICONTROL 新增遠端站台]**.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台名稱]**.
例如， *[!DNL Workfront]*.

1. （視條件而定）如果新增網站，請指定 **[!UICONTROL 遠端站台URL]**.
例如， *yourDomain.my.workfront.com*.

1. 按一下「**[!UICONTROL 儲存]**」。

   此 [!DNL Workfront] 應用程式現已安裝在您的 [!DNL Salesforce] 執行個體，以及 **[!DNL Workfront]** 元件現已新增至您的環境。

   [!UICONTROL Salesforce] 使用者可以使用 [!DNL Workfront] 新增後應用程式 [!DNL Workfront] 區段至其 [!UICONTROL 商機] 或 [!UICONTROL 帳戶] 頁面配置。\
   如需有關設定的資訊 [!DNL Workfront] 區段若為使用者，請參閱 [設定 [!DNL Adobe Workfront] 「 」部分 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
