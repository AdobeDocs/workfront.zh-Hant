---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 此 [!DNL Adobe Workfront] 預覽沙箱環境
description: 預覽沙箱是測試環境，可作為您的即時環境的復本。 Workfront每週末都會重新整理。 在星期五新增到您即時環境的資料會在下星期一之前顯示在您的預覽沙箱中。 所有支援套件皆可存取此沙箱。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# 此 [!DNL Adobe Workfront] 預覽沙箱環境

有兩個測試環境 [!DNL Workfront] 您的電腦的復本 [!DNL Workfront] 生產環境：

* 預覽沙箱

   預覽沙箱是測試環境，可作為即時環境的復本，並於每個週末由更新 [!DNL Workfront]. 在星期五新增到您即時環境的資料會在下星期一之前顯示在您的預覽沙箱中。

   所有支援套件都可存取預覽沙箱。

* 自訂重新整理沙箱

   自訂重新整理沙箱是獨立的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需要額外付費。 如需此環境的詳細資訊，請參閱 [此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[！UICONTROL Standard]支援套件</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL Plus]、[！UICONTROL Preferred]和[！UICONTROL Enterprise]支援套件</strong> </p> </th> 
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

「預覽沙箱」可作為環境，讓組織中的使用者可在此環境中安全地測試及使用生產環境中的資料，而不會影響生產環境。

「預覽沙箱」包含您的實際生產資料；不過，它會在每個週末重新整理，因此資料最多可比生產環境晚一週。 自上次重新整理時間以來建立的專案會位於預覽沙箱環境中，直到下次重新整理為止。

資料會單向流動、從生產環境流至預覽環境，而不會反向流動。 「預覽」環境的重新整理一律會由排程 [!DNL Workfront] 每個週末。

預覽Sandbox也可讓 [!DNL Workfront] 在準備部署到生產環境之前，在安全的環境中部署新功能。 您可以測試新功能並提供 [!DNL Workfront] 存取「預覽Sandbox」即可對其功能提供意見回饋。 因此，雖然您的資料每週都會重新整理，但預覽沙箱的程式碼一律會領先於生產程式碼。

預覽環境非常適合執行培訓、測試新功能和判斷設定功能。

>[!NOTE]
>
>存取預覽沙箱時，請注意畫面頂端的藍色橫幅。 當您在此環境中工作時，無法移除橫幅。
>
>您正在存取的環境名稱（預覽）和程式碼的發行版本會顯示在橫幅上。 按一下 **[!UICONTROL 檢視新增功能]** 以取得該版本的相關資訊。
>
>![](assets/preview-banner-nwe-350x161.png)

## 存取預覽沙箱

依預設，作為 [!DNL Workfront] 管理員，您擁有 [!UICONTROL 預覽] 沙箱環境。 如果您無法存取 [!UICONTROL 預覽] 如本節所述的沙箱環境，請聯絡您的 [!DNL Workfront] 管理員或我們的客戶支援團隊。

* [從存取「預覽沙箱」 [!DNL Workfront] 介面](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [使用URL存取預覽沙箱](#accessing-the-preview-sandbox-using-a-url)

### 從存取「預覽沙箱」 [!DNL Workfront] 介面 {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] 管理員，您可以透過以下方式存取預覽沙箱： [!DNL Workfront] 介面。

若要存取「預覽沙箱」：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 測試環境]** 區段，按一下 **[!UICONTROL 沙箱預覽]**.

1. 使用您的預覽憑證登入。

   這些應該與您的生產認證相同，除非您在預覽重新整理發生後，在生產環境中變更了這些認證。 登入只有在重新整理發生時才會進行同步處理。 它們不會自動同步。

### 使用URL存取預覽沙箱 {#accessing-the-preview-sandbox-using-a-url}

* [存取叢集1、2、3和5上帳戶的預覽沙箱](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [存取叢集4上帳戶的預覽沙箱（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### 存取叢集1、2、3和5上帳戶的預覽沙箱 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

「預覽沙箱」的URL是： `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>如果您有連結至預覽Sandbox的舊URL的書籤，請記下此變更並更新書籤中的URL。

若要使用URL登入「預覽沙箱」：

1. 導覽至此URL： `https://companyname.preview.workfront.com/`.

   如果您是EMEA客戶，且您的帳戶位於叢集4，請參閱區段 [存取叢集4上帳戶的預覽沙箱（EMEA帳戶）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) 本文章內容。

1. 使用您的預覽憑證登入。

   您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，在生產環境中變更了這些認證。 登入只有在重新整理發生時才會進行同步處理。 它們不會自動同步。

#### 存取叢集4上帳戶的預覽沙箱（EMEA帳戶） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

若要使用URL登入「預覽沙箱」：

1. 導覽至此URL： `https://companyname.preview.workfront.com/`.

   您也可以前往「 」，存取「預覽沙箱」 [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. 使用您的預覽憑證登入。

   您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，在生產環境中變更了這些認證。 登入只有在重新整理發生時才會進行同步處理。 它們不會自動同步。

## 從預覽沙箱接收電子郵件

Workfront會停用來自預覽Sandbox環境的所有電子郵件通訊。 如果您想從預覽沙箱環境接收電子郵件通知，您必須在使用者設定中啟用此功能。 如需在預覽沙箱環境中啟用電子郵件通知的詳細資訊，請參閱 [啟用從預覽沙箱環境的電子郵件傳送](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>行動應用程式上的報告傳送和推播通知一律會在預覽沙箱環境中停用。 您或 [!DNL Workfront] 當您存取預覽沙箱環境時，管理員可以為行動應用程式啟用報告傳送或推播通知。
>
>如需生產環境報告傳送的詳細資訊，請參閱 [報告傳遞概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## 單一登入 (SSO)

如果您使用SSO，請與我們的客戶支援團隊合作，確保已正確設定，以便您可以使用SSO憑證登入 [!UICONTROL 預覽] 沙箱。 如果您的初始登入失敗，請連絡您的定期支援聯絡或 [!DNL Workfront] 管理員以尋求協助。

如需單一登入的詳細資訊，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 在預覽沙箱中設定單一登入

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未上線至的組織。 [!DNL Adobe Admin Console]. 如果您的組織已上線至 [!DNL Adobe Admin Console]，無需採取任何動作。
>
>針對因貴組織是否已上線至而不同的程式清單， [!DNL Adobe Admin Console]，請參閱 [平台式管理差異([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe商務平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


如果您想要設定預覽沙箱以搭配單一登入解決方案使用，您可以透過在生產環境以外個別設定來執行此操作。 預覽沙箱中的SSO設定與生產環境中的SSO設定無關。

當您的預覽沙箱重新整理（每週末）時，SSO資訊不會從您的生產環境複製以覆寫預覽沙箱設定。

在預覽沙箱中設定單一登入的步驟與在生產環境中設定它的步驟類似。

如需關於設定的詳細資訊 [!DNL Workfront] 若使用SSO，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 預覽環境效能和可用性

[!DNL Workfront] 預覽環境並非用於效能或負載測試。 而是使用這些環境來驗證您組織現有工作流程的功能性。

[!DNL Workfront] 預覽環境旨在永遠可用。

對的任何中斷 [!DNL Workfront] 解決任何生產問題（如果存在）後，將立即優先在正常工作時間內預覽環境。

對的任何中斷 [!DNL Workfront] 週末（星期六和星期日）預覽環境將進行處理，以便環境在星期一的營業時間執行。
