---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者
description: 安裝後 [!DNL Adobe Workfront] Salesforce as a [!DNL Workfront] 管理員，您可以在Salesforce的「機會」和「帳戶」頁面配置中將其添加到新區段中，使用戶可以使用它。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# 設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者

A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要計畫。 如需各種可用計畫的詳細資訊，請參閱 [[!DNL Workfront] 計畫。](https://www.workfront.com/plans)

安裝後 [!DNL Adobe Workfront] for [!DNL Salesforce] as a [!DNL Workfront] 管理員，您可以將其新增至使用者的新區段，以讓使用者使用 [!UICONTROL 機會] 和 [!UICONTROL 帳戶]
頁面配置 [!UICONTROL Salesforce].

有關安裝的資訊 [!DNL Workfront for Salesforce]，請參閱 [安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

若使用者 [!DNL Workfront] 可在 [!DNL Classic] 和 [!DNL Lightning Experience] 框架，您必須新增 [!DNL WorkfrontOpportunities] 和 [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] 頁面 [!UICONTROL 機會] 和 [!UICONTROL 帳戶] 頁面配置。

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

## 必要條件

* 您必須有 [!DNL Salesforce] 具有系統管理員帳戶訪問權限的實例。
* 您必須有 [!DNL Workfront] 具有系統管理員帳戶訪問權限的實例。

## 設定 [!DNL Workfront] 區段 [!DNL Salesforce Classic] 框架

1. 登入 [!DNL Salesforce] 身為Workfront管理員。
1. 按一下 **[!UICONTROL 設定].**
1. 在 **[!UICONTROL 建置]** 區段，展開 **[!UICONTROL 自訂].**

1. 展開 **[!UICONTROL 機會]**，然後按一下 **[!UICONTROL 頁面配置]** 若要新增 [!DNL Workfront] Opportunity的部分。

   或

   展開 **[!UICONTROL 帳戶]**，然後按一下 **[!UICONTROL 頁面配置]** 若要新增 [!DNL Workfront] 區段轉換為帳戶。

1. 按一下 **[!UICONTROL 編輯]** 在現有版面上。

   或

   按一下 **[!UICONTROL 新增]** 來新增版面。

1. （選用）拖曳 **[!UICONTROL 區段]** 元件，並將其拖曳至所需位置。

1. （選用）指定新區段的名稱。

   建議您為此區段命名 **[!DNL Workfront]**.

1. （選用）指定所需 **[!UICONTROL 版面]** 和 **[!UICONTROL 索引鍵順序]** ，以取得Advertising Cloud的說明。

   建議您選取 **[!UICONTROL 1欄]** 版面 [!DNL Workfront] 區段。

1. 按一下 **[!UICONTROL 確定]**.
1. 在 **[!UICONTROL 版面]** 按一下 **[!UICONTROL 視覺效果強制頁面].**

1. 拖放 **[!UICONTROL WorkfrontOpportunity]** 元件至 **[!UICONTROL 機會]** 版面。

   或

   拖放 **[!UICONTROL WorkfrontAccounts]** 元件至  **[!UICONTROL 帳戶]** 佈局。\

1. 按一下 **[!UICONTROL 屬性]** 表徵圖。\

1. 若要獲得最佳顯示，請為 [!DNL Workfront Visualforce] 頁面：

   * **[!UICONTROL 寬度（像素或%）]**:100%
   * **[!UICONTROL 高度（像素）]**:600
   * 選擇 **[!UICONTROL 顯示捲軸]**.

1. 按一下 **[!UICONTROL 確定]**.
1. 按一下 **[!UICONTROL 儲存]** 來儲存版面。

   所有已指派此配置給他們的使用者，現在都可以看到 [!DNL Workfront] 區段 [!UICONTROL 機會] 或 [!UICONTROL 帳戶] 對象。

   使用者可看見 [!DNL Workfront] 登入畫面 [!DNL Workfront] 區段。 如果他們沒有 [!DNL Workfront] 帳戶，則它們可以折疊區段，但無法將其從配置中移除。

## 設定 [!DNL Workfront] 區段 [!DNL Salesforce Lightning Experience] 框架

您可以新增 [!DNL Workfront] 區段至 [!DNL Salesforce] [!UICONTROL 機會] 或 [!DNL Salesforce Lightning Experience] 框架，方法是 [!UICONTROL 設定] 區域，或來自帳戶或 [!UICONTROL 機會] 物件。

* [設定 [!DNL Workfront] 區段 [!UICONTROL 設定] 層級](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [設定 [!DNL Workfront] Opportunity或Account級別的部分](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### 設定 [!DNL Workfront] 區段 [!UICONTROL 設定] 層級 {#configure-the-workfront-section-at-the-setup-level}

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 按一下 **[!UICONTROL 設定]** 圖示，然後按一下 **[!UICONTROL 設定]**.

1. 展開 **[!UICONTROL 物件和欄位]**，然後按一下 **[!UICONTROL 物件管理員]**.

1. 按一下 **[!UICONTROL 機會]** 定制Opportunity的佈局。

   或

   按一下 **[!UICONTROL 帳戶]** 以自訂帳戶的配置。

1. 按一下 **[!UICONTROL 頁面配置]**.
1. 按一下現有頁面版面的名稱即可加以編輯。

   或

   按一下 **[!UICONTROL 新增]** 來建立新的頁面配置。

1. 繼續 [設定 [!DNL Workfront] Opportunity或Account級別的部分](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) 下方。

### 設定 [!DNL Workfront] Opportunity或Account級別的部分 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. 前往 **[!UICONTROL 機會]** 或 **[!UICONTROL 帳戶]**.

1. 按一下 **[!UICONTROL 設定]** 圖示，然後按一下 **[!UICONTROL 編輯頁面]**.\

1. 展開 **[!UICONTROL 自訂管理]** 區段。
1. 拖放 **[!DNL Workfront]** 元件 [!UICONTROL 機會] 或帳戶頁面。

   建議將頁面的全部寬度用於 [!DNL Workfront] 區段，而非版面的其中一欄。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   所有已指派此配置給他們的使用者，現在都可以看到 [!DNL Workfront] 區段 [!UICONTROL 機會] 或 [!UICONTROL 帳戶] 對象。

   >[!NOTE]
   >
   >使用者可看見 [!DNL Workfront] 登入畫面 [!DNL Workfront] 區段。 如果他們沒有 [!DNL Workfront] 帳戶，則它們可以折疊區段，但無法將其從配置中移除。 使用者可以使用您已啟用的驗證方法登入：增強驗證或您的安全斷言標籤語言(SAML)URL。

