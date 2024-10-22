---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: 授予「首頁」區域中物件的存取權
description: 使用者可以要求存取Adobe Workfront中的物件。 如需請求存取許可權的詳細資訊，請參閱請求物件的存取許可權。
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 授予「首頁」區域中物件的存取權

<!--Audited: 10/2024-->

使用者可以要求存取Adobe Workfront中的物件。

如需有關要求存取許可權的詳細資訊，請參閱[要求存取物件](../../workfront-basics/grant-and-request-access-to-objects/request-access.md)。

如果您是物件的擁有者，則可以在首頁區域授予或拒絕專案存取權。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p> 
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、任務、問題或檔案的存取權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案、任務、問題或檔案的許可權或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 授予「首頁」區域中物件的存取權

1. 按一下熒幕右上角的&#x200B;**主功能表** ![](assets/dots-main-menu.png)，或按一下左上角的&#x200B;**主功能表** ![](assets/lines-main-menu.png) （如果可用），然後按一下&#x200B;**首頁**
或
按一下Adobe Workfront左上角的**首頁**&#x200B;圖示![](assets/home-icon-30x29.png)。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對您環境中的「首頁」圖示進行下列變更：
   >
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來將會與本文中顯示的有所不同。
   >* 使用其他頁面取代連結至該頁面的頁面。 在此情況下，請按一下頁面右上角的&#x200B;**主要功能表** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**。

1. 執行下列動作：

   1. 移至&#x200B;**我的核准** Widget並尋找更多存取權的要求，然後按一下&#x200B;**授與存取權**。

      ![](assets/request-for-access-to-project-in-new-home-approvals-widget.png)

   1. （選擇性）若要授與不同層級的存取權，請按一下[授與存取權]按鈕左側的下拉式功能表，並選取新的存取權，然後按一下[授與存取權]。****

      存取請求被授予，並從核准請求清單中消失。

1. （選擇性）按一下&#x200B;**忽略**&#x200B;以拒絕存取。 未授予存取要求，且要求會從核准要求清單中消失。

## 設定存取請求的電子郵件通知

您可以設定是否要收到存取請求的電子郵件通知。 您的Workfront管理員可以停用此功能（如[為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)中所述）。

1. 執行下列任一項作業，前往您的使用者設定檔：

   * 按一下熒幕右上角的&#x200B;**主要功能表** ![](assets/dots-main-menu.png)，然後按一下您的名稱。
   * 按一下右上角的Adobe **主要功能表** ![](assets/adobe-blue-main-menu.png) （如果可用），然後按一下&#x200B;**Workfront設定檔**。

1. 按一下標題中您名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。
1. 按一下&#x200B;**通知**，然後選取或取消選取&#x200B;**需要動作**&#x200B;區段中的&#x200B;**某人向我要求存取權**，這取決於您是否要在其他使用者向您要求存取權時收到電子郵件通知。

   您可以啟用每日或即時通知。

1. 按一下「**儲存變更**」。

<!--1. (Conditional) From the legacy Home area, do the following: 
   
   1. In the **Work List**, select the access request you want to manage in the **Approvals** section.  

   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

   The request displays on the right of the Work List. 

   1. In the upper-right corner, click the grant access button.  
   Depending on the type of access requested, the button name changes. For example, if the requestor asks for View access, the button says **Grant View Access**.  
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

   1. (Optional) To grant a different level of access than requested, click the arrow next to the grant access button and select the new access, then click **Grant < Permission level > Access >**.  
   A message appears confirming access was granted.  
   
   1. (Optional) Click **Ignore** to deny access.  
   A message appears confirming access was ignored.-->
