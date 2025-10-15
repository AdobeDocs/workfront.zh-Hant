---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 使用電子郵件內容從Google Workspace更新 [!DNL Adobe Workfront] 專案
description: 您可以利用非Adobe Workfront電子郵件的資訊，更新現有的專案、任務或問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 使用電子郵件內容更新[!DNL Adobe Workfront]中的[!DNL Google Workspace]專案

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
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Google Workspace之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Gmail模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google行事曆模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

您可以從非[!DNL Adobe Workfront]電子郵件更新具有資訊的現有專案、任務或問題。

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
   <td> <p>標準</p><p>工作或更高</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先使用來自[!DNL Workfront]的電子郵件內容更新[!DNL Google Workspace]專案，然後才能進行更新

* 安裝[!DNL Workfront for Google Workspace]\
   如需指示，請參閱[安裝 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用來自[!DNL Workfront]的電子郵件內容更新[!DNL Google Workspace]專案

1. 如果未顯示Google Workspace[!UICONTROL 的]Workfront面板，請按一下頁面最右側![附加元件側邊欄中的Workfront圖示](assets/wf-lion-icon.png)Workfront圖示[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中開啟電子郵件訊息後，在&#x200B;**[!UICONTROL 面板中按一下]**&#x200B;張貼為新的更新[!DNL Google Workspace]。
1. 在&#x200B;**[!UICONTROL 型別]**&#x200B;下，按一下下拉箭頭，然後按一下您要新增更新的物件型別。
1. 按一下「**[!UICONTROL 搜尋]**」選項，開始輸入您要新增更新的物件名稱，然後選取出現在下列清單中的專案。

   此選項會依您在步驟3中所選取的專案而有所不同。 它可能是&#x200B;**[!UICONTROL 搜尋專案]**、**[!UICONTROL 搜尋任務]**&#x200B;或&#x200B;**[!UICONTROL 搜尋問題]**。

   >[!NOTE]
   >
   >當您輸入任務的名稱時，臨時個人任務會從下面顯示的名稱清單中排除。

1. 進行下列任一項選擇性變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 更新]</td> 
      <td>編輯此文字的任何部分，這些部分取自電子郵件的主旨行與內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 包含電子郵件附件]</td> 
      <td><p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項，將附件儲存在任務或問題的[!UICONTROL 檔案]索引標籤中。 </p><p>如果您不想儲存附件，請按一下附件名稱右側的X。 </p><p>如果電子郵件包含指向[!DNL Google Drive]中檔案的連結，則連結會儲存到您正在建立之任務或問題的[!UICONTROL 概觀]索引標籤。 </p><p>重要： <span style="color: #ff1493;"><span style="color: #000000;">若要讓此功能運作，您的</span></span>[!DNL Workfront]管理員<span style="color: #ff1493;"><span style="color: #000000;">必須授權[!DNL Google Drive]與[!DNL Workfront]</span></span>合作</p>
      <p>如果啟用此選項，則對於您轉換為任務、問題和更新的其他電子郵件，此選項仍保持啟用狀態。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>按一下<strong>[!UICONTROL 通知]</strong>，按一下出現的<strong>[!UICONTROL 搜尋使用者或團隊]</strong>選項，然後開始輸入人員或團隊的名稱，並在它出現在以下清單中時按一下它。 對您要新增的每個人和團隊重複此動作，然後按一下<strong>[!UICONTROL 儲存]</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 更新]**。

   當您重新整理瀏覽器時，訊息會在[!DNL Workfront for Google Workspace]面板底部顯示連結，確認您已轉換電子郵件為更新：

   您可以按一下連結，針對您在步驟4中指定的物件，移至[!UICONTROL 中的]更新[!DNL Workfront]標籤。

   您可以重複這些步驟，將相同的電子郵件轉換為更新、任務和問題(請參閱[在 [!DNL Google Workspace] 中建立一個Adobe Workfront問題](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在[!UICONTROL Google Workspace的Workfront]面板底部。

1. （選擇性）執行下列任一項作業，繼續在[!DNL Workfront]附加元件面板中處理更新：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上新增另一個更新，請按一下&#x200B;**[!UICONTROL 開始新的更新]**&#x200B;並輸入資訊。

   * 若要回覆&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上的更新，請按一下&#x200B;**[!UICONTROL 回覆]**，然後輸入您的回覆。

     對於上述兩個選項，您可以按一下&#x200B;**[!UICONTROL 通知]**，指定回覆的收件者，如步驟5所示。 準備就緒後，按一下&#x200B;**[!UICONTROL 貼文]**&#x200B;以新增更新或回覆。

   * 按一下「**[!UICONTROL 詳細資料]**」標籤，以檢視新專案、任務或問題的詳細資料。
