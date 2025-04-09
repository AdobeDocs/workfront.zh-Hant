---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: '為Microsoft團隊安裝 [!DNL Adobe Workfront] '
description: 該應用程式 [!DNL Adobe Workfront for Microsoft Teams] 允許您在不離開 [!DNL Microsoft Teams] 聊天頻道的情況下執行基本作 [!DNL Workfront] 。
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 41d898e82bc5b06498966ba938b68ed10e742d3b
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# 安裝Microsoft Teams的[!DNL Adobe Workfront]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>自2025年7月1日起，Microsoft將移除對Classic Teams案頭應用程式的支援。 因此，Classic Teams案頭應用程式無法使用後，將不支援Workfront與Microsoft Teams的整合。


該應用程式[!DNL Adobe Workfront for Microsoft Teams]允許您在不離開[!DNL Microsoft Teams]聊天頻道的情況下執行基本作[!DNL Workfront]。

>[!NOTE]
>
>[!DNL Microsoft Teams] 不再支援 [!DNL Internet Explorer]. [!DNL Adobe Workfront for Microsoft Teams integration]要使用 ，您必須使用 Web 瀏覽器 [!DNL Internet Explorer]以外的其他 Web 。


## 存取需求

+++ 展開以視圖本文中功能的訪問要求。

您必須具有以下存取權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 許可證</td> 
   <td><p>新：標準</p>
    <p>當前：[！UICONTROL 工作]、[！UICONTROL 計劃]</p> </td> 
  </tr> 
 </tbody> 
</table>

有關此表中資訊的更多詳細資訊，請參閱 [Workfront 文件中](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)的訪問要求。

+++

## 先決條件

您必須是[!DNL Microsoft Teams]中的團隊擁有者才能為[!DNL Microsoft Teams]安裝[!DNL Workfront]。

## 安裝[!DNL Workfront for Microsoft Teams]

作為[!DNL Microsoft Teams]中的團隊擁有者，您可以從[!DNL Microsoft]市集或從[!DNL Workfront]提供的檔案為每個團隊安裝[!DNL Workfront for Microsoft Teams]應用程式。

### 從應用程式商店安裝[!DNL Workfront for Microsoft Teams] [!DNL Microsoft]

1. 以團隊所有者身分登入 [!DNL Microsoft Teams] 。
1. 選擇要為其安裝 [!DNL Workfront for Microsoft Teams] 應用程式團隊。
1. 按一下側面導覽列上的&#x200B;**[!UICONTROL 商店]**。

1. 在&#x200B;**[!UICONTROL 搜尋全部]**&#x200B;方塊中，輸入&#x200B;*[!DNL Workfront]*。

1. 按一下&#x200B;**[!DNL Workfront]**&#x200B;卡片，然後依照精靈中的指示進行。
1. （建議）從&#x200B;**[!UICONTROL 新增至團隊]**&#x200B;下拉式選單中選取團隊，並啟用&#x200B;**[!UICONTROL 是]**&#x200B;選項以將應用程式新增至團隊。

   ![ms_teams_add_to_a_團隊_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. 對於通道，選擇「常規&#x200B;]**」**[!UICONTROL &#x200B;以使用該通道中的應用程式用於所選團隊，然後按兩下&#x200B;**[!UICONTROL 設置]**「以選擇所需的功能。

1. 安裝完成後，所選團隊的「常規]」通道中將顯示安裝[!UICONTROL 成功的通知。團隊的所有成員都可以看到此通知。
1. （選擇）固定應用程式 [!DNL Workfront] 以便輕鬆存取：

   1. **[!UICONTROL 按一般]通道中[!UICONTROL 留言欄位下方的更多]**&#x200B;圖示。

   1. 將滑鼠移到應用程式上方[!DNL Workfront]清單，然後按下其右側的「更多」****&#x200B;圖示。

   1. 按兩下&#x200B;**[!UICONTROL 「釘選」。]**

      這會在聊天欄位下添加一個 [!DNL Workfront] 圖示。 您可以從此處快速訪問 [!UICONTROL Search] 區域。

      有關搜索 [!DNL Workfront] 專案的資訊，請參閱 [Search和共享 [!DNL Adobe Workfront] 專案 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md)。

1. 點選 **[!UICONTROL 登入以[!DNL Workfront]]** 存取 [!DNL Workfront from Microsoft Teams]。

   如需有關登入[!DNL Workfront]的資訊，請參閱本文中的[從Microsoft Teams登入Workfront](#log-in-to-workfront-from-microsoft-teams)一節。

### 從私人檔案安裝[!DNL Workfront for Microsoft Teams]

如果您的組織限制從[!DNL Microsoft]市集下載應用程式的存取權，您必須連絡我們的支援團隊，並要求[!DNL Workfront for Microsoft Teams]應用程式的私人檔案以安裝應用程式。

有關聯繫我們的支持團隊的資訊，請參閱 [聯繫客戶支援](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。

要從私有文件安裝 [!DNL Workfront for Microsoft Teams] ，請執行以下作：

1. 儲存您從 [!DNL Workfront] 電腦上收到的私人文件。
1. 以[!DNL Microsoft]團隊擁有者的身分登入[!DNL Microsoft Teams]。
1. 按一下您要安裝[!DNL Workfront for Microsoft Teams]之團隊的&#x200B;**[!UICONTROL 更多]**&#x200B;圖示。

1. 按一下&#x200B;**[!UICONTROL 管理團隊]**。
1. 選取「**[!UICONTROL 應用程式]**」標籤，然後按一下畫面右下角的「**[!UICONTROL 上傳自訂應用程式]**」。

1. 瀏覽您儲存在電腦上的私人檔案，然後依照安裝步驟安裝[!DNL Workfront for Microsoft Teams]。
1. 安裝完成後，所選團隊的「常規」通道中將顯示安裝成功的通知。 團隊的所有成員都可以看到此通知。
1. （選擇）**[!UICONTROL 按兩下在此處輸入您的問題]**&#x200B;欄位&#x200B;**[!UICONTROL 下方的更多]**（三個點）圖示。

1. （選擇）將滑鼠移到應用程式上方[!DNL Workfront]清單，然後按下其右側的「更多」****&#x200B;圖示。

1. （選擇）按兩下&#x200B;**[!UICONTROL 「釘選」。]**

   這將在在此處]輸入您的問題欄位[!UICONTROL 下添加一個[!DNL Workfront]圖示。您可以從這裡快速存取[!UICONTROL 搜尋]區域。\
   如需有關搜尋Workfront專案的資訊，請參閱[搜尋並共用 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md)中的 [!DNL Adobe Workfront] 專案。

## 從[!DNL Microsoft]團隊登入[!DNL Workfront]

您身為[!DNL Microsoft Teams]團隊擁有者，必須先為團隊安裝[!DNL Workfront for Microsoft Teams]應用程式，您或團隊中的任何人員才能登入[!DNL Workfront from Microsoft Teams]。

當您從[!DNL Microsoft Teams]登入[!DNL Workfront]時，您可以在[!DNL Workfront]機器人頻道中接收[!DNL Workfront]個通知，或者您可以從[!DNL Microsoft Teams]在[!DNL Workfront]中執行某些動作。

有關安裝 [!DNL Workfront] 應用的資訊，請參閱 [本文中的“安裝 [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) ”部分。

有關從訪問 [!DNL Workfront] 以 [!DNL Microsoft Teams] 執行某些作的資訊，請參閱 [訪問 [!DNL Adobe Workfront] 自 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md)。

若要從 [!DNL Microsoft Teams]登入[!DNL Workfront]：

1. 轉到&#x200B;**[!UICONTROL 已安裝應用程式團隊[!DNL Workfront for Microsoft Teams]的「常規]**&#x200B;通道」，然後按下「**[!UICONTROL 登錄到 Workfront]**」。。

   [!DNL Workfront]機器人聊天頻道已新增到您的[!DNL Microsoft Teams]聊天頻道。

1. 移至[!DNL Microsoft Teams]中的[!DNL Workfront]機器人聊天頻道，並在&#x200B;**[!UICONTROL 在此輸入您的問題]**&#x200B;欄位中輸入&#x200B;*[!UICONTROL 登入]*。

   或

   按兩下「 **[!UICONTROL 登入]**」。

   此時會開啟一個新的瀏覽器標籤。

1. 按照提示登錄， [!DNL Workfront] 使用增強Authentication、OAuth 2.0 或安全斷言標記語言 （SAML） URL登錄。

   >[!NOTE]
   >
   >* 當系統提示您輸入帳戶域 [!DNL Workfront] 時，請使用以下格式鍵入它： *yourCompany&#39;sDomain.my.workfront.com*。 公司的網域通常是您公司的名稱。
   >* 增強Authentication在管理員啟用此整合後方 [!DNL Workfront] 可使用。


1. 關閉您用來登入並返回 [!DNL Microsoft Teams]的瀏覽器標籤。

   機器人聊天通道中 [!DNL Workfront] 會顯示一個通知，以確認您已成功登錄 [!DNL Workfront] 。
