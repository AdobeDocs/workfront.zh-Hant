---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] 預覽沙箱環境'
description: 預覽沙箱是測試環境，可作為即時環境的復本。 Workfront每週末都會重新整理。 星期五新增到您即時環境的資料會在下星期一之前顯示在您的預覽沙箱中。 所有支援套件皆可存取此沙箱。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# [!DNL Adobe Workfront]預覽沙箱環境

<!-- Audited: 12/2023 -->

[!DNL Workfront]有兩個測試環境，它們是[!DNL Workfront]生產環境的復本：

* 預覽沙箱

  預覽沙箱是測試環境，可作為您即時環境的復本，並在每個週末由[!DNL Workfront]重新整理。 星期五新增到您即時環境的資料會在下星期一之前顯示在您的預覽沙箱中。

  所有支援套件都可存取預覽沙箱。

* 自訂重新整理沙箱

  自訂重新整理沙箱是獨立的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需要額外付費。 如需此環境的詳細資訊，請參閱[自訂重新整理沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。 [!DNL Adobe Workfront] 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard]支援套件</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus]、[!UICONTROL Preferred]和[!UICONTROL Enterprise]支援套件</strong> </p> </th> 
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

「預覽沙箱」可作為環境，讓您組織中的使用者可在此環境中安全地測試及使用生產環境中的資料，而不會影響生產環境。

預覽沙箱包含您的實際生產資料；但是，它每週末都會重新整理，以便資料最多可在生產環境後一週內完成。 自上次重新整理時間以來建立的專案會位於預覽沙箱環境中，直到後續重新整理為止。

資料會單向流動，從生產環境流至預覽環境，而不會反向流動。 預覽環境的重新整理一律由[!DNL Workfront]安排在每個週末。

預覽沙箱還允許[!DNL Workfront]在準備部署到生產環境之前，在安全環境中部署新功能。 您可以測試新功能，並透過存取預覽沙箱提供[!DNL Workfront]對其功能的意見反應。 因此，預覽沙箱的程式碼一律先於生產程式碼，不過您的資料每週都會重新整理。

預覽環境適用於執行培訓、測試新功能和判斷設定功能。

>[!NOTE]
>
>存取預覽沙箱時，請注意熒幕頂端的藍色橫幅。 當您在此環境中工作時，無法移除橫幅。
>
>您存取的環境名稱（預覽）和程式碼的發行版本會顯示在橫幅上。 按一下&#x200B;**[!UICONTROL 檢視新增功能]**&#x200B;以取得該版本的相關資訊。
>
>![預覽橫幅](assets/preview-banner-nwe-350x161.png)

## 存取預覽沙箱

依預設，身為[!DNL Workfront]管理員，您擁有[!UICONTROL 預覽]沙箱環境的存取權。 如果您無法存取本節所述的[!UICONTROL 預覽]沙箱環境，請連絡您的[!DNL Workfront]系統管理員或我們的客戶支援團隊。


### 從[!DNL Workfront]介面存取預覽沙箱 {#accessing-the-preview-sandbox-from-the-workfront-interface}

作為[!DNL Workfront]管理員，您可以透過[!DNL Workfront]介面存取「預覽沙箱」。

若要存取「預覽沙箱」：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 測試環境]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL 沙箱預覽]**。

1. 使用您的「預覽」憑證登入。

   這些應該與您的生產認證相同，除非您在預覽重新整理發生後，於生產環境中變更了這些認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

### 使用URL存取預覽沙箱 {#accessing-the-preview-sandbox-using-a-url}

您可以使用URL存取預覽沙箱。

#### 存取叢集1、2、3和5上帳戶的預覽沙箱 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

預覽沙箱的URL是： `https://companyname.preview.workfront.com/`。

>[!NOTE]
>
>如果您有書籤連結到預覽沙箱的舊URL，請記下此變更並更新書籤中的URL。

若要使用URL登入預覽Sandbox：

1. 瀏覽至此URL： `https://companyname.preview.workfront.com/`。

   如果您是EMEA客戶且您的帳戶位於叢集4，請參閱以下存取叢集4上帳戶的預覽沙箱（EMEA帳戶）一節。

1. 使用您的預覽憑證登入。

   >[!TIP]
   >
   >您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，於生產環境中變更了這些認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。


#### 存取叢集4上帳戶的預覽沙箱（EMEA帳戶） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

若要使用URL登入預覽Sandbox：

1. 瀏覽至此URL： `https://companyname.preview.workfront.com/`。

   您也可以前往[https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login)存取「預覽沙箱」。

1. 使用您的預覽憑證登入。

   您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，於生產環境中變更了這些認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

## 從預覽Sandbox接收電子郵件

Workfront會停用來自預覽Sandbox環境的所有電子郵件通訊。 如果您想從預覽Sandbox環境接收電子郵件通知，您必須在使用者設定中啟用此功能。 如需在預覽Sandbox環境中啟用電子郵件通知的詳細資訊，請參閱[從預覽Sandbox環境啟用電子郵件傳遞](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

>[!NOTE]
>
>行動應用程式上的報告傳送和推播通知一律會在預覽沙箱環境中停用。 存取預覽沙箱環境時，您和[!DNL Workfront]管理員都無法啟用行動應用程式的報告傳遞或推播通知。
>
>如需生產環境報告傳送的詳細資訊，請參閱[報告傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。


## 單一登入 (SSO)

如果您使用SSO，請與我們的客戶支援團隊合作，確保已正確設定，以便您可以使用SSO憑證登入[!UICONTROL 預覽]沙箱。 若您的初始登入失敗，請連絡您的一般支援連絡人或[!DNL Workfront]管理員以尋求協助。

如需單一登入的詳細資訊，請參閱[Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

## 在預覽沙箱中設定單一登入

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上線到[!DNL Adobe Admin Console]的組織。 如果您的組織已加入[!DNL Adobe Admin Console]，則不需要採取任何動作。
>
>如需根據貴組織是否已加入[!DNL Adobe Admin Console]而不同的程式清單，請參閱[以平台為基礎的管理差異([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe商務平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。


如果您想要將預覽沙箱設定為使用單一登入解決方案，您可以透過與生產環境分開設定來執行此操作。 預覽沙箱中的SSO設定與生產環境中的SSO設定無關。

當您的預覽沙箱重新整理（每個週末）時，SSO資訊不會從您的生產環境複製以覆寫預覽沙箱設定。

在預覽沙箱中設定單一登入的步驟與在生產環境中設定它的步驟類似。

如需使用SSO設定[!DNL Workfront]的詳細資訊，請參閱[Adobe Workfront單一登入的概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

## 自動重新計算專案時間表

重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。

身為Workfront管理員，您可以設定Workfront何時自動重新計算專案時間表。 Workfront可每晚或專案範圍變更時，或同時於兩者，重新計算專案時間表。

如需詳細資訊，請參閱[設定專案的時間表重新計算](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

對於預覽環境，會停用夜間重新計算，且不會自動重新計算專案時間表。 您必須手動重新計算預覽環境的專案時間表。 如需詳細資訊，請參閱[重新計算專案時間表](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)。

## 預覽環境效能和可用性

[!DNL Workfront]預覽環境並非用於效能或負載測試。 反之，使用這些環境來驗證組織現有工作流程的功能性。

[!DNL Workfront]預覽環境旨在永遠可用。

[!DNL Workfront]預覽環境在正常工作時間內發生的任何中斷都將成為解決任何生產問題（如果存在）後的第一優先專案。

[!DNL Workfront]預覽環境在週末（星期六和星期日）發生的任何中斷都會得到解決，因此環境會在星期一的營業時間執行。
