---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 設定 [!DNL Adobe Workfront] 使用者的 [!DNL Salesforce] 區段
description: 當您以 [!DNL Adobe Workfront] 管理員身分安裝Salesforce的 [!DNL Workfront] 後，您可以將其新增至使用者在Salesforce中的「商機」和「帳戶」頁面配置的新區段，讓使用者可以使用它。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# 設定[!DNL Adobe Workfront]使用者的[!DNL Salesforce]區段

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Salesforce整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>為了滿足貴組織與Salesforce的整合需求，我們建議您使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Salesforce之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Salesforce模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

當您以[!DNL Adobe Workfront]管理員身分安裝[!DNL Salesforce]的[!DNL Workfront]後，您可以將其新增至使用者的[!UICONTROL 機會]和[!UICONTROL 帳戶]的新區段，讓使用者可以使用它
[!UICONTROL Salesforce]中的版面配置。

如需有關安裝[!DNL Workfront for Salesforce]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

若要讓使用者在[!DNL Workfront]和[!DNL Classic]架構中同時具有[!DNL Lightning Experience]可用，您必須分別將[!DNL WorkfrontOpportunities]和[!DNL WorkfrontAccounts] [!UICONTROL Visualforce]頁面新增至[!UICONTROL Opportunity]和[!UICONTROL Accounts]頁面配置。



## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>規劃</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 您必須擁有可存取系統管理員帳戶的[!DNL Salesforce]執行個體。
* 您必須擁有可存取系統管理員帳戶的[!DNL Workfront]執行個體。

## 在[!DNL Workfront]架構中設定[!DNL Salesforce Classic]區段

1. 以Workfront管理員身分登入[!DNL Salesforce]。
1. 按一下&#x200B;**[!UICONTROL 設定].**
1. 在&#x200B;**[!UICONTROL 建置]**&#x200B;區段中，展開&#x200B;**[!UICONTROL 自訂].**

1. 展開&#x200B;**[!UICONTROL 商機]**，然後按一下&#x200B;**[!UICONTROL 頁面配置]**，將[!DNL Workfront]區段新增至商機。

   或

   展開&#x200B;**[!UICONTROL 帳戶]**，然後按一下&#x200B;**[!UICONTROL 頁面配置]**，將[!DNL Workfront]區段新增至帳戶
.

1. 按一下現有配置上的&#x200B;**[!UICONTROL 編輯]**。

   或

   按一下&#x200B;**[!UICONTROL 新增]**&#x200B;以新增配置。

1. （選用）將&#x200B;**[!UICONTROL Section]**&#x200B;元件拖曳到版面配置中，並將它拖曳到需要的位置。\

1. （選擇性）指定新區段的名稱。

   我們建議您將此區段命名為&#x200B;**[!DNL Workfront]**。

1. （選擇性）為新區段指定所需的&#x200B;**[!UICONTROL 配置]**&#x200B;和&#x200B;**[!UICONTROL Tab鍵順序]**。

   建議您為&#x200B;**[!UICONTROL 區段選取]** 1欄[!DNL Workfront]配置。

1. 按一下&#x200B;**[!UICONTROL 「確定」]**。
1. 在&#x200B;**[!UICONTROL 配置]**&#x200B;區域中，按一下&#x200B;**[!UICONTROL Visualforce頁面].**

1. 將&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;元件拖放至&#x200B;**[!UICONTROL 機會]**&#x200B;配置中的新區段。

   或

   將&#x200B;**[!UICONTROL WorkfrontAccounts]**&#x200B;元件拖放到&#x200B;**[!UICONTROL 帳戶]**&#x200B;配置中的新區段。\

1. 按一下新新增的元件右上角的&#x200B;**[!UICONTROL 屬性]**&#x200B;圖示。\

1. 若要達到最佳顯示，請為[!DNL Workfront Visualforce]頁面指定下列屬性：

   * **[!UICONTROL 寬度（以畫素或%）]**： 100%
   * **[!UICONTROL 高度（畫素）]**： 600
   * 選取&#x200B;**[!UICONTROL 顯示卷軸]**。

1. 按一下&#x200B;**[!UICONTROL 「確定」]**。
1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您的版面。

   所有已指派此配置的使用者現在都可以檢視其[!DNL Workfront]機會[!UICONTROL 或]帳戶[!UICONTROL 物件上的]區段。

   使用者在[!DNL Workfront]區段上看到[!DNL Workfront]登入畫面。 如果他們沒有[!DNL Workfront]帳戶，則可以摺疊該區段，但無法從其版面配置中移除該區段。

## 在[!DNL Workfront]架構中設定[!DNL Salesforce Lightning Experience]區段

您可以將[!DNL Workfront]區段新增至[!DNL Salesforce] [!UICONTROL 商機]或帳戶的配置
在[!DNL Salesforce Lightning Experience]架構中，存取[!UICONTROL Setup]區域或帳戶進行存取
或[!UICONTROL 機會]物件。

* [在 [!DNL Workfront] 設定[!UICONTROL 層級設定]區段](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [在機會或帳戶層級設定 [!DNL Workfront] 區段](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### 在[!DNL Workfront]設定[!UICONTROL 層級設定]區段 {#configure-the-workfront-section-at-the-setup-level}

1. 以系統管理員身分登入[!DNL Salesforce]。
1. 按一下&#x200B;**[!UICONTROL 設定]**&#x200B;圖示，然後按一下&#x200B;**[!UICONTROL 設定]**。

1. 展開&#x200B;**[!UICONTROL 物件和欄位]**，然後按一下&#x200B;**[!UICONTROL 物件管理員]**。

1. 按一下「**[!UICONTROL 商機]**」以自訂商機的配置。

   或

   按一下&#x200B;**[!UICONTROL 帳戶]**&#x200B;以自訂帳戶的配置。

1. 按一下&#x200B;**[!UICONTROL 頁面配置]**。
1. 按一下現有頁面配置的名稱以進行編輯。

   或

   按一下[新增]&#x200B;**&#x200B;**&#x200B;以建立新的版面配置。

1. 繼續進行[在以下的機會或帳戶層級 [!DNL Workfront] 設定](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)區段。

### 在機會或帳戶層級設定[!DNL Workfront]區段 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. 以系統管理員身分登入[!DNL Salesforce]。
1. 移至&#x200B;**[!UICONTROL 商機]**&#x200B;或&#x200B;**[!UICONTROL 帳戶]**。

1. 按一下&#x200B;**[!UICONTROL 設定]**&#x200B;圖示，然後按一下&#x200B;**[!UICONTROL 編輯頁面]**。

1. 展開&#x200B;**[!UICONTROL 自訂管理]**&#x200B;區段。
1. 將&#x200B;**[!DNL Workfront]**&#x200B;元件拖放到您的[!UICONTROL 機會]或帳戶上
頁面。

   我們建議對[!DNL Workfront]區段使用頁面的完整寬度，而不是配置的其中一個欄。

1. 按一下「**[!UICONTROL 儲存]**」。

   所有已指派此配置的使用者現在都可以檢視其[!DNL Workfront]機會[!UICONTROL 或]帳戶[!UICONTROL 物件上的]區段。

   >[!NOTE]
   >
   >使用者在[!DNL Workfront]區段上看到[!DNL Workfront]登入畫面。 如果他們沒有[!DNL Workfront]帳戶，則可以摺疊該區段，但無法從其版面配置中移除該區段。 使用者可以使用您已啟用的驗證方法登入：增強式驗證或您的安全性宣告標籤語言(SAML) URL。

