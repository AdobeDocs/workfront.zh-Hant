---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 配置任務的完成按鈕
description: 「完成」按鈕可自動設定任務或問題的狀態。 依預設，當受託人按一下其工作項目的「完成」時，Adobe Workfront會將任務標示為「完成」。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# 設定 [!UICONTROL 完成] 任務按鈕

此 [!UICONTROL 完成] 按鈕可以自動設定任務或問題的狀態。 依預設， [!UICONTROL Adobe Workfront] 將任務標籤為 [!UICONTROL 已完成] 當受託人按一下其工作項目的「完成」時。

## 總覽

具有特定權限的使用者可以設定 [!UICONTROL 完成] 按鈕來反映系統中的某些狀態。 有兩種不同的方式 [!UICONTROL 完成] 按鈕適用於中的任務 [!UICONTROL Workfront]:

* 如果用戶已分配了「主團隊」，則 [!DNL Workfront] 管理員或使用 [!UICONTROL 計畫] 授權可設定 [!UICONTROL 完成] 按鈕來反映團隊成員的某些狀態。 請參閱 [設定 [!UICONTROL 完成] 按鈕](#configure-the-uicontrol-done-button-for-a-team) 這篇文章。
* 若使用者未獲派主團隊，則 [!UICONTROL 完成] 「 」按鈕會系結至完成狀態。 此情境中沒有可用的配置選項。 此 [!UICONTROL 完成] 按鈕自動預設為此狀態。

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
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 設定 [!UICONTROL 完成] 按鈕

您可以使用 [!UICONTROL 完成] 按鈕。 您也可以設定多個狀態，並允許使用者選擇適當的狀態。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 表徵圖，然後從下拉菜單中選擇新團隊，或在搜索欄中搜索團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後按一下 **[!UICONTROL 編輯]**.
1. 尋找 **[!UICONTROL 完成按鈕]** 區段 **[!UICONTROL 團隊設定]** 頁面。

1. 為每個工作項類型選擇一個或多個狀態。

   >[!NOTE]
   >
   >為任務或問題選擇狀態時，請考慮以下事項：
   >
   >* 當您為每種類型的工作項目選擇一個狀態時，當用戶按一下時，任務或問題狀態將設定為該狀態 [!UICONTROL 完成] 在他們的項目上。 如果您為每種類型的工作項目設定多個狀態，則下拉式功能表會新增至 [!UICONTROL 完成] 按鈕和用戶必須選擇狀態才能更改工作項的狀態。
   >* 您只能將系統層級狀態與 [!UICONTROL 完成] 按鈕。 您不能將特定組狀態與工作項狀態關聯。
   >* 當被指派給項目的使用者將項目置於與 [!UICONTROL 完成] 按鈕，項目顯示為 [!UICONTROL 完成] 無論您選取的狀態是否為 [!UICONTROL 已完成] 或 [!UICONTROL 已關閉] 狀態或工作狀態。

   >   
   >   
   >  例如，將 [!UICONTROL 完成] 按鈕 [!UICONTROL 進行中] 使工作項顯示為 [!UICONTROL 完成] 從 [!UICONTROL 新增] to [!UICONTROL 正在進行中].
   >   
   >* 問題類型可自訂，其名稱可能與您環境中列出的名稱不同。\
      >  預設任務和問題類型如下：
      >     
      >   * [!UICONTROL 任務]
      >   * [!UICONTROL 問題]
      >   * [!UICONTROL 請求]
      >   * [!UICONTROL 變更順序]
      >   * [!UICONTROL 錯誤報告]


   如果將任務或問題分配給多個用戶，您會看到「[!UICONTROL 完成我的任務]」選項，以及為您的團隊選擇的多個狀態。

1. 按一下 **[!UICONTROL 儲存變更]**.

## 將使用者與首頁團隊關聯

若要變更 [!UICONTROL 完成] 按鈕功能對用戶可見，您可以讓您的設定更改了用戶的「主團隊」的團隊。

將用戶與主團隊關聯：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront].

1. 按一下 **[!UICONTROL 使用者]**，然後選擇要與主團隊關聯的用戶或組。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 組織]** 區段，選取 **[!UICONTROL 主隊]** 欄位。 開始鍵入要與用戶關聯的團隊的名稱。 在清單中看到團隊的名稱時，按一下該團隊的名稱。

1. 按一下 **[!UICONTROL 儲存變更]**.\
   您選取的使用者現在與首頁團隊相關聯。
任何團隊設定，包括與 [!UICONTROL 完成] 按鈕。
