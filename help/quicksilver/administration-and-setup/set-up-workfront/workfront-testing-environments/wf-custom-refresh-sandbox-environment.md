---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境
description: 自訂重新整理沙箱是一個環境，您可在其中使用生產環境中的資料進行測試和工作。 此外，也非常適合用於執行培訓及判斷設定功能。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# 此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境

自訂重新整理沙箱是一個環境，您可在其中使用生產環境中的資料進行測試和工作。 此外，也非常適合用於執行培訓及判斷設定功能。

>[!NOTE]
>
>這與預覽沙箱不同，後者也是複製您的的測試環境 [!DNL Workfront] 生產環境。
>
>* 「預覽沙箱」引入新功能後，才可在生產環境中使用。
>* 自訂重新整理沙箱中不會引入新功能，因此生產環境才能使用這些功能。
>
>  此外，取得預覽沙箱不需要的自訂重新整理沙箱會另外產生成本。
>
>  如需有關預覽沙箱的詳細資訊，請參閱 [此 [!DNL Adobe Workfront] 預覽Sandbox環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 計劃</td> 
   <td> <p>[！UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 授權</p> </td> 
   <td> <p>[！UICONTROL計畫] </p> <p>您必須是 [!DNL Workfront] 管理員。 有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支援套件</td> 
   <td> <p>[！UICONTROL Plus]、[！UICONTROL Preferred]或[！UICONTROL Enterprise]</p> <p>標準支援套件無法存取「自訂重新整理沙箱」，但可存取「預覽沙箱」。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 重新整理自訂重新整理沙箱

自訂重新整理沙箱包含您的實際生產資料，在您排程之前不會重新整理。 您可以安排在任何方便的時間重新整理，頻率為一星期一次。

>[!NOTE]
>
>* 您無法排程當天的重新整理。 例如，如果今天是6月1日，則排程重新整理的最早日期是6月2日。
>* 排程的重新整理會在夜間根據使用者的叢集進行（美國的叢集會在夜間重新整理）。 由於佇列中的其他客戶以及重新整理的資料量，特定時間無法預測。 如果佇列有許多大型客戶，則您的重新整理可能要到當天稍後或第二天才會執行。
>* 您的自訂重新整理沙箱一律會有與生產環境相同的產品功能。 不過，當您重新整理「自訂重新整理沙箱」時，它只會保留登入畫面背景顏色的品牌。 登入畫面和導覽列圖志會重設為 [!DNL Workfront] 預設值，以及您在重新整理之前修改的任何品牌影像都不會顯示。
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 從您的生產環境存取自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-from-your-production-environment}

作為 [!DNL Workfront] 管理員，您可以從生產環境存取您的「自訂重新整理沙箱」。

>[!NOTE]
>
>如果您的帳戶位於叢集4 （EMEA叢集），您無法從生產環境存取自訂重新整理沙箱。 如需當您在Cluster 4擁有帳戶時如何存取自訂重新整理沙箱的詳細資訊，請參閱 [存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

若要存取您的自訂重新整理沙箱：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 系統]** >**[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 測試環境]** 區段，按一下 **[!UICONTROL Sandbox 1]** 或 **[!UICONTROL Sandbox 2]**.

   您的支援套件會指定您是否擁有一或兩個「自訂重新整理沙箱」的存取權。

1. 使用您的自訂重新整理沙箱憑證登入。

   您的自訂重新整理沙箱認證與生產認證相同，除非您自上次重新整理自訂重新整理沙箱以來已變更生產認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

   自訂重新整理沙箱會在畫面頂端的橫幅中顯示版本以及上次重新整理日期。 重新整理完成後，生產環境中的所有資訊都可供使用並準備就緒。

## 使用URL存取自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-using-a-url}

任何使用者都可以使用URL存取「自訂重新整理沙箱」。

* [存取叢集1、2、3和5上帳戶的自訂重新整理沙箱](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 存取叢集1、2、3和5上帳戶的自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

根據您的支援套件，您應該可以存取一或兩個自訂重新整理沙箱。

若要使用URL存取您的自訂重新整理沙箱：

1. 如果您只有一個「自訂重新整理沙箱」，請導覽至此URL：

   https://companyname.sb01.workfront.com (舊URL:https://cr1.attasksandbox.com/.)

   或者，如果您有兩個自訂重新整理沙箱，除了上述URL以外，您還可以前往以下URL來存取第二個自訂重新整理沙箱：

   https://companyname.sb02.workfront.com (舊URL:https://cr2.attasksandbox.com/)

1. 在登入畫面上，使用您的「自訂重新整理沙箱」憑證登入。
1. 您的自訂重新整理沙箱認證與生產認證相同，除非您在上次重新整理自訂重新整理沙箱後已變更生產認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

### 存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶） {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

若您的 [!DNL Workfront] 帳戶位於叢集4 （EMEA叢集），您只能使用URL存取自訂重新整理沙箱。 若要瞭解您的帳戶使用哪個叢集，請連絡我們的客戶支援團隊。

根據您的支援套件，您應該可以存取一或兩個自訂重新整理沙箱。

若要使用URL存取您的自訂重新整理沙箱：

1. 如果您只有一個「自訂重新整理沙箱」，請導覽至此URL：

   https://companyname.sb01.workfront.com (舊URL:https://cr3.attasksandbox.com)

   或

   如果您有兩個自訂重新整理沙箱，請前往這些URL的其中一個：

   https://companyname.sb01.workfront.com (舊URL:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (舊URL:https://cr4.attasksandbox.com)

1. 在登入畫面上，使用您的「自訂重新整理沙箱」憑證登入。

   您的自訂重新整理沙箱認證與生產認證相同，除非您在上次重新整理自訂重新整理沙箱後已變更生產認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

## 排程重新整理您的自訂重新整理沙箱

>[!IMPORTANT]
>
>重新整理的持續時間取決於重新整理的資料大小。 在重新整理程式期間，請務必注意您的自訂重新整理沙箱環境未以任何方式使用（包括API呼叫和整合），因為這會阻礙沙箱重新整理成功完成。 [!DNL Workfront] 將會在開始之前停用自訂重新整理沙箱環境，但您必須結束任何作用中的工作階段，才能確保您的沙箱重新整理成功。

排程重新整理「自訂重新整理沙箱」後，您可以按一下 [!UICONTROL 取消] ，位於頁面頂端。 您也可以稍後重新排程。

>[!NOTE]
>
>您無法排程自動沙箱重新整理。

若要排程重新整理客戶重新整理沙箱：

1. 登入您的自訂重新整理沙箱。
1. 按一下 **[!UICONTROL 排程]** 在畫面頂端的橫幅中，從行事曆中選取日期。
1. 選取要重新整理的日期，然後按一下 **[!UICONTROL 排程重新整理]**.

## 從自訂重新整理沙箱切換到生產環境

1. 登入您的自訂重新整理沙箱。

   如需存取自訂重新整理沙箱的詳細資訊，請參閱 [從您的生產環境存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-from-your-production-environment) 或 [使用URL存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-using-a-url).

1. 按一下 **[!UICONTROL 前往生產]** 在熒幕頂端的橫幅中。

   請記住，在沙箱中完成的工作不會顯示在中 [!UICONTROL 生產] 環境，因為資料傳輸是單向的，從生產環境傳輸到您的自訂重新整理沙箱，而不是反向。

## 接收來自自訂重新整理沙箱的電子郵件

[!DNL Workfront] 停用來自自訂重新整理沙箱環境的所有電子郵件通訊。 如果您想從「自訂重新整理沙箱」環境接收電子郵件通知，您必須在使用者設定中啟用此功能。 如需在「自訂重新整理沙箱」環境中啟用電子郵件通知的詳細資訊，請參閱 [啟用從預覽Sandbox環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>行動應用程式上的報表傳送和推播通知一律會在自訂重新整理沙箱環境中停用。 您或 [!DNL Workfront] 當您存取「自訂重新整理沙箱」環境時，管理員可以為行動應用程式啟用報告傳送或推播通知。\
>如需生產環境之報表傳送的詳細資訊，請參閱 [報表傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)如需有關生產環境之行動應用程式的推播通知詳細資訊，請參閱中的區段。

## 在自訂重新整理沙箱中設定單一登入

如果您想要設定自訂重新整理沙箱以搭配單一登入解決方案使用，您可以透過與生產環境分開設定來執行此操作。 自訂重新整理沙箱中的SSO設定與生產環境中的SSO設定無關。\
當您重新整理自訂重新整理沙箱時，不會從生產環境複製SSO資訊以覆寫自訂重新整理沙箱設定。

在「自訂重新整理沙箱」中設定單一登入的步驟，類似於在生產環境中設定單一登入的步驟。\
如需關於設定的詳細資訊 [!DNL Workfront] 若使用SSO，請參閱 [Adobe Workfront單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>如果您組織的 [!DNL Workfront] 執行個體已啟用Adobe IMS。 如需詳細資訊，請洽詢您的網路或IT管理員。

## 預期用途與可用性

* [!DNL Workfront] 自訂重新整理沙箱環境不適用於效能或負載測試。 反之，使用這些環境來驗證組織現有工作流程的功能性。

* [!DNL Workfront] 自訂重新整理沙箱環境旨在永遠可用。 Workfront自訂重新整理沙箱環境在正常工作時間內發生的任何中斷，都是解決任何生產問題（如果存在）後立即優先考慮的事項。 Workfront自訂重新整理沙箱環境在週末（星期六和星期日）發生的任何中斷都會得到解決，因此環境會在星期一的營業時間執行。

* 校訂在自訂重新整理沙箱環境中不可用。
