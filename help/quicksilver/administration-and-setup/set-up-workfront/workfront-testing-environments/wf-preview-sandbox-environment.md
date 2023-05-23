---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 的 [!DNL Adobe Workfront] 預覽沙盒環境
description: 「預覽沙盒」是一個測試環境，它用作您的活動環境的副本。 每個週末，Workfront都會把它洗乾淨。 星期五添加到您的即時環境的資料將在以下星期一之前顯示在預覽沙盒中。 所有支援包都可以訪問此沙盒。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 616bca509b87fbd746132c2eeb5130e0b7789c47
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 0%

---

# 的 [!DNL Adobe Workfront] 預覽沙盒環境

有兩個測試環境 [!DNL Workfront] 是你 [!DNL Workfront] 生產環境：

* 預覽沙盒

   「預覽沙盒」是一個測試環境，它用作您即時環境的副本，每個週末都會通過 [!DNL Workfront]。 星期五添加到您的即時環境的資料將在以下星期一之前顯示在預覽沙盒中。

   所有支援包都可以訪問「預覽沙盒」。

* 自定義刷新沙盒

   自定義刷新沙盒是您手動刷新的單獨測試環境。 獲取自定義刷新沙盒需要額外的成本。 有關此環境的詳細資訊，請參見 [的 [!DNL Adobe Workfront] 自定義刷新沙盒環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard]支援包</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus]、[!UICONTROL首選]和[!UICONTROL Enterprise]支援包</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>預覽沙盒</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>自定義刷新沙盒</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預覽沙盒

「預覽沙盒」用作一個環境，在此環境中，組織中的用戶可以安全地test和處理來自生產環境的資料，而不會影響生產環境。

預覽沙盒包含您的實際生產資料；但是，它每週末都會刷新一次，因此資料最多可比生產環境落後一週。 自上次刷新後建立的項目在預覽沙盒環境中，直到以下刷新。

資料從「生產」到「預覽」單向流動，而不是反向流動。 預覽環境的刷新始終由 [!DNL Workfront] 每個週末。

預覽沙盒還允許 [!DNL Workfront] 在安全環境中部署新功能，然後再將其部署到生產環境中。 您可以test新功能並提供 [!DNL Workfront] 通過訪問「預覽沙盒」來反饋其功能。 因此，儘管您的資料每週都會刷新，但預覽沙盒的代碼始終在生產代碼之前。

預覽環境是運行培訓、測試新功能和確定設定功能的理想環境。

>[!NOTE]
>
>訪問「預覽沙盒」時，請注意螢幕頂部的藍色橫幅。 在此環境中工作時，無法刪除橫幅。
>
>您要訪問的環境的名稱（預覽）和代碼的發行版將顯示在橫幅上。 按一下 **[!UICONTROL 查看新增內容]** 有關那篇新聞的資訊。
>
>![](assets/preview-banner-nwe-350x161.png)

## 訪問預覽沙盒

預設情況下，作為 [!DNL Workfront] 管理員，您有權 [!UICONTROL 預覽] 沙盒環境。 如果無法訪問 [!UICONTROL 預覽] 沙盒環境（如本節所述），請與 [!DNL Workfront] 管理員或我們的客戶支援團隊。

* [從訪問 [!DNL Workfront] 介面](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [使用URL訪問預覽沙盒](#accessing-the-preview-sandbox-using-a-url)

### 從訪問 [!DNL Workfront] 介面 {#accessing-the-preview-sandbox-from-the-workfront-interface}

作為 [!DNL Workfront] 管理員，您可以通過 [!DNL Workfront] 。

要訪問預覽沙盒：

1. 按一下 **[!UICONTROL 主菜單]** 表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下 **[!UICONTROL 系統]** > **[!UICONTROL 首選項]**。

1. 在 **[!UICONTROL Test環境]** ，按一下 **[!UICONTROL 沙盒預覽]**。

1. 使用預覽憑據登錄。

   這些憑據應與您的生產憑據相同，除非在「預覽」刷新後在「生產」中更改了這些憑據。 登錄名僅在刷新時同步。 它們不會自動同步。

### 使用URL訪問預覽沙盒 {#accessing-the-preview-sandbox-using-a-url}

* [訪問群集1、2、3和5上帳戶的預覽沙盒](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [訪問群集4上帳戶的預覽沙盒（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### 訪問群集1、2、3和5上帳戶的預覽沙盒 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

以前，您通過轉到 [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg)。

此URL不再受支援，並且尚未重定向到「預覽沙盒」環境的新URL。 預覽沙盒的新正確URL為： [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ)。

>[!NOTE]
>
>如果您有連結到預覽沙盒的舊URL的書籤，請記下此更改並更新書籤中的URL。

要使用URL登錄「預覽沙盒」：

1. 導航到此URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   如果您是EMEA客戶，且您的帳戶位於群集4上，請參閱一節 [訪問群集4上帳戶的預覽沙盒（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) 在本文中。

1. 使用預覽憑據登錄。

   您的預覽憑據應與生產憑據相同，除非在預覽刷新後在生產中更改了這些憑據。 登錄名僅在刷新時同步。 它們不會自動同步。

#### 訪問群集4上帳戶的預覽沙盒（EMEA帳戶） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

要使用URL登錄「預覽沙盒」：

1. 導航到此URL: `https://companyname.preview.workfront.com/`。

   您也可以通過轉到 [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login)。

1. 使用預覽憑據登錄。

   您的預覽憑據應與生產憑據相同，除非在預覽刷新後在生產中更改了這些憑據。 登錄名僅在刷新時同步。 它們不會自動同步。

## 從預覽沙盒接收電子郵件

Workfront禁用「預覽沙盒」環境中的所有電子郵件通信。 如果要從「預覽沙盒」環境接收電子郵件通知，必須在用戶設定中啟用此功能。 有關在預覽沙盒環境中啟用電子郵件通知的詳細資訊，請參見 [啟用從「預覽沙盒」環境發送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

>[!NOTE]
>
>對於預覽沙盒環境，始終禁用移動應用上的報告傳遞和推送通知。 你和 [!DNL Workfront] 管理員可以在您訪問「預覽沙盒」環境時為移動應用啟用報告傳遞或推送通知。
>
>有關生產環境的報表交貨的詳細資訊，請參閱 [報告交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。


## 單一登入 (SSO)

如果您使用SSO，請與我們的客戶支援團隊合作，確保正確配置SSO，以便您能夠使用SSO憑據登錄到 [!UICONTROL 預覽] 沙盒。 如果初始登錄失敗，請聯繫您的常規支援聯繫人或 [!DNL Workfront] 管理員以獲取幫助。

有關單一登錄的詳細資訊，請參見 [Adobe Workfront單點登錄概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

## 在預覽沙盒中配置單一登錄

>[!IMPORTANT]
>
>此頁中描述的過程僅適用於尚未加入到 [!DNL Adobe Admin Console]。 如果您的組織已掛接到 [!DNL Adobe Admin Console]，無需執行任何操作。
>
>有關根據您的組織是否已掛接到 [!DNL Adobe Admin Console]，請參閱 [基於平台的管理差異([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe業務平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。


如果要將預覽沙盒配置為使用單一登錄解決方案，可以通過將其與生產環境分開配置來實現。 預覽沙盒中的SSO配置與生產環境中的SSO配置無關。

當預覽沙盒刷新（每週末）時，不會從生產環境中複製SSO資訊以覆蓋預覽沙盒配置。

在預覽沙盒中配置單一登錄的步驟與在生產環境中配置單一登錄的步驟類似。

有關配置的詳細資訊 [!DNL Workfront] 使用SSO，請參見 [Adobe Workfront單點登錄概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

## 預覽環境效能和可用性

[!DNL Workfront] 預覽環境不用於效能或負載測試。 而是使用這些環境來驗證組織現有工作流的功能。

[!DNL Workfront] 預覽環境將始終可用。

任何中斷 [!DNL Workfront] 如果存在任何生產問題，則在正常工作時間內預覽環境將是解決任何生產問題後立即的第一個優先順序。

任何中斷 [!DNL Workfront] 週末（星期六和星期日）的預覽環境將得到處理，以便環境在星期一的工作時間運行。
