---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 此 [!DNL Adobe Workfront] 預覽沙箱環境
description: 「預覽沙箱」是測試環境，可作為即時環境的復本。 每週末由Workfront重新整理。 星期五新增至您即時環境的資料，會在下個星期一前顯示在您的預覽沙箱中。 所有支援套件都可存取此沙箱。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# 此 [!DNL Adobe Workfront] 預覽沙箱環境

有兩個測試環境 [!DNL Workfront] 是 [!DNL Workfront] 生產環境：

* 預覽沙箱

   「預覽沙箱」是測試環境，可作為即時環境的復本，並每週末重新整理一次 [!DNL Workfront]. 星期五新增至您即時環境的資料，會在下個星期一前顯示在您的預覽沙箱中。

   所有支援套件都可存取預覽沙箱。

* 自訂重新整理沙箱

   「自訂重新整理沙箱」是個別的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需額外付費。 如需此環境的詳細資訊，請參閱 [此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

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
   <td scope="col"> <p>預覽沙箱</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>自訂重新整理沙箱</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預覽沙箱

「預覽沙箱」可作為您組織中的使用者在不影響生產環境的情況下，安全地測試及處理來自生產環境的資料。

預覽沙箱包含您的實際生產資料；不過，它會每週末重新整理，因此資料最多可比生產環境落後一週。 自上次重新整理後建立的項目會在「預覽沙箱」環境中，直到後續重新整理為止。

資料從生產流向預覽，而非反向流動。 預覽環境的重新整理一律由 [!DNL Workfront] 每個週末。 有關刷新的特定日期和時間的詳細資訊，請轉至 [status.adobe.com](https://status.adobe.com/).

預覽沙箱也允許 [!DNL Workfront] 在新功能準備好部署到生產環境之前，在安全的環境中進行部署。 您可以測試新功能並提供 [!DNL Workfront] 存取「預覽沙箱」，即可獲得關於其功能的意見反應。 因此，雖然您的資料每週都會重新整理，但預覽沙箱的程式碼一律領先於生產程式碼。

預覽環境是運行培訓、測試新功能和確定設定功能的理想選擇。

>[!NOTE]
>
>存取「預覽沙箱」時，請注意螢幕頂端的藍色橫幅。 在此環境中工作時無法移除橫幅。
>
>您要存取的環境名稱（預覽）和代碼的發行版本會顯示在橫幅上。 按一下 **[!UICONTROL 查看新增功能]** 以取得該版本的相關資訊。
>
>![](assets/preview-banner-nwe-350x161.png)

## 存取預覽沙箱

依預設，作為 [!DNL Workfront] 管理員，您可以 [!UICONTROL 預覽] 沙箱環境。 如果您無法存取 [!UICONTROL 預覽] 沙箱環境（如本節所述）請聯絡您的 [!DNL Workfront] 管理員或我們的客戶支援團隊。

* [從 [!DNL Workfront] 介面](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [使用URL存取預覽沙箱](#accessing-the-preview-sandbox-using-a-url)

### 從 [!DNL Workfront] 介面 {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] 管理員，您可以透過 [!DNL Workfront] 介面。

若要存取預覽沙箱：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 測試環境]** ，按一下 **[!UICONTROL 沙箱預覽]**.

1. 使用您的預覽憑證登入。

   除非您在預覽重新整理發生後在生產環境中變更，否則這些憑證應與生產憑證相同。 只有在重新整理發生時，登入才會同步。 不會自動同步。

### 使用URL存取預覽沙箱 {#accessing-the-preview-sandbox-using-a-url}

* [存取叢集1、2、3和5上帳戶的預覽沙箱](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [存取叢集4上帳戶的預覽沙箱（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### 存取叢集1、2、3和5上帳戶的預覽沙箱 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

過去，您可以前往 [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

不再支援此URL，且尚未針對「預覽沙箱」環境將其重新導向至新的URL。 預覽沙箱的新正確URL為： [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>如果您有連結至預覽沙箱舊URL的書籤，請注意此變更，並在書籤中更新URL。

若要使用URL登入預覽沙箱：

1. 導覽至此URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   如果您是EMEA客戶，且您的帳戶位於叢集4，請參閱區段 [存取叢集4上帳戶的預覽沙箱（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) 這篇文章。

1. 使用您的預覽憑證登入。

   除非您在預覽重新整理後在生產環境中變更，否則預覽認證應與生產認證相同。 只有在重新整理發生時，登入才會同步。 不會自動同步。

#### 存取叢集4上帳戶的預覽沙箱（EMEA帳戶） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

若要使用URL登入預覽沙箱：

1. 導覽至此URL: `https://companyname.preview.workfront.com/`.

   您也可以前往 [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. 使用您的預覽憑證登入。

   除非您在預覽重新整理後在生產環境中變更，否則預覽認證應與生產認證相同。 只有在重新整理發生時，登入才會同步。 不會自動同步。

## 從預覽沙箱接收電子郵件

Workfront會停用「預覽沙箱」環境中的所有電子郵件通訊。 如果您想要從「預覽沙箱」環境接收電子郵件通知，必須在使用者設定中啟用此功能。 如需在「預覽沙箱」環境中啟用電子郵件通知的詳細資訊，請參閱 [啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>在「預覽沙箱」環境中，行動應用程式一律會停用報表傳送和推播通知。 您和 [!DNL Workfront] 當您存取「預覽沙箱」環境時，管理員可以為行動應用程式啟用報表傳送或推播通知。
>
>如需生產環境報表傳送的詳細資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## 單一登入 (SSO)

如果您使用SSO，請與我們的客戶支援團隊合作，確保已正確設定SSO，以便您能使用SSO憑證登入 [!UICONTROL 預覽] 沙箱。 如果您的首次登入失敗，請聯絡您的定期支援連絡人，或 [!DNL Workfront] 管理員以取得協助。

如需單一登入的詳細資訊，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 在預覽沙箱中設定單一登入

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上架到 [!DNL Adobe Admin Console]. 如果您的組織已上線至 [!DNL Adobe Admin Console]，則不需要任何動作。
>
>如需根據貴組織是否已上線至 [!DNL Adobe Admin Console]，請參閱 [平台管理差異([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe業務平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


如果您想要設定「預覽沙箱」以搭配單一登入解決方案運作，您可以與生產環境分開設定，以完成此設定。 預覽沙箱中的SSO設定與生產環境中的SSO設定無關。

預覽沙箱重新整理時（每週末），不會從生產環境複製SSO資訊以覆寫預覽沙箱設定。

在「預覽沙箱」中設定單一登入的步驟，與在生產環境中設定單一登入的步驟類似。

如需有關設定的詳細資訊 [!DNL Workfront] 使用SSO，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 預覽環境效能和可用性

[!DNL Workfront] 預覽環境不適用於效能或負載測試。 請改為使用這些環境來驗證組織現有工作流程的功能。

[!DNL Workfront] 預覽環境旨在隨時可用。

中斷 [!DNL Workfront] 在正常工作時間內預覽環境，會是解決任何生產問題（如果有的話）之後的第一個優先順序。

中斷 [!DNL Workfront] 將解決週末（星期六和星期日）的預覽環境，以便環境在星期一的營業時間內運作。
