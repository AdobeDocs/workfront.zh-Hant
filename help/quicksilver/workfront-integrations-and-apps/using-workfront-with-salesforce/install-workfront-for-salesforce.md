---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 為 [!DNL Salesforce]安裝 [!DNL Adobe Workfront]
description: 若要在 [!DNL Salesforce] AppExchange提供應用程式之前安裝應用程式，請參閱在AppExchange市集中提供應用程式之前安裝Salesforce適用的 [!DNL Workfront] 。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: b088c305cbd16aea1b6b79a9f3a9c5ac326cd0b8
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# 安裝[!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>若要在[!DNL Salesforce AppExchange]提供應用程式之前安裝應用程式，請參閱[在 [!DNL AppExchange] 市集](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)提供應用程式之前安裝 [!DNL Workfront for Salesforce] 。

身為[!DNL Salesforce]和[!DNL Adobe Workfront]管理員，您可以安裝[!DNL Workfront for Salesforce]，讓您的[!DNL Salesforce]使用者提交[!DNL Workfront]請求並自動建立專案，而不需要離開Salesforce。

如需安裝[!DNL Workfront for Salesforce]後可預期結果的一般瞭解，請參閱[[!DNL Adobe Workfront for Salesforce] 概觀](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md)。

* [安裝及使用 [!DNL Workfront for Salesforce]的必要條件](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [正在安裝 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>新增：[!UICONTROL Standard]</p><p>或</p><p>目前： [!UICONTROL 計畫]</p> </td> 
  </tr>  </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 安裝及使用[!DNL Workfront for Salesforce]的必要條件 {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必須擁有可存取系統管理員帳戶的[!DNL Salesforce]執行個體才能安裝應用程式。
* 您必須擁有可存取系統管理員帳戶的[!DNL Workfront]執行個體，才能設定整合。
* [!UICONTROL Salesforce]使用者必須擁有[!DNL Workfront]帳戶才能：

   * 從[!DNL Salesforce]建立[!DNL Workfront]個請求
   * 在Salesforce中檢視[!DNL Workfront]個請求或專案

## 正在安裝[!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

您必須是[!DNL Salesforce]和[!DNL Workfront]系統管理員才能安裝和設定[!DNL Workfront for Salesforce]。

下列子節說明如何為您的[!DNL Salesforce]生產環境安裝[!DNL Workfront]。 您可以依照相同的步驟為[!DNL Salesforce]沙箱環境安裝[!DNL Workfront]。

* [正在安裝 [!DNL Workfront for Salesforce] ，使其可於 [!DNL AppExchange] 市集使用](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [正在安裝 [!DNL Salesforce Classic] 架構中的 [!DNL Workfront for Salesforce] ](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [正在安裝 [!DNL Salesforce Lightning Experience] 架構中的 [!DNL Workfront for Salesforce] ](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 正在安裝[!DNL Workfront for Salesforce]，它才能在[!DNL AppExchange]市集中使用 {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce]很快將在[!DNL Salesforce AppExchange]中提供。

若要在可用之前安裝應用程式：

1. 在您的生產環境中，前往

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   在您的沙箱環境中，前往

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >您必須登入Salesforce才能存取這些頁面。

1. 勾選&#x200B;**[!UICONTROL 是，授與這些協力廠商網站的存取權]**&#x200B;方塊。

   載入畫面隨即顯示。 安裝可能需要一些時間。

1. 安裝完成時，按一下&#x200B;**[!UICONTROL 完成]**。

1. 瀏覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 安全性]控制項** > **[!UICONTROL 遠端站台設定]**。
1. （視條件而定）從清單中選取Workfront 。

   或

   如果您在&#x200B;**[!UICONTROL 所有遠端站台]**&#x200B;清單中未看到您的[!DNL Workfront] URL，請按一下&#x200B;**[!UICONTROL 新增遠端站台]**。

1. （視條件而定）如果新增站台，請指定&#x200B;**[!UICONTROL 遠端站台名稱]**。

   例如，*[!DNL Workfront]*。

1. （視條件而定）如果新增網站，請指定&#x200B;**[!UICONTROL 遠端網站URL]**。

   例如，*yourDomain.my.workfront.com*。

1. 按一下「**[!UICONTROL 儲存]**」。

   [!DNL Workfront]應用程式現已安裝在您的[!DNL Salesforce]執行個體上，而且已在您的環境中建立&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;和&#x200B;**[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce]頁面。

   將[!DNL Workfront]區段新增至其[!UICONTROL 機會]或[!UICONTROL 帳戶]頁面配置後，[!DNL Salesforce]使用者就可以使用應用程式。\
   如需有關為使用者設定Workfront區段的資訊，請參閱[為Salesforce使用者設定Adobe Workfront區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

### 正在[!DNL Salesforce Classic]架構中安裝[!DNL Salesforce]的[!DNL Workfront]

1. 以系統管理員身分登入[!DNL Salesforce]。
1. 移至&#x200B;**安裝程式。**
1. 在&#x200B;**建置**&#x200B;區段中，按一下&#x200B;**AppExchange市集**。

1. 在&#x200B;**搜尋AppExchange應用程式**&#x200B;方塊中，輸入&#x200B;**Workfront**。

1. 找到時，請按一下Workfront應用程式，然後按一下[立即取得]&#x200B;**。**
1. 按一下[在生產環境中安裝] **&#x200B;**，在您的[!DNL Salesforce]生產環境中安裝[!DNL Workfront]應用程式。 （建議）
1. 在您閱讀並同意條款與條件後，請啟用&#x200B;**[!UICONTROL 我已閱讀並同意條款與條件]**&#x200B;欄位。
1. 按一下&#x200B;**[!UICONTROL 確認並安裝]**。
1. 選取[為所有使用者安裝]&#x200B;**&#x200B;** （建議使用），然後按一下[安裝]&#x200B;**&#x200B;**。

1. （視條件而定）若詢問您是否要核准第三方存取權，您必須選取[是]，授與這些第三方網站的存取權&#x200B;**，然後按一下[繼續]**&#x200B;**。**

1. 安裝完成時，按一下&#x200B;**[!UICONTROL 完成]**。

   [!DNL Workfront]應用程式列在&#x200B;**[!UICONTROL 已安裝的封裝]**&#x200B;下。


1. 瀏覽至&#x200B;**[!UICONTROL 設定>安全性控制>遠端站台設定]**。
1. （視條件而定）如果您在&#x200B;**[!UICONTROL 所有遠端站台]**&#x200B;清單中未看到您的[!DNL Workfront] URL，請按一下&#x200B;**[!UICONTROL 新增遠端站台]**。

1. （視條件而定）如果新增站台，請指定&#x200B;**[!UICONTROL 遠端站台名稱]**。
例如，*[!DNL Workfront]*。

1. （視條件而定）如果新增網站，請指定&#x200B;**[!UICONTROL 遠端網站URL]**。
例如，*yourDomain.my.workfront.com*。

1. 按一下「**[!UICONTROL 儲存]**」。\
   [!DNL Workfront]應用程式現已安裝在您的[!DNL Salesforce]執行個體上。 已在您的環境中建立&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;及&#x200B;**[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce]頁面。\
   [!DNL Salesforce]使用者必須先將[!DNL Workfront]區段新增至其[!UICONTROL 機會]或[!UICONTROL 帳戶]頁面配置，才能使用應用程式。\
   如需有關為使用者設定[!DNL Workfront]區段的資訊，請參閱[為 [!DNL Salesforce] 使用者設定 [!DNL Adobe Workfront] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

### 正在[!DNL Salesforce Lightning Experience]架構中安裝[!DNL Workfront for Salesforce]

1. 以系統管理員身分登入[!DNL Salesforce]。
1. 按一下&#x200B;**[!UICONTROL 設定]圖示**，然後按一下&#x200B;**[!UICONTROL 設定]**。

1. 在&#x200B;**[!UICONTROL 平台工具]**&#x200B;區段中，展開&#x200B;**[!UICONTROL 應用程式].**

1. 按一下&#x200B;**[!DNL AppExchange Marketplace]**。
1. 在&#x200B;**[!UICONTROL 搜尋[!DNL AppExchange]應用程式]**&#x200B;方塊中，輸入&#x200B;**[!DNL Workfront]**。

1. 找到時，請按一下Workfront應用程式，然後按一下[立即取得]&#x200B;**。**
1. 按一下&#x200B;**[!UICONTROL 開啟登入畫面]**。\
   您必須使用[!DNL Salesforce]的[!DNL Workfront]系統管理員帳戶登入。

1. 按一下&#x200B;**[!UICONTROL 允許]**。
1. 在「**[!UICONTROL 安裝在此組織]**」方塊中，按一下「**[!UICONTROL 安裝在此處]**」以在[!DNL Salesforce]生產環境中安裝[!DNL Workfront]。 （建議）

1. 在您閱讀並同意條款與條件後，請啟用&#x200B;**[!UICONTROL 我已閱讀並同意條款與條件]**&#x200B;欄位。
1. 按一下&#x200B;**[!UICONTROL 確認並安裝]**。
1. 選取[為所有使用者安裝]&#x200B;**&#x200B;** （建議使用），然後按一下[安裝]&#x200B;**&#x200B;**。

1. （視條件而定）若詢問您是否要核准第三方存取權，您必須選取[是]，授與這些第三方網站的存取權&#x200B;**，然後按一下[繼續]**&#x200B;**。**

1. 安裝完成時，按一下&#x200B;**[!UICONTROL 完成]**。

   [!DNL Workfront]應用程式列在&#x200B;**[!UICONTROL 已安裝的封裝]**&#x200B;下。

1. 瀏覽至&#x200B;**[!UICONTROL 安裝程式].**
1. 在&#x200B;**[!UICONTROL 設定]**&#x200B;區段中，展開&#x200B;**[!UICONTROL 安全性].**

1. 按一下&#x200B;**[!UICONTROL 遠端站台設定]**。
1. （視條件而定）如果您在&#x200B;**[!UICONTROL 所有遠端站台]**&#x200B;清單中未看到您的[!DNL Workfront] URL，請按一下&#x200B;**[!UICONTROL 新增遠端站台]**。

1. （視條件而定）如果新增站台，請指定&#x200B;**[!UICONTROL 遠端站台名稱]**。
例如，*[!DNL Workfront]*。

1. （視條件而定）如果新增網站，請指定&#x200B;**[!UICONTROL 遠端網站URL]**。
例如，*yourDomain.my.workfront.com*。

1. 按一下「**[!UICONTROL 儲存]**」。

   [!DNL Workfront]應用程式現已安裝在您的[!DNL Salesforce]執行個體上，而且&#x200B;**[!DNL Workfront]**&#x200B;元件現已新增到您的環境中。

   將[!DNL Workfront]區段新增至其[!UICONTROL 機會]或[!UICONTROL 帳戶]頁面配置後，[!UICONTROL Salesforce]使用者就可以使用[!DNL Workfront]應用程式。\
   如需有關為使用者設定[!DNL Workfront]區段的資訊，請參閱[為 [!DNL Salesforce] 使用者設定 [!DNL Adobe Workfront] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

## 設定Workfront的許可權以進行Salesforce整合

### `workfront_business`的許可權

1. 瀏覽至&#x200B;**設定** > **安全性** > **信任的URL**。
1. 從清單中選取`workfront_business`。
1. 按一下&#x200B;**編輯**。
1. 在CSP指示下，勾選下列選項：

   * connect-src （指令碼）
   * font-src （字型）
   * frame-src （iframe內容）
   * img-src （影像）
   * media-src （音訊和視訊）
   * style-src （樣式表）

1. 按一下「**儲存**」。


### workfront_session的許可權

1. 瀏覽至&#x200B;**設定** > **安全性** > **信任的URL**。
1. 從清單中選取`workfront_session`。
1. 按一下&#x200B;**編輯**。
1. 在CSP指示下，勾選下列選項：

   * connect-src （指令碼）
   * font-src （字型）
   * frame-src （iframe內容）
   * img-src （影像）
   * media-src （音訊和視訊）
   * style-src （樣式表）

1. 按一下「**儲存**」。

