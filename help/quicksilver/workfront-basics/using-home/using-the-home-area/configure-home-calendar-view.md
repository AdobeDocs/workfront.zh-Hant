---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 配置您的「首頁日曆」視圖設定
description: 您可以配置「主日曆」設定，以便與基於web的Outlook版本整合，並幫助您根據可用工作時間跟蹤工作負載。
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 設定您的 [!UICONTROL 首頁日曆] 檢視設定

您可以設定 [!UICONTROL 首頁日曆] 設定以執行下列動作：

* 與網頁版整合 [!DNL Outlook] 雲端托管 [!DNL Office 365] 或 [!DNL Outlook Live]. 您可以在Outlook日曆中顯示所有事件以及您選擇的任何關聯日曆，如生日和節假日日曆 [!UICONTROL 首頁日曆].
* 幫助您根據工作時間跟蹤工作負載 [!UICONTROL 配置] 欄。

若要進一步了解「首頁行事歷」，請參閱 [[!UICONTROL 首頁日曆] 檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 關於整合 [!DNL Microsoft Outlook] 日曆

在使用 [!DNL Microsoft Outlook] 日曆：

* 您只能整合網頁版 [!DNL Outlook] 雲端托管 [!DNL Office 365] 或 [!DNL Outlook Live].

   內部部署 [!DNL Outlook] 和 [!DNL Outlook] 基於雲的企業 [!DNL Exchange] 不支援伺服器。

   如果貴組織使用單一登入，則您需要 [!DNL Microsoft 365 E3] 或 [!DNL E5].

* 與 [!DNL Outlook] 事件未附加至 [!DNL Outlook] 事件。
* 與 [!DNL Outlook] 每個使用者必須分別完成日曆。
* 顯示於 [!UICONTROL 到期] 欄未顯示在 [!DNL Microsoft] 除非您從 [!UICONTROL 工作清單] 至 [!DNL Adobe Workfront] 日曆。 如需詳細資訊，請參閱 [[!UICONTROL 到期] 條](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 和 [工作清單 [!UICONTROL 首頁日曆]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL 首頁日曆] 檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* 當您啟用與的整合時 [!DNL Outlook]，僅限拖曳至上的工作項目 [!UICONTROL 首頁日曆] 從那時開始，將同步。 在啟用整合之前位於「首頁行事歷」上的項目將不會顯示，而且如果要在中顯示，您必須再次將它們拖曳至「首頁行事歷」 [!DNL Outlook].
* 當您共用（或取消共用） [!DNL Outlook] 與他人共用的日曆，或當您更改與他人共用的日曆的權限級別時，此更改不會影響其日曆約30分鐘(有關詳細資訊，請參閱 [!DNL Microsoft Outlook] 檔案)。\
   因此，當您整合 [!DNL Workfront] 具有 [!DNL Outlook] 您與其他使用者共用的日曆，他們將看不到您的 [!DNL Workfront] 約30分鐘的日曆項。

>[!NOTE]
>
>此 [!DNL Outlook] 日曆設定與 [!DNL Outlook] 載入項([!UICONTROL [!DNL Outlook] 整合] 或 [!DNL Workfront Outlook])。 配置日曆不需要安裝，但需要安裝 [!DNL Outlook] 外接程式。 如需 [!DNL Outlook] 載入項請參閱 [設定 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## 設定您的 [!UICONTROL 首頁日曆] 檢視設定

1. 在 [!UICONTROL 首頁日曆] 檢視，按一下 **[!UICONTROL 設定]** 齒輪表徵圖 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) 在右上角開啟 **[!UICONTROL 日曆設定]** 面板。

   如果您需要有關存取 [!UICONTROL 首頁日曆] 檢視，請參閱 [檢視 [!UICONTROL 首頁日曆]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. （選用）若要整合您的 [!DNL Microsoft Outlook] 日曆，按一下 **[!UICONTROL 新增帳戶]** 在 **[!UICONTROL 日曆設定]** 中。 然後，如果系統提示您執行此操作，請輸入 [!DNL Microsoft Outlook] 登入資訊。 您可以重複此步驟以新增多個 [!DNL Outlook] 帳戶。

   >[!NOTE]
   >
   >你必須給 [!DNL Workfront] 存取您的 [!DNL Outlook] 日曆。 授予權限允許 [!DNL Workfront] 若要維護日曆資料的存取權，請閱讀 [!DNL outlook] 設定檔，並讀取和更新您的 [!DNL Microsoft] 日曆。

1. 重新整理瀏覽器視窗，查看您 [!DNL Outlook] 在日曆和 [!UICONTROL 日曆設定] 中。
1. 按一下 **[!UICONTROL 設定]** 齒輪圖示，以開啟 **[!UICONTROL 日曆設定]** 中。 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （選用）在 [!DNL Microsoft] 您在上一步驟中新增的帳戶，請選取 **[!UICONTROL 檢視]** 或 **[!UICONTROL 同步]**:

   * **[!UICONTROL 檢視]**:這是唯讀選項，會顯示 [!DNL Microsoft] 您的 [!UICONTROL 首頁日曆].
   * **[!UICONTROL 同步]**:此選項可讓您的 [!DNL Microsoft] 和 [!UICONTROL 首頁] 日曆。 換句話說， [!DNL Workfront] [!UICONTROL 首頁日曆] 項目匯出至 [!DNL Microsoft] 日曆和 [!DNL Microsoft] 匯入至Workfront的日曆項目 [!UICONTROL 首頁日曆] 即時。

      ![](assets/view-sync-checkboxes-qs.png)

1. （選用）在 [!DNL Workfront] 帳戶或整合帳戶，選擇要在您的 [!UICONTROL 首頁日曆] （例如您的PTO、生日或假日日曆），然後按一下瀏覽器的 [!UICONTROL 重新整理] 或 [!UICONTROL 重新載入] 按鈕，查看更改。

1. （選用）在 **[!UICONTROL 一般]** 一節 **[!UICONTROL 開始周於]**，請在「首頁日曆」中選取要顯示為一週中第一天的日期。

1. 設定下列選項：

   * **[!UICONTROL 我的工作日]:** 選擇您的工作日。
   * **[!UICONTROL 我通常的開始時間]:** 選擇開始工作日的時間。
   * **[!UICONTROL 我通常的結束時間]:** 選擇結束工作日的時間。

   [!DNL Workfront] 使用這三個設定來計算一週中的工作小時數。 此數字會影響 [!UICONTROL 配置] 欄，幫助您根據可用工作時間跟蹤工作量。 如需詳細資訊，請參閱 [[!UICONTROL 配置] 條](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) 在文章中 [[!UICONTROL 首頁日曆] 檢視](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. 按一下外部 **[!UICONTROL 日曆設定]** 要解除的區域。

   [!DNL Workfront] 會自動儲存您的變更。

如需使用 [!UICONTROL 日曆] 查看以管理您的工作分配和整合的日曆事件，請參閱 [使用 [!UICONTROL 首頁日曆] 檢視](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
