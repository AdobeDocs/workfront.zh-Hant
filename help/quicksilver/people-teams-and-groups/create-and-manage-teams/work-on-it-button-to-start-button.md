---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕
description: Adobe Workfront的預設設定包含「Work On It」按鈕，用於針對您已指派給的項目顯示的任務和問題。
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 取代 [!UICONTROL 努力] 按鈕 [!UICONTROL 開始] 按鈕

[!DNL Adobe Workfront]的預設設定包含 [!UICONTROL 努力] 按鈕，顯示已指派給的項目的任務和問題。 當您按一下 [!UICONTROL 努力] 對於指派給您的項目，您會向其他使用者發出訊號，告知您已收到工作，並確認您將會處理該工作。 不過， [!DNL Work On It] 按鈕不會更新任務或問題狀態以指示工作實際已啟動。

您可以取代 [!DNL Work On It] 按鈕 [!UICONTROL 開始] 按鈕。 在此情況下，您按一下 [!UICONTROL 開始] 按鈕而非 [!UICONTROL 努力]，會自動更新狀態和 [!UICONTROL 實際開始日期] 工作項目，表明你開始工作。 如需關於哪個團隊可能會影響您在 [!UICONTROL 努力] 按鈕，請參閱區段 [設定 [!UICONTROL 開始] 按鈕](#configure-the-uicontrol-start-button) 這篇文章。

>[!IMPORTANT]
>
>按一下 [!UICONTROL 開始] 按鈕將更改項目的狀態和 [!UICONTROL 實際開始日期]. 如果其他人已開始處理任務或問題(這會將狀態變更為 [!UICONTROL 進行中] 並填入 [!UICONTROL 實際開始日期])，項目的按鈕會顯示為 [!UICONTROL 努力] 即使您所屬的團隊已將按鈕更換為 [!UICONTROL 開始] 按鈕。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>計劃</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 設定 [!UICONTROL 開始] 按鈕

如果您有 [!UICONTROL 計畫] 許可證，您可以設定 [!UICONTROL 開始] 按鈕 [!UICONTROL 編輯] 團隊窗口。 以下為為團隊啟用按鈕後的運作方式：

* **該團隊被分配給工作項目**:如果將團隊分配給工作項，則該團隊的成員將看到 [!UICONTROL 開始] 按鈕和為該團隊配置的狀態。
* **使用者屬於首頁團隊**:如果未將任何團隊分配給工作項目，但用戶在其配置檔案中被分配給主團隊，則用戶將看到 [!UICONTROL 開始] 按鈕和為該團隊配置的狀態。 如果您希望使用者使用 [!UICONTROL 開始] 按鈕。
* **將用戶分配給工作項**:如果沒有為工作項分配任何團隊，並且沒有為用戶分配任何「主團隊」，但將用戶分配給該工作項，則用戶將看到 [!UICONTROL 開始] 按鈕，並為其分配給的所有團隊配置的組合狀態。
* **未將用戶分配給任何團隊：** 如果沒有為工作項分配任何團隊，並且沒有為用戶（包括主團隊）分配任何團隊，並且該項被分配給用戶，則用戶似乎是 [!UICONTROL 努力] 按鈕。

>[!NOTE]
>
>此功能目前在
>
>* 此 [!DNL Workfront] 行動應用程式
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] 電子郵件通知
>


配置「開始」按鈕：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 團隊]**.

1. 在 **[!UICONTROL 團隊]** 下拉式功能表，選取團隊。\
   或\
   按一下 **[!UICONTROL 建立團隊]**.

1. 按一下 **[!UICONTROL 更多]** 圖示 ![](assets/more-icon.png)，然後按一下 **[!UICONTROL 編輯]**.

1. 尋找 **[!UICONTROL 努力]** 按鈕區段 [!UICONTROL 編輯團隊] 頁面。
1. 選取 **[!UICONTROL 將Work On It按鈕更改為Start按鈕，以自動更新項目的狀態]** 框。
1. 為每個工作項類型選擇一個或多個狀態。 如果您選取多個狀態，當您按一下「 」時，下拉式功能表隨即出現 [!UICONTROL 開始] 您可以在其中選擇所需狀態。
1. 按一下 **[!UICONTROL 儲存變更]**. 使用者現在會看到 [!UICONTROL 啟動任務] 或 [!UICONTROL 開始問題] 按鈕，而非 [!UICONTROL 努力] 按鈕。

   >[!NOTE]
   >
   >我們建議將團隊設定為使用者的主團隊，這樣開始按鈕就會顯示在其所有指派的工作項目上。 請參閱 [將使用者與首頁團隊關聯](#associate-users-with-a-home-team) 下方。

## 將使用者與首頁團隊關聯

將用戶與主團隊關聯：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront].

1. 按一下 **[!UICONTROL 使用者]**，然後選擇要與主團隊關聯的用戶或組。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 組織]** 區段，選取 **[!UICONTROL 主隊]** 欄位。 開始鍵入要與用戶關聯的團隊的名稱。 在清單中看到團隊的名稱時，按一下該團隊的名稱。

1. 按一下 **[!UICONTROL 儲存變更]**.\
   您選取的使用者現在與首頁團隊相關聯。

   任何團隊設定，包括與 [!UICONTROL 完成] 按鈕。

