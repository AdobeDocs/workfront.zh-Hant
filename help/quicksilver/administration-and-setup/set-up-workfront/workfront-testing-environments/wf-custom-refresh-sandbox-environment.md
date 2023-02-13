---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境
description: 「自訂重新整理沙箱」是一個環境，您可在此測試及使用生產環境中的資料。 它也是運行培訓和確定設定功能的理想選擇。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# 此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境

「自訂重新整理沙箱」是一個環境，您可在此測試及使用生產環境中的資料。 它也是運行培訓和確定設定功能的理想選擇。

>[!NOTE]
>
>這與「預覽沙箱」不同，「預覽沙箱」也是複製您 [!DNL Workfront] 生產環境。
>
>* 新功能會導入「預覽沙箱」中，之後才可在生產環境中使用。
>* 自訂重新整理沙箱中不會導入新功能，這些功能才會在生產環境中使用。
>
>  此外，取得「預覽沙箱」不需要的自訂重新整理沙箱，也需額外付費。
>
>  如需預覽沙箱的詳細資訊，請參閱 [此 [!DNL Adobe Workfront] 預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 計劃</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 授權</p> </td> 
   <td> <p>[!UICONTROL計畫] </p> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支援套件</td> 
   <td> <p>[!UICONTROL Plus]、[!UICONTROL Preferred]或[!UICONTROL Enterprise]</p> <p>標準支援套件無法存取自訂重新整理沙箱，但可存取預覽沙箱。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 重新整理自訂重新整理沙箱

自訂重新整理沙箱包含您的實際生產資料，除非您排程重新整理，否則資料不會重新整理。 您隨時都可以安排重新整理的時間，這樣的頻率可以達到每週一次。

>[!NOTE]
>
>* 您無法排程當天的重新整理。 例如，如果今天是6月1日，則您可以排程重新整理的最早日期為6月2日。
>* 您的自訂重新整理沙箱的產品功能一律與生產環境相同。 不過，當您重新整理自訂重新整理沙箱時，只會針對登入畫面背景顏色保留品牌。 登入畫面和導覽列標誌會重設為 [!DNL Workfront] 預設值，在重新整理之前您修改的任何品牌影像都不會顯示。
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 從生產環境存取自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a [!DNL Workfront] 管理員，您可以從生產環境存取自訂重新整理沙箱。

>[!NOTE]
>
>如果您的帳戶位於叢集4（EMEA叢集），則無法從生產環境存取自訂重新整理沙箱。 如需在叢集4上擁有帳戶時，如何存取自訂重新整理沙箱的詳細資訊，請參閱 [訪問群集4（EMEA帳戶）上帳戶的自定義刷新沙箱](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [訪問群集4（EMEA帳戶）上帳戶的自定義刷新沙箱](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

若要存取自訂重新整理沙箱：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 系統]** >**[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 測試環境]** ，按一下 **[!UICONTROL 沙箱1]** 或 **[!UICONTROL 沙箱2]**.

   您的支援套件會指定您是否擁有一或兩個自訂重新整理沙箱的存取權。

1. 使用您的自訂重新整理沙箱憑證登入。

   除非您自上次重新整理自訂重新整理沙箱後，已變更生產憑證，否則您的自訂重新整理沙箱憑證與生產憑證相同。 只有在重新整理發生時，登入才會同步。 不會自動同步。

   「自訂重新整理沙箱」會在畫面頂端顯示橫幅中的版本以及上次重新整理日期。 生產環境中的所有資訊都可供使用，且可在重新整理完成後繼續使用。

## 使用URL存取自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-using-a-url}

任何使用者都可使用URL存取自訂重新整理沙箱。

* [存取叢集1、2、3和5上帳戶的自訂重新整理沙箱](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [訪問群集4（EMEA帳戶）上帳戶的自定義刷新沙箱](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 存取叢集1、2、3和5上帳戶的自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

根據您的支援套件，您應可存取一或兩個自訂重新整理沙箱。

若要使用URL存取自訂重新整理沙箱：

1. 如果您只有一個自訂重新整理沙箱，請導覽至此URL:

   https://companyname.sb01.workfront.com（舊URL）:https://cr1.attasksandbox.com/)

   或者，除了上述URL外，如果您有兩個「自訂重新整理」沙箱，您也可以前往下列URL來存取第二個「自訂重新整理沙箱」：

   https://companyname.sb02.workfront.com（舊URL）:https://cr2.attasksandbox.com/)

1. 在登入畫面中，使用您的自訂重新整理沙箱憑證登入。
1. 自訂重新整理沙箱認證與生產認證相同，除非您自上次重新整理自訂重新整理沙箱以來已變更生產認證。 只有在重新整理發生時，登入才會同步。 不會自動同步。

### 訪問群集4（EMEA帳戶）上帳戶的自定義刷新沙箱 {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

若您的 [!DNL Workfront] 帳戶位於叢集4（EMEA叢集），您只能使用URL存取自訂重新整理沙箱。 若要了解您的帳戶所在的叢集，請聯絡我們的客戶支援團隊。

根據您的支援套件，您應可存取一或兩個自訂重新整理沙箱。

若要使用URL存取自訂重新整理沙箱：

1. 如果您只有一個自訂重新整理沙箱，請導覽至此URL:

   https://companyname.sb01.workfront.com（舊URL）:https://cr3.attasksandbox.com

   或

   如果您有兩個「自訂重新整理」沙箱，請前往以下任一URL:

   https://companyname.sb01.workfront.com（舊URL）:https://cr3.attasksandbox.com

   https://companyname.sb02.workfront.com（舊URL）:https://cr4.attasksandbox.com

1. 在登入畫面中，使用您的自訂重新整理沙箱憑證登入。

   自訂重新整理沙箱認證與生產認證相同，除非您自上次重新整理自訂重新整理沙箱以來已變更生產認證。 只有在重新整理發生時，登入才會同步。 不會自動同步。

## 排程重新整理自訂重新整理沙箱

>[!IMPORTANT]
>
>重新整理的持續時間取決於要重新整理的資料大小。 在重新整理程式期間，您的自訂重新整理沙箱環境絕對不會受到任何使用（包括API呼叫和整合），因為這會使沙箱重新整理作業無法順利完成。 [!DNL Workfront] 會在自訂重新整理沙箱環境開始前加以停用，但您必須結束任何作用中的工作階段，以確保沙箱重新整理成功。

排程自訂重新整理沙箱的重新整理後，按一下「 」即可取消 [!UICONTROL 取消] 頁面頂端。 您也可以稍後重新排程。

>[!NOTE]
>
>您無法排程自動沙箱重新整理。

若要排程重新整理客戶重新整理沙箱：

1. 登入自訂重新整理沙箱。
1. 按一下 **[!UICONTROL 排程]** 在畫面頂端的橫幅中，從日曆中選取日期。
1. 選取要重新整理的日期，然後按一下 **[!UICONTROL 排程重新整理]**.

## 從自訂重新整理沙箱切換至生產環境

1. 登入自訂重新整理沙箱。

   如需存取自訂重新整理沙箱的詳細資訊，請參閱 [從生產環境存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-from-your-production-environment) 或 [使用URL存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-using-a-url).

1. 按一下 **[!UICONTROL 前往生產環境]** 在畫面頂端的橫幅中。

   請記住，沙箱中完成的工作不會顯示在 [!UICONTROL 生產] 環境，因為資料傳輸是單向的，從生產環境傳輸到自訂重新整理沙箱，而不是反向傳輸。

## 從自訂重新整理沙箱接收電子郵件

[!DNL Workfront] 停用來自「自訂重新整理沙箱」環境的所有電子郵件通訊。 如果您想要從「自訂重新整理沙箱」環境接收電子郵件通知，必須在您的使用者設定中啟用此功能。 如需在自訂重新整理沙箱環境中啟用電子郵件通知的詳細資訊，請參閱 [啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>行動應用程式上的報表傳送和推播通知一律會在自訂重新整理沙箱環境中停用。 您和 [!DNL Workfront] 存取「自訂重新整理沙箱」環境時，管理員可為行動應用程式啟用報表傳送或推播通知。\
>如需生產環境報表傳送的詳細資訊，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。如需生產環境之行動應用程式上推播通知的詳細資訊，請參閱中的區段。

## 在自訂重新整理沙箱中設定單一登入

如果您想要設定自訂重新整理沙箱以搭配單一登入解決方案使用，您可以與生產環境分開設定，以完成此設定。 自訂重新整理沙箱中的SSO設定與生產環境中的SSO設定無關。\
重新整理自訂重新整理沙箱時，系統不會從生產環境複製SSO資訊，以覆寫自訂重新整理沙箱設定。

在「自訂重新整理沙箱」中設定單一登入的步驟，與在生產環境中設定單一登入的步驟類似。\
如需有關設定的詳細資訊 [!DNL Workfront] 使用SSO，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>如果您組織的 [!DNL Workfront] 例項已透過Adobe IMS啟用。 如需詳細資訊，請洽詢您的網路或IT管理員。

## 預期用途和可用性

[!DNL Workfront] 自訂重新整理沙箱環境不適用於效能或負載測試。 請改為使用這些環境來驗證組織現有工作流程的功能。

[!DNL Workfront] 自訂重新整理沙箱環境可隨時使用。 在正常營業時間內，Workfront自訂重新整理沙箱環境的任何中斷，都會是解決生產問題（如果有的話）之後的第一個優先順序。 週末（星期六和星期日）Workfront自訂重新整理沙箱環境的任何中斷都將解決，使環境在星期一的營業時間內執行。
