---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] 自訂重新整理沙箱環境'
description: 自訂重新整理沙箱是一個環境，您可在其中使用生產環境中的資料進行測試和工作。 此外，也非常適合用於執行培訓及判斷設定功能。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
TQID: https://experienceleague.adobe.com/0orzAcBft4J52M4nMDMxk6Kupagmn81V3qHB-M5YkvY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1f811e3467e8efa7c048bdc148792c4b6f03416c
workflow-type: tm+mt
source-wordcount: 1828
ht-degree: 0%

---

# [!DNL Adobe Workfront]自訂重新整理沙箱環境

自訂重新整理沙箱是一個環境，您可在其中使用生產環境中的資料進行測試和工作。 此外，也非常適合用於執行培訓及判斷設定功能。

>[!NOTE]
>
>這與預覽沙箱不同，預覽沙箱也是複製您的[!DNL Workfront]生產環境的測試環境。
>
>* 「預覽沙箱」引入新功能後，才可在生產環境中使用。
>* 自訂重新整理沙箱中不會引入新功能，因此生產環境才能使用這些功能。
>
>  此外，取得預覽沙箱不需要的自訂重新整理沙箱會另外產生成本。
>
>  如需有關預覽沙箱的詳細資訊，請參閱[預覽沙箱環境 [!DNL Adobe Workfront] &#x200B;](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront套件</td> 
   <td> <p>Prime或Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Workfront授權</td> 
   <td> <p>標準</p><p>規劃</p>  </td> 
  </tr> 
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td><p>您必須是Workfront管理員。</p>
   </td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 重新整理自訂重新整理沙箱

自訂重新整理沙箱包含您的實際生產資料，在您排程之前不會重新整理。 您可以安排在任何方便的時間重新整理，頻率為一星期一次。

>[!IMPORTANT]
>
>自訂重新整理沙箱環境只會從您的生產環境重新整理。 沙箱環境沒有執行時間點還原的程式。 若要更新沙箱資料，請從生產環境排程標準重新整理。

>[!NOTE]
>
>* 您無法排程當天的重新整理。 例如，如果今天是6月1日，則排程重新整理的最早日期是6月2日。
>* 排程的重新整理會在夜間根據使用者的叢集進行（美國的叢集會在夜間重新整理）。 由於佇列中的其他客戶以及重新整理的資料量，特定時間無法預測。 如果佇列有許多大型客戶，則您的重新整理可能要到當天稍後或第二天才會執行。
>* 您的自訂重新整理沙箱一律會有與生產環境相同的產品功能。 不過，當您重新整理「自訂重新整理沙箱」時，它只會保留登入畫面背景顏色的品牌。 登入畫面與導覽列圖志會重設為[!DNL Workfront]預設值，而您在重新整理前修改的所有商標影像都不會顯示。
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 自訂重新整理沙箱中的Adobe雲端儲存空間

Adobe雲端儲存空間可在自訂重新整理沙箱中使用，因此您可以在生產環境中啟用它之前先測試它。 不過，Frame.io檢視器不適用於沙箱環境，因此完整統一檢閱和核准體驗必須在生產環境中驗證。

升級至支援Adobe雲端儲存空間的Workfront版本後，您必須重新整理自訂重新整理沙箱，才能存取沙箱中的Adobe雲端儲存空間功能。 重新整理完成後，您可以開始測試Adobe雲端儲存空間。 如需詳細資訊，請參閱[為您的組織啟用Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

## 從您的生產環境存取自訂重新整理沙箱 {#access-the-custom-refresh-sandbox-from-your-production-environment}

作為[!DNL Workfront]管理員，您可以從生產環境存取您的「自訂重新整理沙箱」。

>[!NOTE]
>
>如果您的帳戶位於叢集4 （EMEA叢集），您無法從生產環境存取自訂重新整理沙箱。 如需如何在您擁有叢集4上的帳戶時存取自訂重新整理沙箱的詳細資訊，請參閱[存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)。

若要存取您的自訂重新整理沙箱：

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 系統]** >**[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 測試環境]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL 沙箱1]**&#x200B;或&#x200B;**[!UICONTROL 沙箱2]**。

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

   `https://companyname.sb01.workfront.com` （舊URL：`https://cr1.attasksandbox.com/`。）

   或者，如果您有兩個自訂重新整理沙箱，除了上述URL以外，您還可以前往以下URL來存取第二個自訂重新整理沙箱：

   `https://companyname.sb02.workfront.com` （舊URL：`https://cr2.attasksandbox.com/`）

1. 在登入畫面上，使用您的「自訂重新整理沙箱」憑證登入。
1. 您的自訂重新整理沙箱認證與生產認證相同，除非您在上次重新整理自訂重新整理沙箱後已變更生產認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

### 存取叢集4上帳戶的自訂重新整理沙箱（EMEA帳戶） {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

如果您的[!DNL Workfront]帳戶位於叢集4 （EMEA叢集），您只能使用URL存取自訂重新整理沙箱。 若要瞭解您的帳戶使用哪個叢集，請連絡我們的客戶支援團隊。

根據您的支援套件，您應該可以存取一或兩個自訂重新整理沙箱。

若要使用URL存取您的自訂重新整理沙箱：

1. 如果您只有一個「自訂重新整理沙箱」，請導覽至此URL：

   `https://companyname.sb01.workfront.com` （舊URL：`https://cr3.attasksandbox.com`）

   或

   如果您有兩個自訂重新整理沙箱，請前往這些URL的其中一個：

   `https://companyname.sb01.workfront.com` （舊URL：`https://cr3.attasksandbox.com`）

   `https://companyname.sb02.workfront.com` （舊URL：`https://cr4.attasksandbox.com`）

1. 在登入畫面上，使用您的「自訂重新整理沙箱」憑證登入。

   您的自訂重新整理沙箱認證與生產認證相同，除非您在上次重新整理自訂重新整理沙箱後已變更生產認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。

## 排程重新整理您的自訂重新整理沙箱

>[!IMPORTANT]
>
>重新整理的持續時間取決於重新整理的資料大小。 在重新整理程式期間，請務必注意您的自訂重新整理沙箱環境未以任何方式使用（包括API呼叫和整合），因為這會阻礙沙箱重新整理成功完成。 [!DNL Workfront]將會在開始之前停用自訂重新整理沙箱環境，但您必須結束任何作用中的工作階段，才能確保您的沙箱重新整理成功。

在您排程重新整理「自訂重新整理沙箱」後，可以按一下頁面頂端的「[!UICONTROL 取消]」來取消它。 您也可以稍後重新排程。

>[!NOTE]
>
>您無法排程自動沙箱重新整理。

若要排程重新整理客戶重新整理沙箱：

1. 登入您的自訂重新整理沙箱。
1. 按一下熒幕上方橫幅中的&#x200B;**[!UICONTROL 排程]**，並從行事曆中選取日期。
1. 選取要重新整理的日期，然後按一下&#x200B;**[!UICONTROL 排程重新整理]**。

## 從自訂重新整理沙箱切換到生產環境

1. 登入您的自訂重新整理沙箱。

   如需有關存取自訂重新整理沙箱的詳細資訊，請參閱[從您的生產環境存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-from-your-production-environment)或[使用URL存取自訂重新整理沙箱](#access-the-custom-refresh-sandbox-using-a-url)。

1. 按一下熒幕上方橫幅中的&#x200B;**[!UICONTROL [前往生產環境]]**。

   請記住，在沙箱中完成的工作不會顯示在[!UICONTROL 生產]環境中，因為資料傳輸是單向的，從生產環境傳輸到您的自訂重新整理沙箱，而不是反向。

## 接收來自自訂重新整理沙箱的電子郵件

[!DNL Workfront]會停用所有來自自訂重新整理沙箱環境的電子郵件通訊。 如果您想從「自訂重新整理沙箱」環境接收電子郵件通知，您必須在使用者設定中啟用此功能。 如需有關在自訂重新整理沙箱環境中啟用電子郵件通知的詳細資訊，請參閱[啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

>[!NOTE]
>
>行動應用程式上的報表傳送和推播通知一律會在自訂重新整理沙箱環境中停用。 當您存取「自訂重新整理沙箱」環境時，您和[!DNL Workfront]管理員都無法啟用行動應用程式的報表傳送或推播通知。\
>如需生產環境報告傳送的詳細資訊，請參閱[報告傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

<!--

Remove me October 2026

## Configure Single Sign-On in the Custom Refresh Sandbox

If you want to configure your Custom Refresh Sandbox to work with a Single Sign-On solution, you can do so by configuring it separately from your Production environment. The SSO configuration in the Custom Refresh Sandbox is independent from your SSO configuration in the Production environment.\
When you refresh your Custom Refresh Sandbox, the SSO information is not copied from your Production environment to overwrite the Custom Refresh Sandbox configuration.

The steps for configuring single sign-on in the Custom Refresh Sandbox are similar to those for configuring it in the Production environment.\
For more information about configuring [!DNL Workfront] with SSO, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>This is not available if your organization's [!DNL Workfront] instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

-->

## 自動重新計算專案時間表

重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。

身為Workfront管理員，您可以設定Workfront何時自動重新計算專案時間表。 Workfront可每晚或專案範圍變更時，或同時於兩者，重新計算專案時間表。

如需詳細資訊，請參閱[設定專案的時間表重新計算](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

在「自訂重新整理沙箱」環境中，會停用每晚重新計算，且不會自動重新計算專案時間表。 您必須手動重新計算「自訂重新整理沙箱」環境的專案時間表。 如需詳細資訊，請參閱[重新計算專案時間表](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)。


## 預期用途與可用性

* [!DNL Workfront]自訂重新整理沙箱環境不適用於效能或負載測試。 反之，使用這些環境來驗證組織現有工作流程的功能性。

* 涉及檔案的工作流程應專注於流程，而不是負載測試。 沙箱環境不支援大型檔案。

* [!DNL Workfront]自訂重新整理沙箱環境旨在永遠可用。 Workfront自訂重新整理沙箱環境在正常工作時間內發生的任何中斷，都是解決任何生產問題（如果存在）後立即優先考慮的事項。 Workfront自訂重新整理沙箱環境在週末（星期六和星期日）發生的任何中斷都會得到解決，因此環境會在星期一的營業時間執行。

* 校訂在自訂重新整理沙箱環境中不可用。

* 下列通知不適用於自訂重新整理沙箱環境：

   * 提醒通知
   * 自動延遲或提早提醒通知

### 商業規則注意事項

業務規則會刻意從Workfront預覽和沙箱環境重新整理中排除。 與大部分資料不同，Business Rules會被視為環境專屬設定，與使用者類似。 每個環境都可以維護一組根據其用途而量身打造的不同規則（例如，測試、開發或生產）。

在重新整理中加入Business Rules將會覆寫這些設定，可能會干擾管理員特意在非生產環境中設定的規則。

如果您需要在環境之間移動業務規則，請使用「環境升級」，它可讓您透過控制時間與範圍的選擇，轉移設定物件。 如需詳細資訊，請參閱[在Workfront環境之間移動物件的概述](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md)。

