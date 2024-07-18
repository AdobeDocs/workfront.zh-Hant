---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 設定您的首頁行事曆檢視設定
description: 您可以設定[首頁行事曆]設定，以與Outlook網頁版整合，並協助您根據可用工作時數追蹤工作負載。
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 設定您的[!UICONTROL 首頁行事曆]檢視設定

<!--Audited: 01/2024-->

您可以設定[!UICONTROL 首頁行事曆]設定，以執行下列動作：

* 與雲端託管的 [!DNL Office 365] 或 [!DNL Outlook Live] 之網頁版 [!DNL Outlook] 整合。您可以在Adobe Workfront中顯示Outlook行事曆的所有活動，以及您在[!UICONTROL 首頁行事曆]中選取的任何相關行事曆。
* 協助您根據[!UICONTROL 配置]列上的可用工作時數追蹤工作負載。

若要深入瞭解首頁行事曆，請參閱[[!UICONTROL 首頁行事曆]檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)。

本文說明如何設定首頁行事曆設定，以及如何將首頁行事曆與外部Outlook行事曆整合。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>目前： [！UICONTROL Work]或更高版本</p> 
   或
   <p>新增：[！UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*若要瞭解您擁有的計畫或授權型別，請連絡您的[!DNL Workfront]管理員。 如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於整合[!DNL Microsoft Outlook]行事曆

當您使用[!DNL Microsoft Outlook]行事曆設定首頁行事曆時，請考慮下列事項：

* 您只能在雲端託管的[!DNL Office 365]或[!DNL Outlook Live]中整合[!DNL Outlook]的網頁型版本。

  不支援雲端型企業[!DNL Exchange]伺服器上的內部部署[!DNL Outlook]和[!DNL Outlook]。

  如果您的組織使用單一登入，您需要[!DNL Microsoft 365 E3]或[!DNL E5]。

* 與您的[!DNL Outlook]活動關聯的附件未附加到您的首頁行事曆中的[!DNL Outlook]活動。
* 必須為每個使用者個別完成與[!DNL Outlook]行事曆的整合。
* 出現在[!UICONTROL 到期]列中的事件不會出現在您的[!DNL Microsoft]行事曆上，除非您將其從[!UICONTROL 工作清單]拖曳到您的[!DNL Adobe Workfront]行事曆。 如需詳細資訊，請參閱[[!UICONTROL 首頁行事曆]檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)中[!UICONTROL 首頁行事曆]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view)的[[!UICONTROL 到期]列](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar)和[工作清單。

* 當您啟用與[!DNL Outlook]的整合時，只有從該時間點開始拖曳至[!UICONTROL 首頁行事曆]的工作專案才會同步。 在啟用整合之前位於首頁行事曆上的專案將不會顯示，如果您希望這些專案在[!DNL Outlook]中顯示，必須將其拖曳到首頁行事曆上。
* 當您與其他人共用（或取消共用） [!DNL Outlook]行事曆，或變更與其他人共用行事曆的許可權層級時，此變更不會影響其行事曆約30分鐘。 如需詳細資訊，請參閱[!DNL Microsoft Outlook]檔案。\
   因此，當您將[!DNL Workfront]行事曆與您與其他使用者共用的[!DNL Outlook]行事曆整合時，他們將在大約30分鐘內看不到您的[!DNL Workfront]行事曆專案。

>[!NOTE]
>
>[!DNL Outlook]行事曆設定與[!DNL Outlook]增益集完全不同（[!UICONTROL [!DNL Outlook]整合]或[!DNL Workfront Outlook]）。 設定行事曆不需要安裝，但[!DNL Outlook]增益集需要安裝。 如需[!DNL Outlook]增益集的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)。

## 設定您的[!UICONTROL 首頁行事曆]檢視設定，並將其與Outlook行事曆整合

1. 在[!UICONTROL 首頁行事曆]檢視中，按一下右上角的&#x200B;**[!UICONTROL 設定]**&#x200B;齒輪圖示![行事曆設定_齒輪圖示.png](assets/calendar-settings-gear-icon.png)以開啟右邊的&#x200B;**[!UICONTROL 行事曆設定]**&#x200B;面板。

   如果您需要有關存取[!UICONTROL 首頁行事曆]檢視的資訊，請參閱[檢視[!UICONTROL 首頁行事曆]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)。

1. （選擇性）若要整合您的[!DNL Microsoft Outlook]行事曆，請按一下&#x200B;**[!UICONTROL 行事曆設定]**&#x200B;面板右上角的&#x200B;**[!UICONTROL 新增帳戶]**。 然後，如果系統提示您這樣做，請輸入您的[!DNL Microsoft Outlook]登入資訊。 您可以重複此步驟以新增多個[!DNL Outlook]帳戶。

   >[!NOTE]
   >
   >您必須授予[!DNL Workfront]許可權才能存取您的[!DNL Outlook]行事曆。 授與許可權可讓[!DNL Workfront]保持行事曆資料的存取權、讀取您的[!DNL outlook]設定檔，以及讀取和更新您的[!DNL Microsoft]行事曆。

1. 重新整理瀏覽器視窗以在行事曆和[!UICONTROL 行事曆設定]面板中檢視您[!DNL Outlook]帳戶的資訊。
1. 再按一下右上角的&#x200B;**[!UICONTROL 設定]**&#x200B;齒輪圖示以開啟&#x200B;**[!UICONTROL 行事曆設定]**&#x200B;面板。 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （選擇性）在您在上一步中新增的每個[!DNL Microsoft]帳戶下，選取&#x200B;**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 同步]**：

   * **[!UICONTROL 檢視]**：這是唯讀選項，會在您的[!UICONTROL 首頁行事曆]上顯示[!DNL Microsoft]個行事曆事件。
   * **[!UICONTROL 同步]**：此選項允許在您的[!DNL Microsoft]和[!UICONTROL 首頁]行事曆之間進行雙向同步。 換句話說，[!DNL Workfront]個[!UICONTROL 首頁行事曆]專案會匯出至您的[!DNL Microsoft]行事曆，而[!DNL Microsoft]個行事曆專案會匯入您的Workfront [!UICONTROL 首頁行事曆]即時完成。

     ![](assets/view-sync-checkboxes-qs.png)

1. （選擇性）在您的[!DNL Workfront]帳戶或整合帳戶下，選取您想要在[!UICONTROL 首頁行事曆]上檢視的相關行事曆（例如您的PTO、生日或節假日行事曆），然後按一下瀏覽器的[!UICONTROL 重新整理]或[!UICONTROL 重新載入]按鈕以檢視您的變更。

1. （選擇性）在&#x200B;**[!UICONTROL 每週開始日期]**&#x200B;下的&#x200B;**[!UICONTROL 一般]**&#x200B;區段中，選取您要在首頁行事曆中顯示為工作週第一天的日期。

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 設定下列選項：

   * **[!UICONTROL 我的工作日]：**&#x200B;選取您工作的日。
   * **[!UICONTROL 我的日常開始時間]：**&#x200B;選取您開始工作日的時間。
   * **[!UICONTROL 我的日常結束時間]：**&#x200B;選取您結束工作日的時間。

   [!DNL Workfront]會使用這三個設定來計算您一週的工作時數。 此數字會影響[!UICONTROL 配置]列，可協助您根據可用工作時數追蹤工作負載。 如需詳細資訊，請參閱文章[[!UICONTROL 首頁行事曆]檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)中的[[!UICONTROL 配置]列](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time)。

1. 按一下&#x200B;**[!UICONTROL 行事曆設定]**&#x200B;區域外部以關閉它。

   [!DNL Workfront]會自動儲存您的變更。

如需使用[!UICONTROL 行事曆]檢視來管理您的工作指派和整合行事曆事件的相關資訊，請參閱[使用[!UICONTROL 首頁行事曆]檢視](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md)。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
