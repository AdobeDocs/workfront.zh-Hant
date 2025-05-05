---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: '為Microsoft Teams安裝 [!DNL Adobe Workfront] '
description: ' [!DNL Adobe Workfront for Microsoft Teams] 應用程式可讓您在 [!DNL Workfront] 中執行基本動作，而不需離開 [!DNL Microsoft Teams] 聊天頻道。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# 安裝Microsoft Teams的[!DNL Adobe Workfront]

<!-- Audited: 1/2024 -->

<!--

>[!IMPORTANT]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->


[!DNL Adobe Workfront for Microsoft Teams]應用程式可讓您在[!DNL Workfront]中執行基本動作，而不需離開[!DNL Microsoft Teams]聊天頻道。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支援[!DNL Internet Explorer]。 若要使用[!DNL Adobe Workfront for Microsoft Teams integration]，您必須使用[!DNL Internet Explorer]以外的網頁瀏覽器。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：標準</p>
    <p>目前： [!UICONTROL Work]， [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須是[!DNL Microsoft Teams]中的團隊擁有者才能為[!DNL Microsoft Teams]安裝[!DNL Workfront]。

## 安裝[!DNL Workfront for Microsoft Teams]

作為[!DNL Microsoft Teams]中的團隊擁有者，您可以從[!DNL Microsoft]市集或從[!DNL Workfront]提供的檔案為每個團隊安裝[!DNL Workfront for Microsoft Teams]應用程式。

### 從[!DNL Microsoft]存放區安裝[!DNL Workfront for Microsoft Teams]

1. 以團隊擁有者身分登入[!DNL Microsoft Teams]。
1. 選取您要為其安裝[!DNL Workfront for Microsoft Teams]應用程式的團隊。
1. 按一下側面導覽列上的&#x200B;**[!UICONTROL 商店]**。

1. 在&#x200B;**[!UICONTROL 搜尋全部]**&#x200B;方塊中，輸入&#x200B;*[!DNL Workfront]*。

1. 按一下&#x200B;**[!DNL Workfront]**&#x200B;卡片，然後依照精靈中的指示進行。
1. （建議）從&#x200B;**[!UICONTROL 新增至團隊]**&#x200B;下拉式選單中選取團隊，並啟用&#x200B;**[!UICONTROL 是]**&#x200B;選項以將應用程式新增至團隊。

   ![ms_teams_add_to_a_team_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. 針對頻道，選取「**[!UICONTROL 一般]**」以針對選取的團隊使用該頻道中的應用程式，然後按一下「**[!UICONTROL 設定]**」以取得您想要的功能。

1. 安裝完成時，您選取之團隊的[!UICONTROL 一般]頻道中會顯示安裝成功的通知。 團隊的所有成員都可以看到此通知。
1. （選擇性）釘選您的[!DNL Workfront]應用程式以更輕鬆存取：

   1. 按一下[!UICONTROL 一般]頻道中訊息欄位下的&#x200B;**[!UICONTROL 更多]**&#x200B;圖示。

   1. 將滑鼠移至清單中的[!DNL Workfront]應用程式上，然後按一下其右側的&#x200B;**[!UICONTROL 更多]**&#x200B;圖示。

   1. 按一下&#x200B;**[!UICONTROL 釘選]**。

      這會在聊天欄位下新增[!DNL Workfront]圖示。 您可以從這裡快速存取[!UICONTROL 搜尋]區域。

      如需搜尋[!DNL Workfront]專案的相關資訊，請參閱[搜尋並共用 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md)中的 [!DNL Adobe Workfront] 專案。

1. 按一下&#x200B;**[!UICONTROL 登入[!DNL Workfront]]**&#x200B;以存取[!DNL Workfront from Microsoft Teams]。

   如需有關登入[!DNL Workfront]的資訊，請參閱本文中的[從Microsoft Teams登入Workfront](#log-in-to-workfront-from-microsoft-teams)一節。

### 從私人檔案安裝[!DNL Workfront for Microsoft Teams]

如果您的組織限制從[!DNL Microsoft]市集下載應用程式的存取權，您必須連絡我們的支援團隊，並要求[!DNL Workfront for Microsoft Teams]應用程式的私人檔案以安裝應用程式。

如需連絡支援團隊的詳細資訊，請參閱[連絡客戶支援](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。

若要從私人檔案安裝[!DNL Workfront for Microsoft Teams]：

1. 將您從[!DNL Workfront]收到的私人檔案儲存在電腦上。
1. 以[!DNL Microsoft]團隊擁有者的身分登入[!DNL Microsoft Teams]。
1. 按一下您要安裝[!DNL Workfront for Microsoft Teams]之團隊的&#x200B;**[!UICONTROL 更多]**&#x200B;圖示。

1. 按一下&#x200B;**[!UICONTROL 管理團隊]**。
1. 選取「**[!UICONTROL 應用程式]**」標籤，然後按一下畫面右下角的「**[!UICONTROL 上傳自訂應用程式]**」。

1. 瀏覽您儲存在電腦上的私人檔案，然後依照安裝步驟安裝[!DNL Workfront for Microsoft Teams]。
1. 安裝完成後，您選取之團隊的「一般」頻道中會顯示安裝成功的通知。 團隊的所有成員都可以看到此通知。
1. （選擇性）按一下&#x200B;**[!UICONTROL 在此輸入您的問題]**&#x200B;欄位下的&#x200B;**[!UICONTROL 更多]** （三點）圖示。

1. （選用）將滑鼠移至清單中的[!DNL Workfront]應用程式上，然後按一下其右側的&#x200B;**[!UICONTROL 更多]**&#x200B;圖示。

1. （選擇性）按一下&#x200B;**[!UICONTROL 釘選]**。

   這會在[!UICONTROL 在這裡輸入您的問題]欄位底下新增[!DNL Workfront]圖示。 您可以從這裡快速存取[!UICONTROL 搜尋]區域。\
   如需有關搜尋Workfront專案的資訊，請參閱[搜尋並共用 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md)中的 [!DNL Adobe Workfront] 專案。

## 從[!DNL Microsoft]團隊登入[!DNL Workfront]

您身為[!DNL Microsoft Teams]團隊擁有者，必須先為團隊安裝[!DNL Workfront for Microsoft Teams]應用程式，您或團隊中的任何人員才能登入[!DNL Workfront from Microsoft Teams]。

當您從[!DNL Microsoft Teams]登入[!DNL Workfront]時，您可以在[!DNL Workfront]機器人頻道中接收[!DNL Workfront]個通知，或者您可以從[!DNL Microsoft Teams]在[!DNL Workfront]中執行某些動作。

如需有關安裝[!DNL Workfront]應用程式的資訊，請參閱本文中的[安裝 [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams)一節。

如需有關從[!DNL Microsoft Teams]存取[!DNL Workfront]以執行特定動作的資訊，請參閱[從 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md)存取 [!DNL Adobe Workfront] 。

若要從[!DNL Microsoft Teams]登入[!DNL Workfront]：

1. 前往已安裝[!DNL Workfront for Microsoft Teams]應用程式的團隊之&#x200B;**[!UICONTROL 一般]**&#x200B;頻道，然後按一下&#x200B;**[!UICONTROL 登入Workfront]**。

   [!DNL Workfront]機器人聊天頻道已新增到您的[!DNL Microsoft Teams]聊天頻道。

1. 移至[!DNL Microsoft Teams]中的[!DNL Workfront]機器人聊天頻道，並在&#x200B;**[!UICONTROL 在此輸入您的問題]**&#x200B;欄位中輸入&#x200B;*[!UICONTROL 登入]*。

   或

   按一下&#x200B;**[!UICONTROL 登入]**。

   新的瀏覽器標籤隨即開啟。

1. 依照提示使用Enhanced Authentication、OAuth 2.0或您的安全性宣告標籤語言(SAML) URL登入[!DNL Workfront]。

   >[!NOTE]
   >
   >* 當系統提示您輸入[!DNL Workfront]帳戶的網域時，請使用此格式輸入它： *yourCompany&#39;sDomain.my.workfront.com*。 您公司的網域通常是您公司的名稱。
   >* 增強式驗證必須由[!DNL Workfront]系統管理員針對這項整合啟用才能使用。


1. 關閉您用來登入的瀏覽器標籤並返回[!DNL Microsoft Teams]。

   [!DNL Workfront]機器人聊天頻道中會顯示通知，以確認您已成功登入[!DNL Workfront]。
