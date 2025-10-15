---
navigation-topic: notifications
title: 啟用從預覽Sandbox環境傳送電子郵件
description: 如果您想從預覽Sandbox環境接收電子郵件通知，您必須在登入預覽時在使用者設定中啟用此功能。
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# 啟用從預覽Sandbox環境傳送電子郵件

[!UICONTROL Adobe Workfront]會停用預覽和自訂重新整理沙箱環境的所有電子郵件通訊。 如需有關預覽沙箱環境的資訊，請參閱[Adobe Workfront預覽沙箱環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。 如需自訂重新整理沙箱環境的詳細資訊，請參閱[Adobe Workfront自訂重新整理沙箱環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。

如果您想從預覽Sandbox環境接收以下電子郵件通知，您必須在登入預覽時在使用者設定中啟用此功能：

* 事件通知觸發的電子郵件通知
* 提醒通知
* 自動延遲或提早提醒通知
* 電子郵件邀請

您可以自行或為您有權編輯的任何使用者執行此操作。 如需編輯使用者所需存取許可權的詳細資訊，請參閱[授予使用者存取許可權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

>[!NOTE]
>
>行動應用程式上的報告傳送和推播通知一律會在預覽沙箱環境中停用。 存取預覽沙箱環境時，您和[!DNL Workfront]管理員都無法啟用行動應用程式的報告傳遞或推播通知。
>
>如需報告傳送的相關資訊，請參閱[報告傳送概述](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td> 
   <p>投稿人或以上人員變更您自己的設定</p> <p>用於編輯其他使用者的設定的標準</p> 
   或
   <p> 要求或更高版本變更您自己的設定</p> <p>計畫編輯其他使用者的設定</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>[!UICONTROL 系統管理員]存取層級。</p> </li> 
     <li> <p>在您的存取層級中，必須為[!UICONTROL 使用者]設定選取[!UICONTROL 編輯] 。 此外，針對[!UICONTROL 使用者]設定，在[!UICONTROL 微調您的設定] <img src="assets/gear-icon-in-access-levels.png">下，必須啟用[!UICONTROL 建立]選項以及兩個[!UICONTROL 使用者管理]選項中的至少一個。 </li> 
     <li>如果您使用[!UICONTROL 使用者管理員（群組使用者）]選項，您必須是使用者所屬群組的群組管理員。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 啟用從預覽Sandbox環境的電子郵件傳送

1. 登入您的預覽Sandbox環境。
1. 按一下[!DNL Adobe Workfront]右上角的設定檔圖片。 然後，按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表並選取&#x200B;**[!UICONTROL 編輯]**。

   或

   在[!DNL Workfront]中搜尋使用者，然後按一下其名稱。 然後，按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表並選取&#x200B;**[!UICONTROL 編輯]**。

   或

   針對多位使用者：按一下Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 使用者]** ![使用者圖示](assets/users-icon-in-main-menu.png)。  然後，選取多位使用者並按一下&#x200B;**[!UICONTROL 編輯]**。

1. 按一下&#x200B;**[!UICONTROL 偏好設定]**。
1. 選取&#x200B;**[!UICONTROL 接收來自此測試環境的電子郵件]**。

   >[!NOTE]
   >
   >如果您在生產環境中，則無法使用此選項。

1. 按一下「**[!UICONTROL 儲存變更]**」。
