---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 將處理它按鈕取代為開始按鈕
description: Adobe Workfront的預設設定包含處理它的一個按鈕，用於顯示已指派給您的專案的任務和問題。
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 以[!UICONTROL 開始]按鈕取代[!UICONTROL 處理它]按鈕

[!DNL Adobe Workfront]的預設設定包含針對指派給您的專案所顯示之任務與問題的[!UICONTROL 處理它]按鈕。 當您在指派給您的專案上按一下[!UICONTROL 處理它]時，您會向其他使用者表示您已收到工作，並認可您會處理它。 但是，[!DNL Work On It]按鈕不會更新任務或問題狀態以表示工作實際上已開始。

您可以為您所屬的團隊將[!DNL Work On It]按鈕取代為[!UICONTROL 開始]按鈕。 在此情況下，您按一下[!UICONTROL 開始]按鈕而非[!UICONTROL 處理它]，這會自動更新工作專案的狀態和[!UICONTROL 實際開始日期]，表示您已開始工作。 如需有關哪個團隊的設定可能會影響您在[!UICONTROL 處理它]按鈕中的變更的資訊，請參閱本文章的[設定[!UICONTROL 開始]按鈕](#configure-the-uicontrol-start-button)小節。

>[!IMPORTANT]
>
>按一下[!UICONTROL 開始]按鈕會變更專案的狀態和[!UICONTROL 實際開始日期]。 如果其他人已開始處理任務或問題（將狀態變更為[!UICONTROL 進行中]並填入[!UICONTROL 實際開始日期]），即使您所屬的團隊已將該按鈕取代為[!UICONTROL 開始]按鈕，專案的按鈕仍會顯示為[!UICONTROL 處理它]。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>計劃</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡您的[!DNL Workfront]系統管理員。

## 設定[!UICONTROL 啟動]按鈕

如果您有[!UICONTROL 計畫]授權，您可以在[!UICONTROL 編輯]團隊視窗中為團隊設定[!UICONTROL 開始]按鈕。 為團隊啟用按鈕後，其運作方式如下：

* **已將團隊指派給工作專案**：如果將團隊指派給工作專案，則該團隊的成員會看到[!UICONTROL 開始]按鈕和為該團隊設定的狀態。
* **使用者屬於主團隊**：如果沒有團隊指派給工作專案，但使用者在其設定檔中被指派給主團隊，則使用者會看到[!UICONTROL 開始]按鈕和為該團隊設定的狀態。 如果您希望使用者經常使用[!UICONTROL 開始]按鈕，我們建議使用此情境。
* **將使用者指派給工作專案**：如果沒有團隊指派給工作專案，並且沒有主團隊指派給使用者，但使用者被指派給工作專案，則使用者會看到[!UICONTROL 開始]按鈕和為其指派的所有團隊設定的組合狀態。
* **使用者未指派給任何團隊：**&#x200B;如果沒有團隊指派給工作專案，而且沒有團隊指派給使用者（包括主團隊），而且專案已指派給使用者，則使用者看起來[!UICONTROL 處理它]按鈕。

>[!NOTE]
>
>此功能目前在中無法使用
>
>* [!DNL Workfront]行動應用程式
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront]個電子郵件通知
>

設定[開始]按鈕：

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 團隊]**。

1. 在&#x200B;**[!UICONTROL 團隊]**&#x200B;下拉式功能表中，選取團隊。\
   或\
   按一下&#x200B;**[!UICONTROL 建立團隊]**。

1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;圖示![](assets/more-icon.png)，然後按一下&#x200B;**[!UICONTROL 編輯]**。

1. 在[!UICONTROL 編輯團隊]頁面底部附近找到&#x200B;**[!UICONTROL 處理它]**&#x200B;按鈕區段。
1. 選取&#x200B;**[!UICONTROL 將處理它按鈕變更為開始按鈕以自動更新專案]**&#x200B;的狀態核取方塊。
1. 為每個工作專案型別選取一或多個狀態。 如果您選取多個狀態，當您按一下[!UICONTROL 開始]時，會出現一個下拉式功能表，您可在此選擇想要的狀態。
1. 按一下&#x200B;**[!UICONTROL 儲存變更]**。 當使用者被指派工作專案時，他們現在會看到[!UICONTROL 開始任務]或[!UICONTROL 開始問題]按鈕，而不是[!UICONTROL 處理它]按鈕。

   >[!NOTE]
   >
   >我們建議將團隊設定為使用者的主團隊，以便「開始」按鈕會出現在他們所有指派的工作專案上。 請參閱下方的[將使用者與主團隊](#associate-users-with-a-home-team)建立關聯。

## 將使用者與主團隊建立關聯

若要將使用者與主團隊建立關聯：

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**[!UICONTROL 使用者]**，然後選取您要與主團隊建立關聯的一或多個使用者。
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 編輯]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. 在&#x200B;**[!UICONTROL 組織]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 主團隊]**&#x200B;欄位。 開始輸入您想要與使用者建立關聯的團隊名稱。 當您在清單中看到團隊名稱時，請按一下該團隊的名稱。

1. 按一下「**[!UICONTROL 儲存變更]**」。\
   您選取的使用者現在與主團隊相關聯。

   這些使用者現在可以看到任何團隊設定，包括與[!UICONTROL 完成]按鈕相關聯的狀態。

