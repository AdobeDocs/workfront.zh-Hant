---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 使用電子郵件內容從Google Workspace更新 [!DNL Adobe Workfront] 專案
description: 您可以利用非Adobe Workfront電子郵件的資訊，更新現有的專案、任務或問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 使用電子郵件內容更新[!DNL Google Workspace]中的[!DNL Adobe Workfront]專案

>[!NOTE]
>
>Google適用的Adobe Workfront外掛程式最新版本已於2023年6月26日發行。

您可以從非[!DNL Adobe Workfront]電子郵件更新具有資訊的現有專案、任務或問題。

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

您必須先使用來自[!DNL Google Workspace]的電子郵件內容更新[!DNL Workfront]專案，然後才能進行更新

* 安裝[!DNL Workfront for Google Workspace]\
   如需指示，請參閱[安裝 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用來自[!DNL Google Workspace]的電子郵件內容更新[!DNL Workfront]專案

1. 如果未顯示Google Workspace]的[!UICONTROL Workfront面板，請按一下頁面最右側[!DNL Google Workspace]附加元件側邊欄中的Workfront圖示![](assets/wf-lion-icon.png)。
1. 在[!DNL Google Workspace]中開啟電子郵件訊息後，在[!DNL Google Workspace]面板中按一下&#x200B;**[!UICONTROL Post作為新更新]**。
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
      <td role="rowheader">[！UICONTROL更新]</td> 
      <td>編輯此文字的任何部分，這些部分取自電子郵件的主旨行與內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含電子郵件附件]</td> 
      <td><p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項，將附件儲存在任務或問題的[！UICONTROL檔案]索引標籤中。 </p><p>如果您不想儲存附件，請按一下附件名稱右側的X。 </p><p>如果電子郵件包含指向[!DNL Google Drive]中檔案的連結，則連結會儲存到您正在建立之任務或問題的[！UICONTROL概觀]索引標籤。 </p><p>重要： <span style="color: #ff1493;"><span style="color: #000000;">若要讓此功能運作，您的</span></span>[!DNL Workfront]管理員<span style="color: #ff1493;"><span style="color: #000000;">必須授權[!DNL Google Drive]與[!DNL Workfront]</span></span>合作</p>
      <p>如果啟用此選項，則對於您轉換為任務、問題和更新的其他電子郵件，此選項仍保持啟用狀態。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>按一下<strong>[！UICONTROL通知]</strong>，按一下出現的<strong>[！UICONTROL搜尋使用者或團隊]</strong>選項，然後開始輸入人員或團隊的名稱，並在它出現在以下清單中時按一下它。 對您要新增的每個人和團隊重複此動作，然後按一下<strong>[！UICONTROL儲存]</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 更新]**。

   當您重新整理瀏覽器時，訊息會在[!DNL Workfront for Google Workspace]面板底部顯示連結，確認您已轉換電子郵件為更新：

   您可以按一下連結，針對您在步驟4中指定的物件，移至[!DNL Workfront]中的[!UICONTROL 更新]標籤。

   您可以重複這些步驟，將相同的電子郵件轉換為更新、任務和問題(請參閱[在 [!DNL Google Workspace] 中建立一個Adobe Workfront問題](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在[!UICONTROL Google Workspace的Workfront]面板底部。

1. （選擇性）執行下列任一項作業，繼續在[!DNL Workfront]附加元件面板中處理更新：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上新增另一個更新，請按一下&#x200B;**[!UICONTROL 開始新的更新]**&#x200B;並輸入資訊。

   * 若要回覆&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上的更新，請按一下&#x200B;**[!UICONTROL 回覆]**，然後輸入您的回覆。

     對於上述兩個選項，您可以按一下&#x200B;**[!UICONTROL 通知]**，指定回覆的收件者，如步驟5所示。 準備就緒後，按一下&#x200B;**[!UICONTROL Post]**&#x200B;以新增更新或回覆。

   * 按一下「**[!UICONTROL 詳細資料]**」標籤，以檢視新專案、任務或問題的詳細資料。
