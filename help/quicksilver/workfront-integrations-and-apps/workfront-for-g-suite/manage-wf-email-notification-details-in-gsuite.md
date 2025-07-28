---
product-area: workfront-integrations
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 從Google Workspace管理 [!DNL Adobe Workfront] 通知詳細資料
description: 在Google Workspace中，當您開啟Adobe [!DNL Workfront] 已傳送的通知電子郵件時，可以檢視相關工作專案詳細資訊，並在不離開收件匣的情況下回應。 如果有可用動作（例如核准請求），您可以直接從適用於Google Workspace的Workfront執行這些動作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 管理來自[!DNL Adobe Workfront]的[!DNL Google Workspace]通知詳細資料

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，下列Google Workspace適用的Workfront功能在&#x200B;**2026年2月28日**&#x200B;後將無法使用：
>
>* 從Workfront存取Google Workspace功能
>
>* 從Gmail或Google行事曆網站面板檢視和管理Workfront工作
>
>為了滿足貴組織與Google Workspace的整合需求，我們建議您使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Google Workspace之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Gmail模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google行事曆模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

在[!DNL Google Workspace]中，當您開啟已傳送的通知電子郵件[!DNL Adobe Workfront]時，您可以檢視相關工作專案詳細資料並回應，而不需離開[!UICONTROL 收件匣]。 如果有可用動作（例如核准請求），您可以直接從[!DNL Workfront for Google Workspace]執行這些動作。

>[!NOTE]
>
> [!DNL Workfront for Google Workspace]支援您從[!DNL Workfront]收到的幾乎所有電子郵件通知型別（大約120種不同的型別）。 [!UICONTROL 每日摘要]從[!DNL Workfront]傳送的電子郵件未出現在[!DNL Workfront for Google Workspace]中。 如需[!DNL Workfront]電子郵件通知型別的相關資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL Work]， [！UICONTROL計畫]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

在您可以從[!DNL Google Workspace]管理通知詳細資料之前，您必須

* 安裝[!DNL Workfront for Google Workspace]\
   如需指示，請參閱[安裝 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 管理來自[!DNL Adobe Workfront]的[!DNL Google Workspace]通知詳細資料

1. 如果未顯示[!DNL Workfront for Google Workspace]面板，請按一下頁面最右側[!DNL Workfront]附加元件側邊欄中的![圖示](assets/wf-lion-icon.png)Workfront圖示[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中，開啟[!DNL Workfront]通知電子郵件。
1. 如果更新顯示在面板頂端附近，請按一下&#x200B;**[!UICONTROL 檢視所有更新]**。
1. 按一下&#x200B;**[!UICONTROL 詳細資料]**。
1. 按一下任何可用選項。

   可能顯示的選項與您已開啟的電子郵件通知型別有關。 例如，如果是要求您核准任務的電子郵件通知，您會看到&#x200B;**[!UICONTROL 核准]**&#x200B;和&#x200B;**[!UICONTROL 拒絕]**，而不是像&#x200B;**[!UICONTROL 處理它]**&#x200B;或&#x200B;**[!UICONTROL 完成]**&#x200B;之類的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>電子郵件通知型別</th> 
      <th>動作</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>任務或問題</td> 
      <td><strong>[！UICONTROL核准]</strong>它，<strong>[！UICONTROL拒絕]</strong>它，<strong>[！UICONTROL授予]</strong>存取它，<strong>[！UICONTROL忽略]</strong>存取它的要求，<strong>[！UICONTROL處理它]</strong>，或按一下選項以表示您有<strong>[！UICONTROL完成]</strong></td> 
     </tr> 
     <tr> 
      <td>專案</td> 
      <td><strong>[！UICONTROL核准]</strong>它，<strong>[！UICONTROL拒絕]</strong>它，<strong>[！UICONTROL授予]</strong>存取它或<strong>[！UICONTROL忽略]</strong>存取它的要求</td> 
     </tr> 
     <tr> 
      <td>文件</td> 
      <td><strong>[！UICONTROL核准]</strong>它，<strong>[！UICONTROL拒絕]</strong>它，<strong>[！UICONTROL授予]</strong>存取它或<strong>[！UICONTROL忽略]</strong>存取它的要求</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>檢視專案更新完整清單的任何部分，讓您的內容需要<strong>[！UICONTROL Post]</strong>新的更新或<strong>[！UICONTROL回覆]</strong>。 您可以按一下<strong>[！UICONTROL Notify]</strong>，提醒特定使用者您的回覆。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">回覆[!DNL Adobe Workfront]的[!DNL Google Workspace]</a>更新通知。</p> </td> 
     </tr> 
     <tr> 
      <td>核准請求</td> 
      <td><strong>[！UICONTROL核准]</strong>或<strong>[！UICONTROL拒絕]</strong>它（您可以按一下其他選項來改變您的想法）、下載、檢視其擁有者或檢視其參考號碼</td> 
     </tr> 
     <tr> 
      <td>專案狀態的變更</td> 
      <td> 檢視專案的所有目前資訊，包括任何自訂表格。 </td> 
     </tr> 
    </tbody> 
   </table>
